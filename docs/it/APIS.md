> [!CAUTION]
>
> Questo documento è obsoleto, si prega di non farvi riferimento.

<h2 id="toc">Indice dei contenuti</h2>
Il presente progetto supporta due tipi di API, tutti i metodi necessitano di Redis;

- [Chiamate funzionali in Python](#api-python)
- [Protocolli HTTP](#api-http)

---

<h2 id="api-python">Python</h2>

Poiché `pdf2zh` è un modulo installato in Python, esponiamo due metodi che altri programmi possono chiamare in qualsiasi script Python.

Ad esempio, se desideri tradurre un documento dall'inglese al cinese utilizzando Google Translate, puoi utilizzare il seguente codice:

```python
from pdf2zh_next import translate, translate_stream

params = {
    'lang_in': 'en',
    'lang_out': 'zh',
    'service': 'google',
    'thread': 4,
}
```
Traduci con i file:
```python
(file_mono, file_dual) = translate(files=['example.pdf'], **params)[0]
```
Traduci con flusso:
```python
with open('example.pdf', 'rb') as f:
    (stream_mono, stream_dual) = translate_stream(stream=f.read(), **params)
```

[⬆️ Torna all'inizio](#toc)

---

<h2 id="api-http">HTTP</h2>

In un modo più flessibile, puoi comunicare con il programma utilizzando i protocolli HTTP, se:

1. Installa ed esegui il backend

   ```bash
   pip install pdf2zh_next[backend]
   pdf2zh_next --flask
   pdf2zh_next --celery worker
   ```

2. Utilizza i protocolli HTTP come segue:

   - Invia un task di traduzione

     ```bash
     curl http://localhost:11008/v1/translate -F "file=@example.pdf" -F "data={\"lang_in\":\"en\",\"lang_out\":\"zh\",\"service\":\"google\",\"thread\":4}"
     {"id":"d9894125-2f4e-45ea-9d93-1a9068d2045a"}
     ```

   - Controlla lo stato

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"info":{"n":13,"total":506},"state":"PROGRESS"}
     ```

   - Controlla lo stato _(se completato)_

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"state":"SUCCESS"}
     ```

   - Salva il file monolingue

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/mono --output example-mono.pdf
     ```

   - Salva il file bilingue

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/dual --output example-dual.pdf
     ```

   - Interrompi se in esecuzione ed elimina il task
     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a -X DELETE
     ```

[⬆️ Torna all'inizio](#toc)

---

<div align="right"> 
<h6><small>Parte del contenuto di questa pagina è stata tradotta da GPT e potrebbe contenere errori.</small></h6>