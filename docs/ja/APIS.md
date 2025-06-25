> [!CAUTION]
>
> このドキュメントは古くなっていますので、参照しないでください。

<h2 id="toc">目次</h2>
現在のプロジェクトは2種類のAPIをサポートしており、すべてのメソッドにはRedisが必要です。

- [Pythonでの関数呼び出し](#api-python)
- [HTTPプロトコル](#api-http)

---

<h2 id="api-python">Python</h2>

`pdf2zh`はPythonのインストール済みモジュールであるため、他のプログラムが任意のPythonスクリプトで呼び出せる2つのメソッドを公開しています。

例えば、Google翻訳を使用して英語から中国語に文書を翻訳したい場合、以下のコードを使用できます:

```python
from pdf2zh_next import translate, translate_stream

params = {
    'lang_in': 'en',
    'lang_out': 'zh',
    'service': 'google',
    'thread': 4,
}
```

ファイルを使用して翻訳:

```python
(file_mono, file_dual) = translate(files=['example.pdf'], **params)[0]
```

```markdown
# ホーム

## 始め方

### インストール

`pdf2zh` をインストールするには、以下のコマンドをコマンドラインで実行してください：

```bash
pip install pdf2zh
```

### 使い方

基本的な使い方は以下の通りです：

```bash
pdf2zh input.pdf output.pdf
```

## 翻訳サービスドキュメント

### 開始

`PDFMathTranslate` を使用してPDFを翻訳する方法について説明します。

### 高度な設定

翻訳の精度を向上させるための高度な設定オプションです。

## サポート言語

現在サポートされている言語コードの一覧です。

## コミュニティ

質問やフィードバックはコミュニティで共有してください。

## よくある質問

よくある質問とその回答をまとめました。
```

```python
with open('example.pdf', 'rb') as f:
    (stream_mono, stream_dual) = translate_stream(stream=f.read(), **params)
```

[⬆️ トップに戻る](#toc)

---

<h2 id="api-http">HTTP</h2>

より柔軟な方法として、以下の条件を満たす場合、HTTPプロトコルを使用してプログラムと通信できます：

1. バックエンドのインストールと実行

   ```bash
   pip install pdf2zh_next[backend]
   pdf2zh_next --flask
   pdf2zh_next --celery worker
   ```

2. HTTPプロトコルを使用する方法は以下の通りです:

   - 翻訳タスクを送信

     ```bash
     curl http://localhost:11008/v1/translate -F "file=@example.pdf" -F "data={\"lang_in\":\"en\",\"lang_out\":\"zh\",\"service\":\"google\",\"thread\":4}"
     {"id":"d9894125-2f4e-45ea-9d93-1a9068d2045a"}
     ```

- 進捗確認

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"info":{"n":13,"total":506},"state":"PROGRESS"}
     ```

- 進捗確認 _(完了した場合)_

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"state":"SUCCESS"}
     ```

- 単一言語ファイルを保存

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/mono --output example-mono.pdf
     ```

- バイリンガルファイルを保存

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/dual --output example-dual.pdf
     ```

- 実行中の場合は中断してタスクを削除
     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a -X DELETE
     ```

[⬆️ トップに戻る](#toc)

---

<div align="right"> 
<h6><small>このページの一部のコンテンツはGPTによって翻訳されており、エラーが含まれている可能性があります。</small></h6>