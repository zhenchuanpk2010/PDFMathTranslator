Alcune domande vengono poste frequentemente, quindi abbiamo fornito un elenco per gli utenti che incontrano problemi simili.

## È necessaria una GPU?

- **Domanda**:  
Poiché il programma utilizza l'intelligenza artificiale per riconoscere ed estrarre documenti, è necessaria una GPU?

- **Risposta**:  
**La GPU non è necessaria.** Ma se disponi di una GPU, il programma la utilizzerà automaticamente per ottenere prestazioni più elevate.

## Download interrotta?

- **Domanda**:  
Ho riscontrato il seguente errore di interruzione durante il download del modello. Cosa devo fare?

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **Risposta**:  
La rete sta subendo interferenze, si prega di utilizzare un collegamento di rete stabile o provare a bypassare l'intervento della rete.

## Come aggiornare all'ultima versione？

- **Domanda**:  
Voglio utilizzare alcune funzionalità dell'ultima versione, come posso aggiornarla?

- **Risposta**:  
`pip install -U pdf2zh`

## I seguenti file non esistono: example.pdf

- **Problema**:  
Durante l'esecuzione del programma, gli utenti potrebbero ottenere i seguenti output: `The following files do not exist: example.pdf` se il documento non viene trovato.

- **Soluzione**:
  - Apri la riga di comando nella directory dove si trova il file, oppure
  - Inserisci il percorso completo del file direttamente dopo pdf2zh, oppure
  - Usa la modalità interattiva `pdf2zh -i` per trascinare e rilasciare i file direttamente

## Errore SSL e altri problemi di rete

- **Problema**:  
Quando si scaricano i modelli da Hugging Face, gli utenti in Cina potrebbero riscontrare errori di rete. Ad esempio, nei [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55), [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70).

- **Soluzione**:
  - [Bypass GFW](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Usa lo specchio di Hugging Face](https://hf-mirror.com/).
  - [Usa la versione portatile](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [Usa Docker invece](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [Aggiorna i certificati](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), come suggerito in [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55).

## Localhost non è accessibile

Per favore, consulta qui sotto.

## Errore durante l'avvio della GUI utilizzando 0.0.0.0

- **Problema**:  
L'utilizzo di software proxy in modalità globale potrebbe impedire il corretto avvio di Gradio. Ad esempio, nel [problema #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77).

- **Soluzione**:  
Utilizza la modalità regola

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>Parte del contenuto di questa pagina è stata tradotta da GPT e potrebbe contenere errori.</small></h6>