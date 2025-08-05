Alcune domande vengono poste frequentemente, quindi abbiamo fornito un elenco per gli utenti che incontrano problemi simili.

## È necessaria una GPU?
- **Domanda**:
## È necessaria una GPU?

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
Durante l'esecuzione del programma, gli utenti otterranno i seguenti output: `The following files do not exist: example.pdf` se il documento non viene trovato.

- **Soluzione**:
  - Apri la riga di comando nella directory dove si trova il file, oppure
  - Inserisci il percorso completo del file direttamente dopo pdf2zh, oppure
  - Usa la modalità interattiva `pdf2zh -i` per trascinare e rilasciare i file direttamente


## Errore SSL e Altri Problemi di Rete
- **Problema**:
在下载 Hugging Face 模型时，中国用户可能会遇到网络错误。例如，在[issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55)、[#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70)中提到的案例。

- **Soluzione**:
  - [Bypass GFW](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Usa Hugging Face Mirror](https://hf-mirror.com/).
  - [Usa la versione Portable](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [Usa Docker invece](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [Aggiorna i Certificati](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), come suggerito in [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55).

# Localhost non è accessibile

Se stai utilizzando pdf2zh su un server remoto e non riesci ad accedere all'interfaccia utente web tramite `localhost`, potresti dover configurare il server per consentire l'accesso esterno.  

### Soluzioni:  

1. **Specifica un indirizzo IP pubblico o `0.0.0.0`**  
   - Modifica il comando di avvio per includere `--host 0.0.0.0`:  
     ```bash
     pdf2zh --host 0.0.0.0
     ```
   - Questo renderà il servizio accessibile da qualsiasi indirizzo IP sulla rete.  

2. **Configura le regole del firewall**  
   - Assicurati che la porta predefinita (`5000`) sia aperta nel firewall del server.  
   - Esempio per `ufw` (Ubuntu):  
     ```bash
     sudo ufw allow 5000
     ```

3. **Usa un proxy inverso (opzionale)**  
   - Per maggiore sicurezza, configura Nginx o Apache come proxy inverso.  

4. **Verifica l'accessibilità**  
   - Dopo aver applicato le modifiche, accedi all'interfaccia tramite:  
     ```
     http://<SERVER_IP>:5000
     ```

Per ulteriori dettagli, consulta la sezione [Utilizzo](#utilizzo) o la documentazione del tuo server.  

---
Per favore vedi sotto.

# Errore durante l'avvio della GUI utilizzando 0.0.0.0
- **Problema**:
L'utilizzo di software proxy in modalità globale potrebbe impedire il corretto avvio di Gradio. Ad esempio, nel [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77).

- **Soluzione**:
Utilizza la modalità regola

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>Parte del contenuto di questa pagina è stata tradotta da GPT e potrebbe contenere errori.</small></h6>