> [!CAUTION]
>
> Dieses Dokument ist veraltet, bitte nicht darauf verweisen.

<h2 id="toc">Inhaltsverzeichnis</h2>
Das vorliegende Projekt unterstützt zwei Arten von APIs, alle Methoden benötigen Redis;

- [Funktionsaufrufe in Python](#api-python)
- [HTTP-Protokolle](#api-http)

---

<h2 id="api-python">Python</h2>

Da `pdf2zh` ein installiertes Modul in Python ist, stellen wir zwei Methoden zur Verfügung, die von anderen Programmen in beliebigen Python-Skripten aufgerufen werden können.

Wenn Sie beispielsweise ein Dokument von Englisch ins Chinesische mit Google Translate übersetzen möchten, können Sie den folgenden Code verwenden:

```python
from pdf2zh_next import translate, translate_stream

params = {
    'lang_in': 'en',
    'lang_out': 'zh',
    'service': 'google',
    'thread': 4,
}
```

Übersetzen mit Dateien:

```python
(file_mono, file_dual) = translate(files=['example.pdf'], **params)[0]
```

```bash
pdf2zh --stream
```

[!NOTE]
The `--stream` option is only available in `PDFMathTranslate` version 0.1.0 and above.

[Home](#startseite) | [Getting Start](#erste-schritte) | [Installation](#installation) | [Command Line](#kommandozeile) | [Usage](#verwendung) | [Language Code](#sprachcode) | [Documentation of Translation Services](#dokumentation-der-übersetzungsdienste) | [Getting Started](#erste-schritte) | [Advanced](#erweiterte-optionen) | [Support Languages](#unterstützte-sprachen) | [Community](#gemeinschaft) | [FAQ](#häufig-gestellte-fragen)

```python
with open('example.pdf', 'rb') as f:
    (stream_mono, stream_dual) = translate_stream(stream=f.read(), **params)
```

[⬆️ Zurück zum Anfang](#toc)

---

<h2 id="api-http">HTTP</h2>

Auf eine flexiblere Weise können Sie mit dem Programm über HTTP-Protokolle kommunizieren, wenn:

1. Backend installieren und ausführen

   ```bash
   pip install pdf2zh_next[backend]
   pdf2zh_next --flask
   pdf2zh_next --celery worker
   ```

2. Verwendung von HTTP-Protokollen wie folgt:

   - Übersetzungsaufgabe einreichen

     ```bash
     curl http://localhost:11008/v1/translate -F "file=@example.pdf" -F "data={\"lang_in\":\"en\",\"lang_out\":\"zh\",\"service\":\"google\",\"thread\":4}"
     {"id":"d9894125-2f4e-45ea-9d93-1a9068d2045a"}
     ```

- Fortschritt überprüfen

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"info":{"n":13,"total":506},"state":"PROGRESS"}
     ```

- Fortschritt prüfen _(falls abgeschlossen)_

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"state":"SUCCESS"}
     ```

- Monolinguale Datei speichern

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/mono --output example-mono.pdf
     ```

- Bilinguale Datei speichern

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/dual --output example-dual.pdf
     ```

- Unterbrechen, wenn aktiv, und Aufgabe löschen
     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a -X DELETE
     ```

[⬆️ Zurück zum Anfang](#toc)

---

<div align="right"> 
<h6><small>Ein Teil des Inhalts dieser Seite wurde von GPT übersetzt und kann Fehler enthalten.</small></h6>