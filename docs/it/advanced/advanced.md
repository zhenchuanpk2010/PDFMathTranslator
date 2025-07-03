[**Opzioni avanzate**](./introduction.md) > **Opzioni avanzate** _(current)_

---

<h3 id="toc">Indice</h3>

- [Argomenti della riga di comando](#argomenti-della-riga-di-comando)
- [Traduzione parziale](#traduzione-parziale)
- [Specificare le lingue di origine e di destinazione](#specificare-le-lingue-di-origine-e-di-destinazione)
- [Tradurre con eccezioni](#tradurre-con-eccezioni)
- [Prompt personalizzato](#prompt-personalizzato)
- [Configurazione personalizzata](#configurazione-personalizzata)
- [Salta pulizia](#salta-pulizia)
- [Cache delle traduzioni](#cache-delle-traduzioni)
- [Distribuzione come servizi pubblici](#distribuzione-come-servizi-pubblici)
- [Autenticazione e pagina di benvenuto](#autenticazione-e-pagina-di-benvenuto)
- [Supporto per il glossario](#supporto-per-il-glossario)

---

#### Argomenti della riga di comando

Esegui il comando di traduzione nella riga di comando per generare il documento tradotto `example-mono.pdf` e il documento bilingue `example-dual.pdf` nella directory di lavoro corrente. Utilizza Google come servizio di traduzione predefinito. Altri servizi di traduzione supportati possono essere trovati [QUI](https://github.com/PDFMathTranslate/PDFMathTranslate-next/blob/main/docs/ADVANCED.md#services).

<img src="./../images/cmd_light.svg" width="580px"  alt="cmd"/>

Nella seguente tabella, elenchiamo tutte le opzioni avanzate per riferimento:

##### Argomenti

| Opzione                         | Funzione                                                                               | Esempio                                                                                                              |
| ------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| `files`                         | Percorso del file PDF locale                                                          | `pdf2zh ~/local.pdf`                                                                                                 |
| `links`                         | File online                                                                           | `pdf2zh http://arxiv.org/paper.pdf`                                                                                  |
| `--output`                      | Directory di output per i file                                                         | `pdf2zh example.pdf --output /outputpath`                                                                            |
| `--<Services>`                  | Utilizza [**servizio specifico**](./Documentation-of-Translation-Services.md) per la traduzione | `pdf2zh example.pdf --openai`<br>`pdf2zh example.pdf --deepseek`                                                     |
| `--help`, `-h`                  | Mostra il messaggio di aiuto ed esce                                                             | `pdf2zh -h`                                                                                                          |
| `--config-file`                 | Percorso del file di configurazione                                                   | `pdf2zh --config-file /path/to/config/config.toml`                                                                   |
| `--report-interval`             | Intervallo di segnalazione dello stato di avanzamento in secondi                                                    | `pdf2zh example.pdf --report-interval 5`                                                                             |
| `--debug`                       | Utilizza il livello di registrazione debug                                                                | `pdf2zh example.pdf --debug`                                                                                         |
| `--gui`                         | Interagisci con la GUI                                                                      | `pdf2zh --gui`                                                                                                       |
| `--warmup`                      | Scarica e verifica solo gli asset richiesti e poi esce                                     | `pdf2zh example.pdf --warmup`                                                                                        |
| `--generate-offline-assets`     | Genera il pacchetto di risorse offline nella directory specificata                     | `pdf2zh example.pdf --generate-offline-assets /path`                                                                 |
| `--restore-offline-assets`      | Ripristina il pacchetto di risorse offline dalla directory specificata                 | `pdf2zh example.pdf --restore-offline-assets /percorso`                                                               |
| `--version`                     | Mostra la versione e poi esci                                                                 | `pdf2zh --version`                                                                                                   |
| `--pages`                       | Traduzione parziale del documento                                                           | `pdf2zh example.pdf --pages 1,2,1-,-3,3-5`                                                                           |
| `--lang-in`                     | Il codice della lingua di origine                                                            | `pdf2zh example.pdf --lang-in en`                                                                                    |
| `--lang-out`                    | Il codice della lingua di destinazione                                                            | `pdf2zh example.pdf --lang-out zh-CN`                                                                                |
| `--min-text-length`             | Lunghezza minima del testo da tradurre                                                       | `pdf2zh example.pdf --min-text-length 5`                                                                             |
| `--rpc-doclayout`               | Indirizzo host del servizio RPC per l'analisi del layout del documento                 |                                                                                                                      |
| `--qps`                         | Limite QPS per il servizio di traduzione                                               | `pdf2zh example.pdf --qps 200`                                                                                       |
| `--ignore-cache`                | Ignora la cache delle traduzioni                                                       | `pdf2zh example.pdf --ignore-cache`                                                                                  |
| `--custom-system-prompt`        | Prompt personalizzato per la traduzione. Utilizzato per `/no_think` in Qwen 3                   | `pdf2zh example.pdf --custom-system-prompt "/no_think You are a professional, authentic machine translation engine"` |
| `--pool-max-worker`             | Numero massimo di worker per il pool di traduzione. Se non impostato, verrà utilizzato qps come numero di worker | `pdf2zh example.pdf --pool-max-worker 100`                                                                |
| `--no-auto-extract-glossary`    | Disabilita l'estrazione automatica del glossario                                                          | `pdf2zh example.pdf --no-auto-extract-glossary`                                                                      |
| `--primary-font-family`         | Sovrascrive il font primario per il testo tradotto. Opzioni: 'serif' per font serif, 'sans-serif' per font sans-serif, 'script' per font script/corsivi. Se non specificato, utilizza la selezione automatica del font basata sulle proprietà del testo originale. | `pdf2zh example.pdf --primary-font-family serif` |
| `--no-dual`                     | Non generare file PDF bilingue                                                      | `pdf2zh example.pdf --no-dual`                                                                                       |
| `--no-mono`                     | Non generare file PDF monolingue                                                    | `pdf2zh example.pdf --no-mono`                                                                                       |
| `--formular-font-pattern`       | Modello di font per identificare il testo della formula                                                  | `pdf2zh example.pdf --formular-font-pattern "(MS.*)"`                                                                |
| `--formular-char-pattern`       | Modello di caratteri per identificare il testo della formula                                             | `pdf2zh example.pdf --formular-char-pattern "(MS.*)"`                                                                |
| `--split-short-line`            | Forza la divisione di righe brevi in paragrafi diversi                                       | `pdf2zh example.pdf --split-short-line`                                                                              |
| `--short-line-split-factor`     | Fattore di soglia di divisione per righe corte                                         |                                                                                                                      |
| `--skip-clean`                  | Salta il passaggio di pulizia del PDF                                                 | `pdf2zh example.pdf --skip-clean`                                                                                    |
| `--dual-translate-first`        | Nella modalità PDF duale, posiziona prima la pagina tradotta                                          | `pdf2zh example.pdf --dual-translate-first`                                                                                            |
| `--disable-rich-text-translate` | Disabilita la traduzione del testo formattato                                                          | `pdf2zh example.pdf --disable-rich-text-translate`                                                                   |
| `--enhance-compatibility`       | Abilita tutte le opzioni di miglioramento della compatibilità                                           | `pdf2zh example.pdf --enhance-compatibility`                                                                         |
| `--use-alternating-pages-dual`  | Utilizza la modalità pagine alternate per PDF duali                                                | `pdf2zh example.pdf --use-alternating-pages-dual`                                                                    |
| `--watermark-output-mode`       | Modalità di output della filigrana per i file PDF                                       | `pdf2zh example.pdf --watermark-output-mode "NoWaterMark"`                                                           |
| `--max-pages-per-part`          | Numero massimo di pagine per parte per la traduzione divisa                                           | `pdf2zh example.pdf --max-pages-per-part 1`                                                                          |
| `--translate-table-text`        | Tradurre il testo delle tabelle (sperimentale)                                                    | `pdf2zh example.pdf --translate-table-text`                                                                          |
| `--skip-scanned-detection`      | Salta il rilevamento di documenti scansionati                                         | `pdf2zh example.pdf --skip-scanned-detection`                                                                        |
| `--ocr-workaround`              | Forza il testo tradotto a essere nero e aggiunge uno sfondo bianco                     | `pdf2zh example.pdf --ocr-workaround`                                                                                |
| `--auto-enable-ocr-workaround`  | Abilita la soluzione automatica per l'OCR. Se un documento viene rilevato come pesantemente scansionato, questo tenterà di abilitare l'elaborazione OCR e saltare ulteriori rilevamenti di scansione. Consultare la documentazione per i dettagli. (default: False) | `pdf2zh example.pdf --auto-enable-ocr-workaround True`                    |
| `--only-include-translated-page`| Includere solo le pagine tradotte nel PDF di output. Efficace solo quando viene utilizzato --pages. | `pdf2zh example.pdf --pages 1-5 --only-include-translated-page`                                                       |
| `--glossaries`                  | Glossario personalizzato per la traduzione.                                                      | `pdf2zh example.pdf --glossaries "glossary1.csv,glossary2.csv,glossary3.csv"`                                         |
| `--save-auto-extracted-glossary`| salva automaticamente il glossario estratto.                                                | `pdf2zh example.pdf --save-auto-extracted-glossary`                                                                   |


##### Argomenti GUI

| Opzione                         | Funzione                               | Esempio                                         |
| ------------------------------- | -------------------------------------- | ----------------------------------------------- |
| `--share`                       | Abilita la modalità di condivisione    | `pdf2zh --gui --share`                          |
| `--auth-file`                   | Percorso del file di autenticazione    | `pdf2zh --gui --auth-file /path`                |
| `--welcome-page`                | Percorso del file html di benvenuto     | `pdf2zh --gui --welcome-page /path`             |
| `--enabled-services`            | Servizi di traduzione abilitati           | `pdf2zh --gui --enabled-services "Bing,OpenAI"` |
| `--disable-gui-sensitive-input` | Disabilita l'input sensibile della GUI | `pdf2zh --gui --disable-gui-sensitive-input`    |
| `--disable-config-auto-save`    | Disabilita il salvataggio automatico della configurazione | `pdf2zh --gui --disable-config-auto-save`       |
| `--server-port`                 | Porta WebUI                             | `pdf2zh --gui --server-port 7860`               |

[⬆️ Torna su](#toc)

---

#### Traduzione parziale

Utilizzare il parametro `--pages` per tradurre una parte di un documento.

- Se i numeri di pagina sono consecutivi, puoi scriverlo così:

```bash
pdf2zh_next example.pdf --pages 1-3
```

```bash
pdf2zh_next example.pdf --pages 25-
```

> [!TIP]
> `25-` include tutte le pagine successive alla pagina 25. Se il tuo documento ha 100 pagine, questo equivale a `25-100`.
> 
> Allo stesso modo, `-25` include tutte le pagine precedenti alla pagina 25, che equivale a `1-25`.

- Se le pagine non sono consecutive, puoi usare una virgola `,` per separarle.

Ad esempio, se vuoi tradurre la prima e la terza pagina, puoi usare il seguente comando:

```bash
pdf2zh_next example.pdf --pages "1,3"
```

- Se le pagine includono sia intervalli consecutivi che non consecutivi, puoi anche collegarli con una virgola, in questo modo:

```bash
pdf2zh_next example.pdf --pages "1,3,10-20,25-"
```

Questo comando tradurrà la prima pagina, la terza pagina, le pagine da 10 a 20 e tutte le pagine da 25 alla fine.


[⬆️ Torna all'inizio](#toc)

---

#### Specificare le lingue di origine e di destinazione

Vedi [Codici lingua di Google](https://developers.google.com/admin-sdk/directory/v1/languages), [Codici lingua di DeepL](https://developers.deepl.com/docs/resources/supported-languages)

```bash
pdf2zh_next example.pdf --lang-in en -lang-out ja
```

[⬆️ Torna su](#toc)

---

#### Tradurre con eccezioni

Utilizza le espressioni regolari per specificare i caratteri dei formula e i caratteri che devono essere preservati:

```

```bash
pdf2zh_next example.pdf --formular-font-pattern "(CM[^RT].*|MS.*|.*Ital)" --formular-char-pattern "(\(|\||\)|\+|=|\d|[\u0080-\ufaff])"
```

Preserva i caratteri `Latex`, `Mono`, `Code`, `Italic`, `Symbol` e `Math` per impostazione predefinita:

```bash
pdf2zh_next example.pdf --formular-font-pattern "(CM[^R]|MS.M|XY|MT|BL|RM|EU|LA|RS|LINE|LCIRCLE|TeX-|rsfs|txsy|wasy|stmary|.*Mono|.*Code|.*Ital|.*Sym|.*Math)"
```

[⬆️ Torna su](#toc)

---

#### Prompt personalizzato

<!-- Note: System prompt is currently not supported. See [this change](https://github.com/PDFMathTranslate/PDFMathTranslate-next/pull/637). -->

Prompt personalizzato del sistema per la traduzione. Viene principalmente utilizzato per aggiungere l'istruzione '/no_think' di Qwen 3 nel prompt.

```bash
pdf2zh_next example.pdf --custom-system-prompt "/no_think You are a professional and reliable machine translation engine responsible for translating the input text into zh_CN.When translating, strictly follow the instructions below to ensure translation quality and preserve all formatting, tags, and placeholders:"
```

[⬆️ Torna su](#toc)

---

#### Configurazione personalizzata

Esistono diversi modi per modificare e importare il file di configurazione.

> [!NOTE]
> **Gerarchia dei file di configurazione**
>
> Quando si modifica lo stesso parametro utilizzando metodi diversi, il software applicherà le modifiche in base all'ordine di priorità riportato di seguito.
>
> Le modifiche con priorità più alta sovrascriveranno quelle con priorità più bassa.
>
> **cli/gui > env > file di configurazione utente > file di configurazione predefinito**

- Modifica della configurazione tramite **Argomenti della riga di comando**

Nella maggior parte dei casi, puoi passare direttamente le impostazioni desiderate attraverso gli argomenti della riga di comando. Per maggiori informazioni, consulta [Argomenti della riga di comando](#cmd).

Ad esempio, se vuoi abilitare una finestra GUI, puoi usare il seguente comando:

```bash
pdf2zh_next --gui
```

- Modifica della configurazione tramite **Variabili d'ambiente**

È possibile sostituire il `--` negli argomenti della riga di comando con `PDF2ZH_`, collegare i parametri utilizzando `=`, e sostituire `-` con `_` come variabili d'ambiente.

Ad esempio, se si desidera abilitare una finestra GUI, è possibile utilizzare il seguente comando:

```bash
PDF2ZH_GUI=TRUE pdf2zh_next
```

<img src="./../images/ev_light.svg" width="580px"  alt="env"/>

- File di **Configurazione** specificato dall'utente

È possibile specificare un file di configurazione utilizzando l'argomento della riga di comando riportato di seguito:

```bash
pdf2zh_next --config-file '/path/config.toml'
```

Se non sei sicuro del formato del file di configurazione, fai riferimento al file di configurazione predefinito descritto di seguito.

- **File di configurazione predefinito**

Il file di configurazione predefinito si trova in `~/.config/pdf2zh`. 
Si prega di non modificare i file di configurazione nella directory `default`. 
Si consiglia vivamente di fare riferimento al contenuto di questo file di configurazione e utilizzare **Configurazione personalizzata** per implementare il proprio file di configurazione.

> [!TIP]
> - Per impostazione predefinita, pdf2zh 2.0 salva automaticamente la configurazione corrente in `~/.config/pdf2zh/config.v3.toml` ogni volta che si clicca sul pulsante di traduzione nell'interfaccia grafica. Questo file di configurazione verrà caricato automaticamente al prossimo avvio.
> - I file di configurazione nella directory `default` sono generati automaticamente dal programma. È possibile copiarli per modificarli, ma si prega di non modificarli direttamente.
> - I file di configurazione possono includere numeri di versione come "v2", "v3", ecc. Questi sono **numeri di versione del file di configurazione**, **non** il numero di versione di pdf2zh stesso.


[⬆️ Torna su](#toc)

---

#### Salta pulizia

Quando questo parametro è impostato su True, il passaggio di pulizia del PDF verrà saltato, il che può migliorare la compatibilità ed evitare alcuni problemi di elaborazione dei caratteri.

Utilizzo:

```bash
pdf2zh_next example.pdf --skip-clean
```

Oppure utilizzando le variabili d'ambiente:

```bash
PDF2ZH_SKIP_CLEAN=TRUE pdf2zh_next example.pdf
```

> [!TIP]
> Quando `--enhance-compatibility` è abilitato, Salta pulizia viene abilitato automaticamente.

---

#### Cache delle traduzioni

PDFMathTranslate memorizza nella cache i testi tradotti per aumentare la velocità ed evitare chiamate API non necessarie per contenuti identici. È possibile utilizzare l'opzione `--ignore-cache` per ignorare la cache delle traduzioni e forzare una nuova traduzione.

```bash
pdf2zh_next example.pdf --ignore-cache
```

[⬆️ Torna su](#toc)

---

#### Distribuzione come servizi pubblici

Quando si distribuisce un'interfaccia grafica pdf2zh su servizi pubblici, è necessario modificare il file di configurazione come descritto di seguito.

> [!TIP]
> - Quando si distribuisce pubblicamente, sia `disable_gui_sensitive_input` che `disable_config_auto_save` dovrebbero essere abilitati.
> - Separare i diversi servizi disponibili con *virgole inglesi* <kbd>,</kbd> .

Una configurazione utilizzabile è la seguente:

```toml title="config.toml"
[basic]
gui = true

[gui_settings]
enabled_services = "Bing,OpenAI"
disable_gui_sensitive_input = true
disable_config_auto_save = true
```

[⬆️ Torna su](#toc)

---

#### Autenticazione e pagina di benvenuto

Quando si utilizza Autenticazione e pagina di benvenuto per specificare quale utente può utilizzare l'interfaccia web e personalizzare la pagina di login:

esempio auth.txt
Ogni riga contiene due elementi, nome utente e password, separati da una virgola.

```
admin,123456
user1,password1
user2,abc123
guest,guest123
test,test123
```

esempio welcome.html

```html
<!DOCTYPE html>
<html>
<head>
    <title>Simple HTML</title>
</head>
<body>
    <h1>Hello, World!</h1>
    <p>Welcome to my simple HTML page.</p>
</body>
</html>
```

> [!NOTE]
> La pagina di benvenuto funzionerà solo se il file di autenticazione non è vuoto.
> Se il file di autenticazione è vuoto, non ci sarà alcuna autenticazione. :)

Una configurazione utilizzabile è la seguente:

```toml title="config.toml"
[basic]
gui = true

[gui_settings]
auth_file = "/path/to/auth/file"
welcome_page = "/path/to/welcome/html/file"
```

[⬆️ Torna su](#toc)

---

#### Supporto per il glossario

PDFMathTranslate supporta la tabella del glossario. Il file delle tabelle del glossario dovrebbe essere un file `csv`.
Ci sono tre colonne nel file. Ecco un file di glossario demo:

| source | target  | tgt_lng |
|--------|---------|---------|
| AutoML | 自动 ML  | zh-CN   |
| a,a    | a       | zh-CN   |
| "      | "       | zh-CN   |


Per gli utenti della riga di comando:
È possibile utilizzare più file per il glossario. E i diversi file dovrebbero essere separati da `,`.

```

```bash
pdf2zh_next example.pdf --glossaries "glossary1.csv,glossary2.csv,glossary3.csv"
```

Per gli utenti WebUI:

Ora puoi caricare il tuo file di glossario. Dopo aver caricato il file, puoi verificarlo cliccando sul suo nome e il contenuto verrà visualizzato di seguito.

[⬆️ Torna all'inizio](#toc)

<div align="right"> 
<h6><small>Parte del contenuto di questa pagina è stata tradotta da GPT e potrebbe contenere errori.</small></h6>