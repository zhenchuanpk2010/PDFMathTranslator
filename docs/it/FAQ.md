Alcune domande vengono poste frequentemente, quindi abbiamo fornito un elenco per gli utenti che incontrano problemi simili.

## È necessaria una GPU?
- **Domanda**:
Il programma utilizza l'intelligenza artificiale per riconoscere ed estrarre documenti, è necessaria una GPU?

- **Risposta**:
**Non è necessaria una GPU.** Ma se hai una GPU, il programma la utilizzerà automaticamente per prestazioni più elevate.

## Download interrotta?
- **Domanda**:
Ho riscontrato il seguente errore di interruzione durante il download del modello. Cosa devo fare?

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **Risposta**:
La rete sta subendo interferenze, utilizza un collegamento di rete stabile o prova a bypassare l'intervento della rete.

## Come aggiornare all'ultima versione?
- **Domanda**:
Voglio utilizzare alcune funzionalità dell'ultima versione, come posso aggiornarla?

- **Risposta**:
`pip install -U pdf2zh`


## I seguenti file non esistono: example.pdf
- **Problema**:
Durante l'esecuzione del programma, gli utenti otterranno i seguenti output: `The following files do not exist: example.pdf` se il documento non è stato trovato.

- **Soluzione**:
  - Apri la riga di comando nella directory in cui si trova il file, oppure
  - Inserisci il percorso completo del file direttamente dopo pdf2zh, oppure
  - Usa la modalità interattiva `pdf2zh -i` per trascinare e rilasciare i file direttamente


## Errore SSL e altri problemi di rete

Se riscontri errori SSL o altri problemi di rete durante l'utilizzo di `pdf2zh`, segui questi passaggi per risolverli:

1. **Verifica la connessione Internet**:
   - Assicurati che il tuo dispositivo sia connesso a Internet.
   - Prova ad accedere ad altri siti web per verificare la connessione.

2. **Aggiorna i certificati SSL**:
   - Su Windows, esegui `certmgr.msc` e aggiorna i certificati.
   - Su macOS/Linux, esegui `sudo update-ca-certificates`.

3. **Disabilita temporaneamente il firewall/antivirus**:
   - Alcuni firewall o software antivirus potrebbero bloccare la connessione. Prova a disabilitarli temporaneamente.

4. **Usa una VPN o cambia rete**:
   - Prova a connetterti tramite una VPN o cambia rete (ad esempio, da Wi-Fi a dati mobili).

5. **Controlla la data e l'ora del sistema**:
   - Un'ora o data errata può causare errori SSL. Assicurati che siano corrette.

Se il problema persiste, contatta il supporto tecnico fornendo i dettagli dell'errore.
- **Problema**:
Durante il download dei modelli di Hugging Face, gli utenti in Cina potrebbero riscontrare errori di rete. Ad esempio, nei [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55), [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70).

- **Soluzione**:
  - [Bypass GFW](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Usa Hugging Face Mirror](https://hf-mirror.com/).
  - [Usa la versione portatile](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [Usa Docker invece](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [Aggiorna i certificati](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), come suggerito nell'[issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55).

## Localhost non è accessibile
Per favore, vedi sotto.

## Errore durante l'avvio della GUI utilizzando 0.0.0.0
- **Problema**:
L'utilizzo di software proxy in modalità globale potrebbe impedire il corretto avvio di Gradio. Ad esempio, nel [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77).

- **Soluzione**:
Modalità di utilizzo delle regole

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>Parte del contenuto di questa pagina è stata tradotta da GPT e potrebbe contenere errori.</small></h6>