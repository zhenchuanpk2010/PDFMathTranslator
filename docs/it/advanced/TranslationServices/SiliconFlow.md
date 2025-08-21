# SiliconFlow

## Servizio di traduzione gratuito

[SiliconFlow](https://siliconflow.cn) fornisce un servizio di traduzione gratuito per questo progetto.

Attualmente, il servizio di traduzione gratuito utilizzerà il modello `THUDM/GLM-4-9B-0414`.

### Utilizzo

#### cli

```bash
pdf2zh_next --siliconflowfree example.pdf 
```

#### webui

1. Selezionare "SiliconFlowFree" dall'elenco a discesa "Translation Options" - "Service".
2. Fare clic sul pulsante Translate nella parte inferiore della pagina per avviare la traduzione.
3. Al termine della traduzione, è possibile trovare il file PDF tradotto nella sezione "Translated" nella parte inferiore della pagina.


### Politica sulla privacy

Il contenuto del file verrà inviato al server del maintainer del progetto [@awwaawwa](https://github.com/awwaawwa), e poi inoltrato a SiliconFlow per la traduzione.

I maintainer di questo progetto raccoglieranno solo le informazioni di errore restituite da SiliconFlow per il debug dei servizi correlati. Il contenuto del tuo file non verrà raccolto.

Politica sulla privacy di SiliconFlow: [简体中文](https://docs.siliconflow.cn/cn/legals/privacy-policy)/[English](https://docs.siliconflow.cn/en/legals/privacy-policy)



## Utilizzare altri modelli da SiliconFlow

[SiliconFlow](https://siliconflow.cn) fornisce anche altri modelli per la traduzione.

### Utilizzo

1. Registra un account su [SiliconFlow](https://siliconflow.cn)

2. Crea una chiave API su [SiliconFlow API Key](https://cloud.siliconflow.cn/me/account/ak). Quindi, fai clic sulla chiave per copiarla.

#### cli

```bash
pdf2zh_next --siliconflow --siliconflow-model "Pro/deepseek-ai/DeepSeek-V3" --siliconflow-api-key <your-api-key> example.pdf
```

#### webui

1. "Opzioni di traduzione" - Menu a discesa **"Servizio"**: Selezionare "SiliconFlow"  
2. "Opzioni di traduzione" - **"URL base per l'API SiliconFlow"**: Mantenere il valore predefinito  
3. "Opzioni di traduzione" - **"Modello SiliconFlow da utilizzare"**: Inserire "Pro/deepseek-ai/DeepSeek-V3" o altri modelli  
4. "Opzioni di traduzione" - **"Chiave API per il servizio SiliconFlow"**: Incollare la propria chiave API  
5. Fare clic sul pulsante Traduci in fondo alla pagina per avviare la traduzione  
6. Al termine della traduzione, è possibile trovare il file PDF tradotto nella sezione "Tradotti" in fondo alla pagina.


## Ringraziamenti

Grazie a [SiliconFlow](https://siliconflow.cn) per aver fornito il servizio di traduzione gratuito per questo progetto.

<div align="right"> 
<h6><small>Parte del contenuto di questa pagina è stata tradotta da GPT e potrebbe contenere errori.</small></h6>