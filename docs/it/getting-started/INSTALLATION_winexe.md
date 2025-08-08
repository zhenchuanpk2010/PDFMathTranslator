[**Iniziare**](./getting-started.md) > **Installazione** > **Windows EXE** _(current)_

---

### Installa PDFMathTranslate tramite file .exe

***Passo 1*** | Scarica `pdf2zh-<version>-with-assets-win64.zip` dalla [pagina delle release](https://github.com/PDFMathTranslate/PDFMathTranslate-next/releases).

> [!TIP]
> **Qual è la differenza tra `pdf2zh-<version>-with-assets-win64.zip` e `pdf2zh-<version>-win64.zip`?**
>
> - Se stai scaricando e utilizzando PDFMathTranslate per la prima volta, si consiglia di scaricare `pdf2zh-<version>-with-assets-win64.zip`.
> - Il file `pdf2zh-<version>-with-assets-win64.zip` include file di risorse (come font e modelli) rispetto a `pdf2zh-<version>-win64.zip`.
> - La versione senza risorse scaricherà anche dinamicamente le risorse durante l'esecuzione, ma il download potrebbe fallire a causa di problemi di rete.

***Passo 2*** | Decomprimi `pdf2zh-<version>-with-assets-win64.zip` e accedi alla cartella `pdf2zh`. La decompressione richiede del tempo, sii paziente.

***Passo 3*** | Accedi alla cartella `pdf2zh`, quindi fai doppio clic su `pdf2zh.exe`.

> [!TIP]
> **Non riesci a eseguire il file .exe**
>
> Se hai problemi nell'eseguire pdf2zh.exe, installa `https://aka.ms/vs/17/release/vc_redist.x64.exe` e riprova.

***Passo 4*** | Dopo aver fatto doppio clic sul file exe, apparirà un terminale. Dopo circa mezzo minuto o un minuto, una pagina web si aprirà nel tuo browser predefinito. Se ciò non accade, puoi provare ad accedere manualmente a `http://localhost:7860/`.

> [!NOTE]
>
> Se riscontri problemi durante l'utilizzo di WebUI, consulta [questa pagina web](./USAGE_webui.md).

***Passo 5*** | Goditelo!

> [!TIP]
> **Puoi utilizzare il file .exe tramite riga di comando**
>
> Utilizza il file .exe tramite riga di comando come segue:
>
> - Avvia il terminale e naviga nella cartella contenente il file .exe:
>
> ```bash
> cd /path/pdf2zh_next/build
> ```
>
> - Chiama il file .exe:
>
> ```bash
> ./pdf2zh_next.exe "document.pdf"
> ```
>
> Puoi utilizzare altri parametri della riga di comando come al solito:
>
> ```bash
> ./pdf2zh_next.exe "document.pdf" --lang-in en --lang-out ja
> ```
>
> Se hai bisogno di maggiori informazioni sull'utilizzo della riga di comando, consulta questo articolo.

<div align="right"> 
<h6><small>Parte del contenuto di questa pagina è stata tradotta da GPT e potrebbe contenere errori.</small></h6>