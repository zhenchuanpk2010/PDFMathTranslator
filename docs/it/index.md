<div align="center">

<img src="./docs/images/banner.png" width="320px"  alt="banner"/>

<h2 id="titolo">PDFMathTranslate</h2>

<p>
  <!-- PyPI -->
  <a href="https://pypi.org/project/pdf2zh-next/">
    <img src="https://img.shields.io/pypi/v/pdf2zh-next"></a>
  <a href="https://pepy.tech/projects/pdf2zh-next">
    <img src="https://static.pepy.tech/badge/pdf2zh-next"></a>
  <a href="https://hub.docker.com/repository/docker/awwaawwa/pdfmathtranslate-next/tags">
    <img src="https://img.shields.io/docker/pulls/awwaawwa/pdfmathtranslate-next"></a>
  <a href="https://hellogithub.com/repository/8ec2cfd3ef744762bf531232fa32bc47" target="_blank"><img src="https://api.hellogithub.com/v1/widgets/recommend.svg?rid=8ec2cfd3ef744762bf531232fa32bc47&claim_uid=JQ0yfeBNjaTuqDU&theme=small" alt="In primo piano｜HelloGitHub" /></a>
  <!-- <a href="https://gitcode.com/PDFMathTranslate/PDFMathTranslate-next/overview">
    <img src="https://gitcode.com/PDFMathTranslate/PDFMathTranslate-next/star/badge.svg"></a> -->
  <!-- <a href="https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker">
    <img src="https://img.shields.io/badge/%F0%9F%A4%97-Online%20Demo-FF9E0D"></a> -->
  <!-- <a href="https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate"> -->
    <!-- <img src="https://img.shields.io/badge/ModelScope-Demo-blue"></a> -->
  <!-- <a href="https://github.com/PDFMathTranslate/PDFMathTranslate-next/pulls">
    <img src="https://img.shields.io/badge/contributions-welcome-green"></a> -->
  <a href="https://t.me/+Z9_SgnxmsmA5NzBl">
    <img src="https://img.shields.io/badge/Telegram-2CA5E0?style=flat-squeare&logo=telegram&logoColor=white"></a>
  <!-- License -->
  <a href="./LICENSE">
    <img src="https://img.shields.io/github/license/PDFMathTranslate/PDFMathTranslate-next"></a>
</p>

<a href="https://trendshift.io/repositories/12424" target="_blank"><img src="https://trendshift.io/api/badge/repositories/12424" alt="Byaidu%2FPDFMathTranslate | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>

</div>

Traduzione di articoli scientifici PDF e confronto bilingue.

