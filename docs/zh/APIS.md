> [!CAUTION]
>
> 本文档已过时，请勿参考。

<h2 id="toc">目录</h2>
当前项目支持两种类型的 API，所有方法都需要 Redis；

- [Python 中的函数调用](#api-python)
- [HTTP 协议](#api-http)

---

<h2 id="api-python">Python</h2>

由于 `pdf2zh` 是 Python 中的一个已安装模块，我们提供了两种方法供其他程序在任何 Python 脚本中调用。

例如，如果你想使用 Google Translate 将文档从英语翻译成中文，可以使用以下代码：

```python
from pdf2zh_next import translate, translate_stream

params = {
    'lang_in': 'en',
    'lang_out': 'zh',
    'service': 'google',
    'thread': 4,
}
```
通过文件翻译：
```python
(file_mono, file_dual) = translate(files=['example.pdf'], **params)[0]
```
流式翻译：
```python
with open('example.pdf', 'rb') as f:
    (stream_mono, stream_dual) = translate_stream(stream=f.read(), **params)
```

[⬆️ 返回顶部](#目录)

---

<h2 id="api-http">HTTP</h2>

以更灵活的方式，您可以通过 HTTP 协议与程序进行通信，前提是：

1. 安装并运行后端服务

   ```bash
   pip install pdf2zh_next[backend]
   pdf2zh_next --flask
   pdf2zh_next --celery worker
   ```

2. 通过 HTTP 协议按以下方式使用：

   - 提交翻译任务

     ```bash
     curl http://localhost:11008/v1/translate -F "file=@example.pdf" -F "data={\"lang_in\":\"en\",\"lang_out\":\"zh\",\"service\":\"google\",\"thread\":4}"
     {"id":"d9894125-2f4e-45ea-9d93-1a9068d2045a"}
     ```

   - 检查进度

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"info":{"n":13,"total":506},"state":"PROGRESS"}
     ```

   - 检查进度 _(如果已完成)_

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"state":"SUCCESS"}
     ```

   - 保存单语文件

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/mono --output example-mono.pdf
     ```

   - 保存双语文件

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/dual --output example-dual.pdf
     ```

   - 如果任务正在运行则中断并删除任务
     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a -X DELETE
     ```

[⬆️ 返回顶部](#目录)

---

<div align="right"> 
<h6><small>本页面的部分内容由 GPT 翻译，可能包含错误。</small></h6>