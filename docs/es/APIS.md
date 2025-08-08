> [!CAUTION]
>
> Este documento está desactualizado, por favor no lo consultes.

<h2 id="toc">Tabla de contenido</h2>
El presente proyecto soporta dos tipos de APIs, todos los métodos necesitan Redis;

- [Llamadas funcionales en Python](#api-python)
- [Protocolos HTTP](#api-http)

---

<h2 id="api-python">Python</h2>

Como `pdf2zh` es un módulo instalado en Python, exponemos dos métodos para que otros programas puedan llamar en cualquier script de Python.

Por ejemplo, si deseas traducir un documento del inglés al chino usando Google Translate, puedes usar el siguiente código:

```python
from pdf2zh_next import translate, translate_stream

params = {
    'lang_in': 'en',
    'lang_out': 'zh',
    'service': 'google',
    'thread': 4,
}
```
Traducir con archivos:
```python
(file_mono, file_dual) = translate(files=['example.pdf'], **params)[0]
```
Traducir con transmisión:
```python
with open('example.pdf', 'rb') as f:
    (stream_mono, stream_dual) = translate_stream(stream=f.read(), **params)
```

[⬆️ Volver arriba](#toc)

---

<h2 id="api-http">HTTP</h2>

De una manera más flexible, puedes comunicarte con el programa utilizando protocolos HTTP, si:

1. Instalar y ejecutar el backend

   ```bash
   pip install pdf2zh_next[backend]
   pdf2zh_next --flask
   pdf2zh_next --celery worker
   ```

2. Usar los protocolos HTTP de la siguiente manera:

   - Enviar tarea de traducción

     ```bash
     curl http://localhost:11008/v1/translate -F "file=@example.pdf" -F "data={\"lang_in\":\"en\",\"lang_out\":\"zh\",\"service\":\"google\",\"thread\":4}"
     {"id":"d9894125-2f4e-45ea-9d93-1a9068d2045a"}
     ```

   - Verificar progreso

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"info":{"n":13,"total":506},"state":"PROGRESS"}
     ```

   - Verificar progreso _(si está completado)_

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"state":"SUCCESS"}
     ```

   - Guardar archivo monolingüe

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/mono --output example-mono.pdf
     ```

   - Guardar archivo bilingüe

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/dual --output example-dual.pdf
     ```

   - Interrumpir si está en ejecución y eliminar la tarea
     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a -X DELETE
     ```

[⬆️ Volver arriba](#toc)

---

<div align="right"> 
<h6><small>Parte del contenido de esta página ha sido traducido por GPT y puede contener errores.</small></h6>