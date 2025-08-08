# Contribuire al progetto

> [!CAUTION]
>
> Gli attuali responsabili del progetto stanno ricercando l'internazionalizzazione automatizzata della documentazione. Pertanto, qualsiasi PR relativa all'internazionalizzazione/traduzione della documentazione NON sarà accettata!
>
> Si prega di NON inviare PR relative all'internazionalizzazione/traduzione della documentazione!

Grazie per il tuo interesse in questo progetto! Prima di iniziare a contribuire, ti preghiamo di dedicare un po' di tempo a leggere le seguenti linee guida per assicurarti che il tuo contributo possa essere accettato senza problemi.

## Tipi di Contributi Non Accettati

1. Documentazione internazionalizzazione/traduzione
2. Contributi relativi all'infrastruttura core, come HTTP API, ecc.
3. Issue contrassegnate esplicitamente come "No help needed" (incluse le issue nei repository [Byaidu/PDFMathTranslate](Byaidu/PDFMathTranslate) e [PDFMathTranslate/PDFMathTranslate-next](PDFMathTranslate/PDFMathTranslate-next)).
4. Altri contributi ritenuti inappropriati dai maintainer.
5. Contribuire alla documentazione, ma modificando la documentazione in lingue diverse dall'inglese.
6. PR che richiedono la modifica di file PDF.

Per favore NON inviare PR relativi ai tipi sopra menzionati.

> [!NOTE]
>
> Se vuoi contribuire alla documentazione, **modifica solo la versione inglese della documentazione**. Le altre versioni linguistiche sono tradotte dai contributori stessi.

## Processo di Contribuzione

1. Forka questo repository e clonalo localmente.
2. Crea un nuovo branch: `git checkout -b feature/<feature-name>`.
3. Sviluppa e assicurati che il tuo codice soddisfi i requisiti.
4. Esegui il commit del tuo codice:
   ```bash
   git add .
   git commit -m "<semantic commit message>"
   ```
5. Esegui il push sul tuo repository: `git push origin feature/<feature-name>`.
6. Crea una PR su GitHub, fornisci una descrizione dettagliata e richiedi una revisione da [@awwaawwa](https://github.com/awwaawwa).
7. Assicurati che tutti i controlli automatizzati siano superati.

> [!TIP]
>
> Non è necessario attendere che lo sviluppo sia completamente terminato per creare una PR. Crearne una in anticipo ci permette di esaminare la tua implementazione e fornire suggerimenti.
>
> Se hai domande sul codice sorgente o su questioni correlate, contatta il maintainer all'indirizzo aw@funstory.ai.
>
> I file delle risorse per la versione 2.0 sono condivisi con [BabelDOC](https://github.com/funstory-ai/BabelDOC). Il codice per scaricare le risorse correlate si trova in BabelDOC. Se desideri aggiungere nuovi file di risorse, contatta il maintainer di BabelDOC all'indirizzo aw@funstory.ai.

## Requisiti di base

<h4 id="sop">1. Flusso di lavoro</h4>

   - Si prega di effettuare il fork dal branch `main` e sviluppare sul proprio branch forkato.
   - Quando si invia una Pull Request (PR), fornire una descrizione dettagliata delle modifiche apportate.
   - Se la PR non supera i controlli automatizzati (indicati da `checks failed` e una croce rossa), si prega di rivedere i corrispondenti `details` e modificare l'invio per garantire che la nuova PR superi tutti i controlli.


<h4 id="dev&test">2. Sviluppo e Test</h4>

   - Utilizzare il comando `pip install -e .` per sviluppo e test.


<h4 id="formato">3. Formattazione del Codice</h4>

   - Configura lo strumento `pre-commit` e abilita `black` e `flake8` per la formattazione del codice.


<h4 id="requpdate">4. Aggiornamenti delle dipendenze</h4>

   - Se introduci nuove dipendenze, aggiorna tempestivamente l'elenco delle dipendenze nel file `pyproject.toml`.


<h4 id="docupdate">5. Aggiornamenti della documentazione</h4>

   - Se aggiungi nuove opzioni da riga di comando, aggiorna l'elenco delle opzioni da riga di comando in tutte le versioni linguistiche del file `README.md` di conseguenza.


<h4 id="commitmsg">6. Messaggi di Commit</h4>

   - Utilizzare [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), ad esempio: `feat(translator): add openai`.


<h4 id="codestyle">7. Stile di Codifica</h4>

   - Assicurati che il codice inviato rispetti gli standard di base dello stile di codifica.
   - Utilizza snake_case o camelCase per la denominazione delle variabili.


<h4 id="doctypo">8. Formattazione della Documentazione</h4>

   - Per la formattazione di `README.md`, seguire le [Linee guida per la scrittura in cinese](https://github.com/sparanoid/chinese-copywriting-guidelines).
   - Assicurarsi che la documentazione in inglese e cinese sia sempre aggiornata; gli aggiornamenti della documentazione in altre lingue sono facoltativi.

## Aggiunta di un motore di traduzione

1. Aggiungi una nuova classe di configurazione del traduttore nel file `pdf2zh/config/translate_engine_model.py`.
2. Aggiungi un'istanza della nuova classe di configurazione del traduttore all'alias di tipo `TRANSLATION_ENGINE_SETTING_TYPE` nello stesso file.
3. Aggiungi la nuova classe di implementazione del traduttore nella cartella `pdf2zh/translator/translator_impl`.

> [!NOTE]
>
> Questo progetto non intende supportare alcun motore di traduzione con un RPS (richieste al secondo) inferiore a 4. Si prega di non inviare supporto per tali motori.

## Struttura del progetto

- **config folder**: Sistema di configurazione.
- **translator folder**: Implementazioni relative al traduttore.
- **gui.py**: Fornisce l'interfaccia GUI.
- **const.py**: Alcune costanti.
- **main.py**: Fornisce lo strumento da riga di comando.
- **high_level.py**: Interfacce di alto livello basate su BabelDOC.
- **http_api.py**: Fornisce API HTTP (non avviato).

## Contattaci

Se hai domande, invia feedback tramite Issue o unisciti al nostro gruppo Telegram. Grazie per il tuo contributo!

> [!TIP]
>
> [Immersive Translate](https://immersivetranslate.com) sponsorizza codici mensili di abbonamento Pro per i contributori attivi a questo progetto. Per i dettagli, consultare: [BabelDOC/PDFMathTranslate Regole di ricompensa per i contributori](https://funstory-ai.github.io/BabelDOC/CONTRIBUTOR_REWARD/)

<div align="right"> 
<h6><small>Parte del contenuto di questa pagina è stata tradotta da GPT e potrebbe contenere errori.</small></h6>