> [!CAUTION]
>
> このドキュメントは古くなっていますので、参照しないでください。

<h2 id="目次">目次</h2>
本プロジェクトは 2 種類の API をサポートしており、すべてのメソッドには Redis が必要です。

- [Python での関数呼び出し](#api-python)
- [HTTP プロトコル](#api-http)

---

<h2 id="api-python">Python</h2>

`pdf2zh` は Python のインストール済みモジュールであるため、他のプログラムが任意の Python スクリプトで呼び出せるように 2 つのメソッドを公開しています。

例えば、Google 翻訳を使用して英語から中国語に文書を翻訳したい場合、以下のコードを使用できます：

```python
from pdf2zh_next import translate, translate_stream

params = {
    'lang_in': 'en',
    'lang_out': 'zh',
    'service': 'google',
    'thread': 4,
}
```
ファイルで翻訳：
```python
(file_mono, file_dual) = translate(files=['example.pdf'], **params)[0]
```
ストリームで翻訳：
```python
with open('example.pdf', 'rb') as f:
    (stream_mono, stream_dual) = translate_stream(stream=f.read(), **params)
```

[⬆️ トップに戻る](#toc)

---

<h2 id="api-http">HTTP</h2>

より柔軟な方法として、以下の場合には HTTP プロトコルを使用してプログラムと通信できます：

1. バックエンドのインストールと実行

   ```bash
   pip install pdf2zh_next[backend]
   pdf2zh_next --flask
   pdf2zh_next --celery worker
   ```

2. HTTP プロトコルを使用する方法：

   - 翻訳タスクの送信

     ```bash
     curl http://localhost:11008/v1/translate -F "file=@example.pdf" -F "data={\"lang_in\":\"en\",\"lang_out\":\"zh\",\"service\":\"google\",\"thread\":4}"
     {"id":"d9894125-2f4e-45ea-9d93-1a9068d2045a"}
     ```

   - 進捗状況の確認

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"info":{"n":13,"total":506},"state":"PROGRESS"}
     ```

   - 進捗状況の確認（完了時）

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"state":"SUCCESS"}
     ```

   - 単一言語ファイルの保存

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/mono --output example-mono.pdf
     ```

   - 二言語ファイルの保存

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/dual --output example-dual.pdf
     ```

   - 実行中のタスクを中断して削除
     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a -X DELETE
     ```

[⬆️ トップに戻る](#toc)

---

<div align="right"> 
<h6><small>このページの一部のコンテンツは GPT によって翻訳されており、エラーが含まれている可能性があります。</small></h6>