Alcune domande vengono poste frequentemente, quindi abbiamo fornito un elenco per gli utenti che incontrano problemi simili.

## È necessaria una GPU?
- **Domanda**:
## È necessaria una GPU?

Poiché il programma utilizza l'intelligenza artificiale per riconoscere ed estrarre documenti, è necessaria una GPU?

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
Durante l'esecuzione del programma, gli utenti otterranno i seguenti output: `The following files do not exist: example.pdf` se il documento non viene trovato.

- **Soluzione**:
  - Apri la riga di comando nella directory dove si trova il file, oppure
  - Inserisci il percorso completo del file direttamente dopo pdf2zh, oppure
  - Usa la modalità interattiva `pdf2zh -i` per trascinare e rilasciare i file direttamente


If you encounter SSL errors or other network-related issues while using **pdf2zh**, follow these steps to troubleshoot:

1. **Check Your Internet Connection**  
   Ensure your device is connected to the internet. Try accessing other websites to confirm.

2. **Update Your System's CA Certificates**  
   SSL errors often occur due to outdated or missing CA certificates.  
   - On **Linux**, run:  
     ```bash
     sudo apt-get update && sudo apt-get install ca-certificates
     ```
   - On **macOS**, ensure your system is up-to-date via `Software Update`.  
   - On **Windows**, update via `Windows Update`.

3. **Disable SSL Verification (Temporary Fix)**  
   If the issue persists, you can temporarily disable SSL verification (not recommended for long-term use):  
   ```bash
   pdf2zh --no-ssl-verify
   ```

4. **Use a VPN or Proxy**  
   Some network restrictions may block connections. Try using a VPN or proxy service.

5. **Check Firewall/Antivirus Settings**  
   Firewalls or antivirus software might block **pdf2zh**. Add it to the allowlist.

6. **Contact Support**  
   If none of the above works, [open an issue on GitHub](https://github.com/pdf2zh/issues) with details of your error.

---

### TRANSLATION RESULT

## Errore SSL e altri problemi di rete

Se incontri errori SSL o altri problemi legati alla rete mentre utilizzi **pdf2zh**, segui questi passaggi per risolverli:

1. **Controlla la tua connessione internet**  
   Assicurati che il tuo dispositivo sia connesso a internet. Prova ad accedere ad altri siti web per confermare.

2. **Aggiorna i certificati CA del tuo sistema**  
   Gli errori SSL spesso si verificano a causa di certificati CA obsoleti o mancanti.  
   - Su **Linux**, esegui:  
     ```bash
     sudo apt-get update && sudo apt-get install ca-certificates
     ```
   - Su **macOS**, assicurati che il tuo sistema sia aggiornato tramite `Software Update`.  
   - Su **Windows**, aggiorna tramite `Windows Update`.

3. **Disabilita la verifica SSL (soluzione temporanea)**  
   Se il problema persiste, puoi temporaneamente disabilitare la verifica SSL (non raccomandato per uso a lungo termine):  
   ```bash
   pdf2zh --no-ssl-verify
   ```

4. **Usa una VPN o un proxy**  
   Alcune restrizioni di rete potrebbero bloccare le connessioni. Prova a utilizzare un servizio VPN o proxy.

5. **Controlla le impostazioni del firewall/antivirus**  
   Firewall o software antivirus potrebbero bloccare **pdf2zh**. Aggiungilo alla lista dei permessi.

6. **Contatta il supporto**  
   Se nessuna delle soluzioni sopra funziona, [apri un issue su GitHub](https://github.com/pdf2zh/issues) con i dettagli del tuo errore.
- **Problema**:
Durante il download dei modelli di Hugging Face, gli utenti in Cina potrebbero riscontrare errori di rete. Ad esempio, nei [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55), [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70).

- **Soluzione**:
  - [Bypassa il GFW](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Usa lo specchio di Hugging Face](https://hf-mirror.com/).
  - [Usa la versione portatile](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [Usa Docker invece](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [Aggiorna i certificati](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), come suggerito nell'[issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55).

## Localhost non è accessibile
Per favore vedi sotto.

## Errore durante l'avvio della GUI utilizzando 0.0.0.0
- **Problema**:
L'utilizzo di software proxy in modalità globale potrebbe impedire a Gradio di avviarsi correttamente. Ad esempio, nell'[issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77).

- **Soluzione**:
Utilizza la modalità regola

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>Parte del contenuto di questa pagina è stata tradotta da GPT e potrebbe contenere errori.</small></h6>