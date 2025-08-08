> [!CAUTION]
>
> 本文件已過時，請勿參考。

<h2 id="目錄">目錄</h2>
本項目支持兩種類型的 API，所有方法都需要 Redis；

- [Python 中的函數調用](#api-python)
- [HTTP 協議](#api-http)

---

<h2 id="api-python">Python</h2>

由於 `pdf2zh` 是 Python 中的一個已安裝模組，我們提供了兩種方法供其他程式在任何 Python 腳本中調用。

例如，如果你想使用 Google 翻譯將文件從英文翻譯成中文，可以使用以下代碼：

```python
from pdf2zh_next import translate, translate_stream

params = {
    'lang_in': 'en',
    'lang_out': 'zh',
    'service': 'google',
    'thread': 4,
}
```
使用檔案翻譯：
```python
(file_mono, file_dual) = translate(files=['example.pdf'], **params)[0]
```
串流翻譯：
```python
with open('example.pdf', 'rb') as f:
    (stream_mono, stream_dual) = translate_stream(stream=f.read(), **params)
```

[⬆️ 返回頂部](#目錄)

---

<h2 id="api-http">HTTP</h2>

以更靈活的方式，您可以使用 HTTP 協議與程序進行通信，如果：

1. 安裝並運行後端

   ```bash
   pip install pdf2zh_next[backend]
   pdf2zh_next --flask
   pdf2zh_next --celery worker
   ```

2. 使用以下 HTTP 協議：

   - 提交翻譯任務

     ```bash
     curl http://localhost:11008/v1/translate -F "file=@example.pdf" -F "data={\"lang_in\":\"en\",\"lang_out\":\"zh\",\"service\":\"google\",\"thread\":4}"
     {"id":"d9894125-2f4e-45ea-9d93-1a9068d2045a"}
     ```

   - 檢查進度

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"info":{"n":13,"total":506},"state":"PROGRESS"}
     ```

   - 檢查進度 _(如果已完成)_

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"state":"SUCCESS"}
     ```

   - 保存單語文件

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/mono --output example-mono.pdf
     ```

   - 保存雙語文件

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/dual --output example-dual.pdf
     ```

   - 如果正在運行則中斷並刪除任務
     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a -X DELETE
     ```

[⬆️ 返回頂部](#目錄)

---

<div align="right"> 
<h6><small>Some content on this page has been translated by GPT and may contain errors.</small></h6>