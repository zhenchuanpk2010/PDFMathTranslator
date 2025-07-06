Alcune domande vengono poste frequentemente, quindi abbiamo fornito un elenco per gli utenti che incontrano problemi simili.

## È necessaria una GPU?
- **Domanda**:
Poiché il programma utilizza l'intelligenza artificiale per riconoscere ed estrarre documenti, è necessaria una GPU?


- **Risposta**:  
```
**Non è necessaria una GPU.** Ma se hai una GPU, il programma la utilizzerà automaticamente per prestazioni più elevate.

## Download interrotto?
- **Domanda**:
Ho riscontrato il seguente errore di interruzione durante il download del modello. Cosa devo fare?

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)


- **Risposta**:  
```
La rete sta subendo interferenze, utilizza un collegamento di rete stabile o prova a bypassare l'intervento della rete.

## Come aggiornare all'ultima versione?
- **Domanda**:
Voglio utilizzare alcune funzionalità dell'ultima versione, come posso aggiornarla?


- **Risposta**:  
```
`pip install -U pdf2zh`


## I seguenti file non esistono: example.pdf
- **Problema**:
Durante l'esecuzione del programma, gli utenti otterranno il seguente output: `I seguenti file non esistono: example.pdf` se il documento non viene trovato.

- **Soluzione**:
  - Aprire la riga di comando nella directory dove si trova il file, oppure
  - Inserire il percorso completo del file direttamente dopo pdf2zh, oppure
  - Utilizzare la modalità interattiva `pdf2zh -i` per trascinare e rilasciare i file direttamente


## Errori SSL e Altri Problemi di Rete
- **Problema**:
Durante il download dei modelli di hugging face, gli utenti in Cina potrebbero riscontrare errori di rete. Ad esempio, nei [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55), [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70).

- **Soluzione**:
  - [Bypassa GFW](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Usa Hugging Face Mirror](https://hf-mirror.com/).
  - [Usa la versione Portable](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [Usa Docker invece](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [Aggiorna i Certificati](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), come suggerito in [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55).

## Localhost non è accessibile
Si prega di vedere sotto.

## Errore durante l'avvio della GUI utilizzando 0.0.0.0
- **Problema**:
L'utilizzo di software proxy in modalità globale potrebbe impedire il corretto avvio di Gradio. Ad esempio, nel [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77).

- **Soluzione**:
Utilizzare la modalità regola

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>Parte del contenuto di questa pagina è stata tradotta da GPT e potrebbe contenere errori.</small></h6>