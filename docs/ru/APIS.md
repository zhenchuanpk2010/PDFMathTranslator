> [!CAUTION]
>
> Этот документ устарел, пожалуйста, не используйте его.

<h2 id="содержание">Содержание</h2>
Настоящий проект поддерживает два типа API, все методы требуют Redis;

- [Функциональные вызовы в Python](#api-python)
- [HTTP протоколы](#api-http)

---

<h2 id="api-python">Python</h2>

Поскольку `pdf2zh` является установленным модулем в Python, мы предоставляем два метода для вызова другими программами в любых скриптах на Python.

Например, если вы хотите перевести документ с английского на китайский с помощью Google Translate, вы можете использовать следующий код:

```python
from pdf2zh_next import translate, translate_stream

params = {
    'lang_in': 'en',
    'lang_out': 'zh',
    'service': 'google',
    'thread': 4,
}
```
Перевод с файлами:
```python
(file_mono, file_dual) = translate(files=['example.pdf'], **params)[0]
```
Перевод с потоком:
```python
with open('example.pdf', 'rb') as f:
    (stream_mono, stream_dual) = translate_stream(stream=f.read(), **params)
```

[⬆️ Наверх](#toc)

---

<h2 id="api-http">HTTP</h2>

Более гибкий способ взаимодействия с программой — использование протокола HTTP, если:

1. Установка и запуск бэкенда

   ```bash
   pip install pdf2zh_next[backend]
   pdf2zh_next --flask
   pdf2zh_next --celery worker
   ```

2. Использование HTTP-протоколов следующим образом:

   - Отправка задачи перевода

     ```bash
     curl http://localhost:11008/v1/translate -F "file=@example.pdf" -F "data={\"lang_in\":\"en\",\"lang_out\":\"zh\",\"service\":\"google\",\"thread\":4}"
     {"id":"d9894125-2f4e-45ea-9d93-1a9068d2045a"}
     ```

   - Проверка прогресса

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"info":{"n":13,"total":506},"state":"PROGRESS"}
     ```

   - Проверка прогресса _(если завершено)_

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"state":"SUCCESS"}
     ```

   - Сохранение одноязычного файла

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/mono --output example-mono.pdf
     ```

   - Сохранение двуязычного файла

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/dual --output example-dual.pdf
     ```

   - Прерывание, если выполняется, и удаление задачи
     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a -X DELETE
     ```

[⬆️ Наверх](#toc)

---

<div align="right"> 
<h6><small>Часть содержимого этой страницы была переведена GPT и может содержать ошибки.</small></h6>