- 📊 Conserva formule, grafici, indice e annotazioni _([anteprima](#anteprima))_.
- 🌐 Supporta [multiple lingue](https://pdf2zh-next.com/supported_languages.html) e diversi [servizi di traduzione](https://pdf2zh-next.com/advanced/Documentation-of-Translation-Services.html).
- 🤖 Fornisce [strumento da riga di comando](https://pdf2zh-next.com/getting-started/USAGE_commandline.html), [interfaccia utente interattiva](https://pdf2zh-next.com/getting-started/USAGE_webui.html) e [Docker](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html)

Sentiti libero di fornire feedback su [GitHub Issues](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues) o [Telegram Group](https://t.me/+Z9_SgnxmsmA5NzBl).

Per dettagli su come contribuire, consulta la [Guida al Contributo](https://pdf2zh-next.com/community/Contribution-Guide.html).

<h2 id="aggiornamenti">Aggiornamenti</h2>

- [4 giu. 2025] Il progetto è stato rinominato e spostato su [PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next) (da [@awwaawwa](https://github.com/awwaawwa))
- [3 mar. 2025] Supporto sperimentale per il nuovo backend [BabelDOC](https://github.com/funstory-ai/BabelDOC) WebUI aggiunto come opzione sperimentale (da [@awwaawwa](https://github.com/awwaawwa))
- [22 feb. 2025] Miglioramento del CI per i rilasci e pacchettizzazione ottimizzata dell'eseguibile windows-amd64 (da [@awwaawwa](https://github.com/awwaawwa))
- [24 dic. 2024] Il traduttore ora supporta modelli locali su [Xinference](https://github.com/xorbitsai/inference) _(da [@imClumsyPanda](https://github.com/imClumsyPanda))_
- [19 dic. 2024] Ora sono supportati documenti non-PDF/A utilizzando `-cp` _(da [@reycn](https://github.com/reycn))_
- [13 dic. 2024] Supporto aggiuntivo per il backend _(da [@YadominJinta](https://github.com/YadominJinta))_
- [10 dic. 2024] Il traduttore ora supporta i modelli OpenAI su Azure _(da [@yidasanqian](https://github.com/yidasanqian))_

<h2 id="anteprima">Anteprima</h2>

<div align="center">
<!-- <img src="./docs/images/preview.gif" width="80%"  alt="preview"/> -->
<img src="https://s.immersivetranslate.com/assets/r2-uploads/images/babeldoc-preview.png" width="80%"/>
</div>

<h2 id="demo">Servizio Online 🌟</h2>

> [!NOTE]
>
> pdf2zh 2.0 attualmente non fornisce una demo online

Puoi provare la nostra applicazione utilizzando una delle seguenti demo:

- [v1.x Servizio pubblico gratuito](https://pdf2zh.com/) online senza installazione _(consigliato)_.
- [Immersive Translate - BabelDOC](https://app.immersivetranslate.com/babel-doc/) 1000 pagine gratuite al mese. _(consigliato)_
<!-- - [Demo hosted on HuggingFace](https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker)
- [Demo hosted on ModelScope](https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate) without installation. -->

Nota che le risorse di calcolo della demo sono limitate, quindi evita di abusarne.

<h2 id="install">Installazione e Utilizzo</h2>

### Installazione

1. [**Windows EXE**](https://pdf2zh-next.com/getting-started/INSTALLATION_winexe.html) <small>Consigliato per Windows</small>
2. [**Docker**](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html) <small>Consigliato per Linux</small>
3. [**uv** (un gestore di pacchetti Python)](https://pdf2zh-next.com/getting-started/INSTALLATION_uv.html) <small>Consigliato per macOS</small>

---

### Utilizzo

1. [Utilizzo di **WebUI**](https://pdf2zh-next.com/getting-started/USAGE_webui.html)
2. [Utilizzo di **Zotero Plugin**](https://github.com/guaguastandup/zotero-pdf2zh) (Programma di terze parti)
3. [Utilizzo di **Commandline**](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)

Per diversi casi d'uso, forniamo metodi distinti per utilizzare il nostro programma. Consulta [questa pagina](./getting-started/getting-started.md) per maggiori informazioni.

<h2 id="usage">Opzioni avanzate</h2>

Per spiegazioni dettagliate, si prega di fare riferimento al nostro documento su [Utilizzo avanzato](https://pdf2zh-next.com/advanced/advanced.html) per un elenco completo di ciascuna opzione.

<h2 id="downstream">Sviluppo secondario (APIs)</h2>

> [!NOTE]
>
> Attualmente, non è fornita alcuna documentazione pertinente. Sarà integrata in seguito. Si prega di attendere con pazienza.


<!-- For downstream applications, please refer to our document about [API Details](./docs/APIS.md) for futher information about:

- [Python API](./docs/APIS.md#api-python), how to use the program in other Python programs
- [HTTP API](./docs/APIS.md#api-http), how to communicate with a server with the program installed -->

<h2 id="codice-lingua">Codice lingua</h2>

Se non sai quale codice utilizzare per tradurre nella lingua di cui hai bisogno, consulta [questa documentazione](https://pdf2zh-next.com/advanced/Language-Codes.html)

<!-- 
<h2 id="todo">TODOs</h2>

- [ ] Parse layout with DocLayNet based models, [PaddleX](https://github.com/PaddlePaddle/PaddleX/blob/17cc27ac3842e7880ca4aad92358d3ef8555429a/paddlex/repo_apis/PaddleDetection_api/object_det/official_categories.py#L81), [PaperMage](https://github.com/allenai/papermage/blob/9cd4bb48cbedab45d0f7a455711438f1632abebe/README.md?plain=1#L102), [SAM2](https://github.com/facebookresearch/sam2)

- [ ] Fix page rotation, table of contents, format of lists

- [ ] Fix pixel formula in old papers

- [ ] Async retry except KeyboardInterrupt

- [ ] Knuth–Plass algorithm for western languages

- [ ] Support non-PDF/A files

- [ ] Plugins of [Zotero](https://github.com/zotero/zotero) and [Obsidian](https://github.com/obsidianmd/obsidian-releases) -->

<h2 id="ringraziamenti">Ringraziamenti</h2>

- [Immersive Translation](https://immersivetranslate.com) sponsorizza codici di riscatto mensili per l'abbonamento Pro per i contributori attivi di questo progetto, vedi dettagli su: [CONTRIBUTOR_REWARD.md](https://github.com/funstory-ai/BabelDOC/blob/main/docs/CONTRIBUTOR_REWARD.md)

- [SiliconFlow](https://siliconflow.cn) fornisce un servizio di traduzione gratuito per questo progetto, alimentato da modelli linguistici di grandi dimensioni (LLM).

- Versione 1.x: [Byaidu/PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate)


- backend: [BabelDOC](https://github.com/funstory-ai/BabelDOC)

- Libreria PDF: [PyMuPDF](https://github.com/pymupdf/PyMuPDF)

- Analisi PDF: [Pdfminer.six](https://github.com/pdfminer/pdfminer.six)

- Anteprima PDF: [Gradio PDF](https://github.com/freddyaboulton/gradio-pdf)

- Analisi del layout: [DocLayout-YOLO](https://github.com/opendatalab/DocLayout-YOLO)

- Standard PDF: [PDF Explained](https://zxyle.github.io/PDF-Explained/), [PDF Cheat Sheets](https://pdfa.org/resource/pdf-cheat-sheets/)

- Carattere multilingue: vedi [BabelDOC-Assets](https://github.com/funstory-ai/BabelDOC-Assets)

- [Asynchronize](https://github.com/multimeric/Asynchronize/tree/master?tab=readme-ov-file)

- [Registrazione avanzata con multiprocessing](https://github.com/SebastianGrans/Rich-multiprocess-logging/tree/main)

- Documentazione i18n utilizzando Weblate: [Weblate](https://weblate.org/)

<h2 id="conduct">Prima di inviare il tuo codice</h2>

Accogliamo con favore la partecipazione attiva dei contributori per migliorare pdf2zh. Prima di essere pronto a inviare il tuo codice, consulta il nostro [Codice di Condotta](https://pdf2zh-next.com/community/CODE_OF_CONDUCT.html) e la [Guida al Contributo](https://pdf2zh-next.com/community/Contribution-Guide.html).

<h2 id="contrib">Contributori</h2>

<a href="https://github.com/PDFMathTranslate/PDFMathTranslate-next/graphs/contributors">
  <img src="https://opencollective.com/PDFMathTranslate/contributors.svg?width=890&button=false" />
</a>

![Alt](https://repobeats.axiom.co/api/embed/45529651750579e099960950f757449a410477ad.svg "Repobeats analytics image")

<h2 id="star_hist">Storia delle Stelle</h2>

<a href="https://star-history.com/#PDFMathTranslate/PDFMathTranslate-next&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date" />
   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date"/>
 <p align="center">
  <a href="https://pdf2zh-next.com">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://pdf2zh-next.com/logo_dark.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://pdf2zh-next.com/logo_light.svg">
      <img alt="pdf2zh" src="https://pdf2zh-next.com/logo_light.svg" width="300">
    </picture>
  </a>
</p>

<p align="center">
  <a href="https://pdf2zh-next.com">Home</a> •
  <a href="https://pdf2zh-next.com/getting-started">Getting Start</a> •
  <a href="https://pdf2zh-next.com/getting-started/INSTALLATION.html">Installation</a> •
  <a href="https://pdf2zh-next.com/getting-started/USAGE_cli.html">Command Line</a> •
  <a href="https://pdf2zh-next.com/getting-started/USAGE_webui.html">Usage</a> •
  <a href="https://pdf2zh-next.com/getting-started/LANGUAGE_CODE.html">Language Code</a> •
  <a href="https://pdf2zh-next.com/getting-started/DOCS.html">Documentation of Translation Services</a>
</p>

<p align="center">
  <a href="https://pdf2zh-next.com/getting-started">Getting Started</a> •
  <a href="https://pdf2zh-next.com/getting-started/ADVANCED.html">Advanced</a> •
  <a href="https://pdf2zh-next.com/getting-started/LANGUAGE_CODE.html">Supported Languages</a> •
  <a href="https://pdf2zh-next.com/community">Community</a> •
  <a href="https://pdf2zh-next.com/faq">FAQ</a>
</p>

---

### Installation

### Usage

---

<p align="center">
  <a href="https://github.com/PDFMathTranslate/pdf2zh">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://pdf2zh-next.com/logo_dark.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://pdf2zh-next.com/logo_light.svg">
      <img alt="pdf2zh" src="https://pdf2zh-next.com/logo_light.svg" width="300">
    </picture>
  </a>
</p>

<p align="center">
  <a href="https://pdf2zh-next.com">Home</a> •
  <a href="https://pdf2zh-next.com/getting-started">Iniziare</a> •
  <a href="https://pdf2zh-next.com/getting-started/INSTALLATION.html">Installazione</a> •
  <a href="https://pdf2zh-next.com/getting-started/USAGE_cli.html">Riga di comando</a> •
  <a href="https://pdf2zh-next.com/getting-started/USAGE_webui.html">Utilizzo</a> •
  <a href="https://pdf2zh-next.com/getting-started/LANGUAGE_CODE.html">Codice lingua</a> •
  <a href="https://pdf2zh-next.com/getting-started/DOCS.html">Documentazione dei servizi di traduzione</a>
</p>

<p align="center">
  <a href="https://pdf2zh-next.com/getting-started">Iniziare</a> •
  <a href="https://pdf2zh-next.com/getting-started/ADVANCED.html">Opzioni avanzate</a> •
  <a href="https://pdf2zh-next.com/getting-started/LANGUAGE_CODE.html">Lingue supportate</a> •
  <a href="https://pdf2zh-next.com/community">Comunità</a> •
  <a href="https://pdf2zh-next.com/faq">Domande frequenti</a>
</p>

---

### Installazione

### Utilizzo

---

<div align="right"> 
<h6><small>Parte del contenuto di questa pagina è stata tradotta da GPT e potrebbe contenere errori.</small></h6>