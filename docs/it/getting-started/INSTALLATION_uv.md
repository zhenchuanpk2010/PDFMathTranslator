[**Iniziare**](./getting-started.md) > **Installazione** > **uv** _(current)_

---

### Installa PDFMathTranslate tramite uv

#### Cos'è uv? Come installarlo?

uv è un gestore di pacchetti e progetti Python estremamente veloce, scritto in Rust.
<br>
Per installare uv sul tuo computer, consulta [questo articolo](https://docs.astral.sh/uv/getting-started/installation/).

---

#### Installazione

1. Python installato (3.10 <= versione <= 3.12);

2. Utilizza il seguente comando per usare il nostro pacchetto:

    ```bash
    pip install uv
    uv tool install --python 3.12 pdf2zh-next
    ```

Dopo l'installazione, puoi iniziare la traduzione tramite la **riga di comando** o **WebUI**.

!!! Warning

    Se vedi l'errore `command not found: pdf2zh_next` durante l'esecuzione, configura le variabili d'ambiente come segue e riprova:

    === "macOS e Linux"

        Aggiungi quanto segue al tuo ~/.zshrc:

        ```console
        export PATH="$PATH:/Users/Username/.local/bin"
        ```

        Quindi riavvia il terminale

    === "Windows"

        Inserisci quanto segue in PowerShell:

        ```powershell
        $env:Path = "C:\Users\Username\.local\bin;$env:Path"
        ```

        Quindi riavvia il terminale

> [!NOTE]
> Se riscontri problemi durante l'utilizzo di WebUI, consulta [Utilizzo --> WebUI](./USAGE_webui.md).

> [!NOTE]
> Se riscontri problemi durante l'utilizzo della riga di comando, consulta [Utilizzo --> Riga di comando](./USAGE_commandline.md).

<div align="right"> 
<h6><small>Parte del contenuto di questa pagina è stata tradotta da GPT e potrebbe contenere errori.</small></h6>