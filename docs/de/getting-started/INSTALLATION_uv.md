[**Erste Schritte**](./getting-started.md) > **Installation** > **uv** _(aktuell)_

---

### Installieren Sie PDFMathTranslate über uv

#### Was ist uv? Wie installiert man es?

uv ist ein extrem schneller Python-Paket- und Projektmanager, geschrieben in Rust.
<br>
Um uv auf Ihrem Computer zu installieren, lesen Sie bitte [diesen Artikel](https://docs.astral.sh/uv/getting-started/installation/).

---

#### Installation

1. Python installiert (3.10 <= Version <= 3.12);

2. Verwenden Sie den folgenden Befehl, um unser Paket zu nutzen:

    ```bash
    pip install uv
    uv tool install --python 3.12 pdf2zh-next
    ```

Nach der Installation können Sie mit der Übersetzung über die **Kommandozeile** oder **WebUI** beginnen.

!!! Warning

    Wenn Sie beim Ausführen den Fehler `command not found: pdf2zh_next` sehen, konfigurieren Sie bitte die Umgebungsvariablen wie folgt und versuchen Sie es erneut:

    === "macOS und Linux"

        Fügen Sie Folgendes zu Ihrer ~/.zshrc hinzu:

        ```console
        export PATH="$PATH:/Users/Username/.local/bin"
        ```

        Starten Sie dann Ihr Terminal neu

    === "Windows"

        Geben Sie Folgendes in PowerShell ein:

        ```powershell
        $env:Path = "C:\Users\Username\.local\bin;$env:Path"
        ```

        Starten Sie dann Ihr Terminal neu

> [!NOTE]
> Wenn Sie während der Verwendung der WebUI auf Probleme stoßen, lesen Sie bitte [Verwendung --> WebUI](./USAGE_webui.md).

> [!NOTE]
> Wenn Sie während der Verwendung der Kommandozeile auf Probleme stoßen, lesen Sie bitte [Verwendung --> Kommandozeile](./USAGE_commandline.md).

<div align="right"> 
<h6><small>Ein Teil des Inhalts dieser Seite wurde von GPT übersetzt und kann Fehler enthalten.</small></h6>