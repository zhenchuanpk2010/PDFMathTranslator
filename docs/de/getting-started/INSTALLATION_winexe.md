[**Erste Schritte**](./getting-started.md) > **Installation** > **Windows EXE** _(aktuell)_

---

### Installieren Sie PDFMathTranslate über eine .exe-Datei

***Schritt 1*** | Laden Sie `pdf2zh-<version>-with-assets-win64.zip` von der [release page](https://github.com/PDFMathTranslate/PDFMathTranslate-next/releases) herunter.

> [!TIP]
> **Was ist der Unterschied zwischen `pdf2zh-<version>-with-assets-win64.zip` und `pdf2zh-<version>-win64.zip`?**
>
> - Wenn Sie PDFMathTranslate zum ersten Mal herunterladen und verwenden, wird empfohlen, `pdf2zh-<version>-with-assets-win64.zip` herunterzuladen.
> - Die `pdf2zh-<version>-with-assets-win64.zip` enthält im Vergleich zu `pdf2zh-<version>-win64.zip` zusätzliche Ressourcendateien (wie Schriftarten und Modelle).
> - Die Version ohne Assets lädt die Ressourcen beim Ausführen dynamisch nach, aber der Download kann aufgrund von Netzwerkproblemen fehlschlagen.

***Schritt 2*** | Entpacken Sie `pdf2zh-<version>-with-assets-win64.zip` und navigieren Sie zum Ordner `pdf2zh`. Das Entpacken dauert eine Weile, bitte haben Sie Geduld.

***Schritt 3*** | Navigieren Sie zum Ordner `pdf2zh` und doppelklicken Sie dann auf `pdf2zh.exe`.

> [!TIP]
> **Kann die .exe-Datei nicht ausführen**
>
> Wenn Sie Probleme beim Ausführen von pdf2zh.exe haben, installieren Sie bitte `https://aka.ms/vs/17/release/vc_redist.x64.exe` und versuchen Sie es erneut.

***Schritt 4*** | Nach dem Doppelklicken auf die exe-Datei öffnet sich ein Terminal. Nach etwa einer halben bis einer Minute öffnet sich eine Webseite in Ihrem Standardbrowser. Falls dies nicht geschieht, können Sie versuchen, manuell auf `http://localhost:7860/` zuzugreifen.

> [!NOTE]
>
> Wenn Sie Probleme bei der Verwendung von WebUI haben, lesen Sie bitte [diese Webseite](./USAGE_webui.md).

***Schritt 5*** | Viel Spaß!

> [!TIP]
> **Sie können die .exe-Datei über die Kommandozeile verwenden**
>
> Verwenden Sie die .exe-Datei über die Kommandozeile wie folgt:
>
> - Starten Sie Ihr Terminal und navigieren Sie zum Ordner, der die .exe-Datei enthält:
>
> ```bash
> cd /path/pdf2zh_next/build
> ```
>
> - Rufen Sie die .exe-Datei auf:
>
> ```bash
> ./pdf2zh_next.exe "document.pdf"
> ```
>
> Sie können andere Kommandozeilenparameter wie gewohnt verwenden:
>
> ```bash
> ./pdf2zh_next.exe "document.pdf" --lang-in en --lang-out ja
> ```
>
> Wenn Sie weitere Informationen zur Verwendung der Kommandozeile benötigen, lesen Sie bitte diesen Artikel.

<div align="right"> 
<h6><small>Ein Teil des Inhalts dieser Seite wurde von GPT übersetzt und kann Fehler enthalten.</small></h6>