<div align="center">

<img src="./docs/images/banner.png" width="320px"  alt="banner"/>

<h2 id="titel">PDFMathTranslate</h2>

<p>
  <!-- PyPI -->
  <a href="https://pypi.org/project/pdf2zh-next/">
    <img src="https://img.shields.io/pypi/v/pdf2zh-next"></a>
  <a href="https://pepy.tech/projects/pdf2zh-next">
    <img src="https://static.pepy.tech/badge/pdf2zh-next"></a>
  <a href="https://hub.docker.com/repository/docker/awwaawwa/pdfmathtranslate-next/tags">
    <img src="https://img.shields.io/docker/pulls/awwaawwa/pdfmathtranslate-next"></a>
  <a href="https://hellogithub.com/repository/8ec2cfd3ef744762bf531232fa32bc47" target="_blank"><img src="https://api.hellogithub.com/v1/widgets/recommend.svg?rid=8ec2cfd3ef744762bf531232fa32bc47&claim_uid=JQ0yfeBNjaTuqDU&theme=small" alt="Featured｜HelloGitHub" /></a>
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

Übersetzung wissenschaftlicher PDF-Papiere und bilingualer Vergleich.

- 📊 Erhalten Sie Formeln, Diagramme, Inhaltsverzeichnisse und Anmerkungen _([Vorschau](#vorschau))_.
- 🌐 Unterstützt [mehrere Sprachen](https://pdf2zh-next.com/supported_languages.html) und verschiedene [Übersetzungsdienste](https://pdf2zh-next.com/advanced/Documentation-of-Translation-Services.html).
- 🤖 Bietet [Kommandozeilen-Tool](https://pdf2zh-next.com/getting-started/USAGE_commandline.html), [interaktive Benutzeroberfläche](https://pdf2zh-next.com/getting-started/USAGE_webui.html) und [Docker](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html)

Gerne können Sie Feedback in den [GitHub Issues](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues) oder der [Telegram Group](https://t.me/+Z9_SgnxmsmA5NzBl) geben.

Weitere Details zur Mitwirkung finden Sie im [Contribution Guide](https://pdf2zh-next.com/community/Contribution-Guide.html).

<h2 id="updates">Aktualisierungen</h2>

- [4. Juni 2025] Das Projekt wurde umbenannt und zu [PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next) verschoben (von [@awwaawwa](https://github.com/awwaawwa))
- [3. März 2025] Experimentelle Unterstützung für das neue Backend [BabelDOC](https://github.com/funstory-ai/BabelDOC) WebUI als experimentelle Option hinzugefügt (von [@awwaawwa](https://github.com/awwaawwa))
- [22. Februar 2025] Verbesserte Release-CI und gut verpackte Windows-amd64-Exe (von [@awwaawwa](https://github.com/awwaawwa))
- [24. Dezember 2024] Der Übersetzer unterstützt nun lokale Modelle auf [Xinference](https://github.com/xorbitsai/inference) _(von [@imClumsyPanda](https://github.com/imClumsyPanda))_
- [19. Dezember 2024] Nicht-PDF/A-Dokumente werden nun mit `-cp` unterstützt _(von [@reycn](https://github.com/reycn))_
- [13. Dezember 2024] Zusätzliche Unterstützung für Backend von _(von [@YadominJinta](https://github.com/YadominJinta))_
- [10. Dezember 2024] Der Übersetzer unterstützt nun OpenAI-Modelle auf Azure _(von [@yidasanqian](https://github.com/yidasanqian))_

<h2 id="vorschau">Vorschau</h2>

<div align="center">
<!-- <img src="./docs/images/preview.gif" width="80%"  alt="preview"/> -->
<img src="https://s.immersivetranslate.com/assets/r2-uploads/images/babeldoc-preview.png" width="80%"/>
</div>

<h2 id="demo">Online-Service 🌟</h2>

> [!NOTE]
>
> pdf2zh 2.0 bietet derzeit keine Online-Demo an

Sie können unsere Anwendung mit einer der folgenden Demos ausprobieren:

- [v1.x Öffentlicher kostenloser Dienst](https://pdf2zh.com/) online ohne Installation _(empfohlen)_.
- [Immersive Translate - BabelDOC](https://app.immersivetranslate.com/babel-doc/) 1000 kostenlose Seiten pro Monat. _(empfohlen)_
<!-- - [Demo hosted on HuggingFace](https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker)
- [Demo hosted on ModelScope](https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate) without installation. -->

[!NOTE]
Beachten Sie, dass die Rechenressourcen der Demo begrenzt sind, bitte vermeiden Sie Missbrauch.

<h2 id="install">Installation und Verwendung</h2>

### Installation

1. [**Windows EXE**](https://pdf2zh-next.com/getting-started/INSTALLATION_winexe.html) <small>Empfohlen für Windows</small>
2. [**Docker**](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html) <small>Empfohlen für Linux</small>
3. [**uv** (ein Python-Paketmanager)](https://pdf2zh-next.com/getting-started/INSTALLATION_uv.html) <small>Empfohlen für macOS</small>

---

### Verwendung

1. [Verwendung der **WebUI**](https://pdf2zh-next.com/getting-started/USAGE_webui.html)
2. [Verwendung des **Zotero-Plugins**](https://github.com/guaguastandup/zotero-pdf2zh) (Drittanbieterprogramm)
3. [Verwendung der **Kommandozeile**](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)

Für verschiedene Anwendungsfälle bieten wir unterschiedliche Methoden zur Nutzung unseres Programms. Weitere Informationen finden Sie auf [dieser Seite](./getting-started/getting-started.md).

<h2 id="usage">Erweiterte Optionen</h2>

Für detaillierte Erklärungen lesen Sie bitte unser Dokument über [Erweiterte Verwendung](https://pdf2zh-next.com/advanced/advanced.html) für eine vollständige Liste aller Optionen.

<h2 id="downstream">Sekundäre Entwicklung (APIs)</h2>

> [!NOTE]
>
> Derzeit wird keine relevante Dokumentation bereitgestellt. Sie wird später ergänzt. Bitte haben Sie etwas Geduld.


<!-- For downstream applications, please refer to our document about [API Details](./docs/APIS.md) for futher information about:

- [Python API](./docs/APIS.md#api-python), how to use the program in other Python programs
- [HTTP API](./docs/APIS.md#api-http), how to communicate with a server with the program installed -->

<h2 id="sprachcode">Sprachcode</h2>

Wenn Sie nicht wissen, welchen Code Sie für die Übersetzung in die gewünschte Sprache verwenden sollen, lesen Sie [diese Dokumentation](https://pdf2zh-next.com/advanced/Language-Codes.html)

<!-- 
<h2 id="todo">TODOs</h2>

- [ ] Parse layout with DocLayNet based models, [PaddleX](https://github.com/PaddlePaddle/PaddleX/blob/17cc27ac3842e7880ca4aad92358d3ef8555429a/paddlex/repo_apis/PaddleDetection_api/object_det/official_categories.py#L81), [PaperMage](https://github.com/allenai/papermage/blob/9cd4bb48cbedab45d0f7a455711438f1632abebe/README.md?plain=1#L102), [SAM2](https://github.com/facebookresearch/sam2)

- [ ] Fix page rotation, table of contents, format of lists

- [ ] Fix pixel formula in old papers

- [ ] Async retry except KeyboardInterrupt

- [ ] Knuth–Plass algorithm for western languages

- [ ] Support non-PDF/A files

- [ ] Plugins of [Zotero](https://github.com/zotero/zotero) and [Obsidian](https://github.com/obsidianmd/obsidian-releases) -->

<h2 id="danksagung">Danksagungen</h2>

- [Immersive Translation](https://immersivetranslate.com) sponsert monatliche Pro-Mitgliedschafts-Einlösecodes für aktive Mitwirkende an diesem Projekt. Details finden Sie unter: [CONTRIBUTOR_REWARD.md](https://github.com/funstory-ai/BabelDOC/blob/main/docs/CONTRIBUTOR_REWARD.md)

- [SiliconFlow](https://siliconflow.cn) bietet einen kostenlosen Übersetzungsdienst für dieses Projekt, unterstützt durch große Sprachmodelle (LLMs).

- 1.x Version: [Byaidu/PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate)


- Backend: [BabelDOC](https://github.com/funstory-ai/BabelDOC)

- PDF-Bibliothek: [PyMuPDF](https://github.com/pymupdf/PyMuPDF)

- PDF-Parsing: [Pdfminer.six](https://github.com/pdfminer/pdfminer.six)

- PDF-Vorschau: [Gradio PDF](https://github.com/freddyaboulton/gradio-pdf)

- Layout-Parsing: [DocLayout-YOLO](https://github.com/opendatalab/DocLayout-YOLO)

- PDF-Standards: [PDF Explained](https://zxyle.github.io/PDF-Explained/), [PDF Cheat Sheets](https://pdfa.org/resource/pdf-cheat-sheets/)

- Mehrsprachige Schriftarten: siehe [BabelDOC-Assets](https://github.com/funstory-ai/BabelDOC-Assets)

- [Asynchronize](https://github.com/multimeric/Asynchronize/tree/master?tab=readme-ov-file)

- [Rich logging with multiprocessing](https://github.com/SebastianGrans/Rich-multiprocess-logging/tree/main)

- Dokumentation i18n mit Weblate: [Weblate](https://weblate.org/)

<h2 id="conduct">Bevor Sie Ihren Code einreichen</h2>

Wir freuen uns über die aktive Teilnahme von Mitwirkenden, um pdf2zh besser zu machen. Bevor Sie Ihren Code einreichen, lesen Sie bitte unseren [Verhaltenskodex](https://pdf2zh-next.com/community/CODE_OF_CONDUCT.html) und unseren [Leitfaden für Beiträge](https://pdf2zh-next.com/community/Contribution-Guide.html).

<h2 id="contrib">Mitwirkende</h2>

<a href="https://github.com/PDFMathTranslate/PDFMathTranslate-next/graphs/contributors">
  <img src="https://opencollective.com/PDFMathTranslate/contributors.svg?width=890&button=false" />
</a>

![Alt](https://repobeats.axiom.co/api/embed/45529651750579e099960950f757449a410477ad.svg "Repobeats analytics image")

<h2 id="star_hist">Star-Historie</h2>

<a href="https://star-history.com/#PDFMathTranslate/PDFMathTranslate-next&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date" />
   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date"/>
 <p align="center">
  <a href="https://pdf2zh-next.com">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://pdf2zh-next.com/logo-dark.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://pdf2zh-next.com/logo-light.svg">
      <img alt="pdf2zh" src="https://pdf2zh-next.com/logo-light.svg" width="300">
    </picture>
  </a>
</p>

<p align="center">
  <a href="https://pdf2zh-next.com/getting-started/INSTALLATION.html">Installation</a>
  •
  <a href="https://pdf2zh-next.com/getting-started/USAGE_cli.html">Command Line</a>
  •
  <a href="https://pdf2zh-next.com/getting-started/USAGE_webui.html">WebUI</a>
  •
  <a href="https://pdf2zh-next.com/getting-started/USAGE_api.html">API</a>
  •
  <a href="https://pdf2zh-next.com/getting-started/SUPPORTED_LANGUAGES.html">Supported Languages</a>
  •
  <a href="https://pdf2zh-next.com/getting-started/FAQ.html">FAQ</a>
</p>

---

# PDFMathTranslate

`PDFMathTranslate` is a tool designed to extract and translate LaTeX from PDFs (especially those containing mathematical formulas), and then compile them into a new PDF with the translated content.

## Features

- **Extract LaTeX from PDF**: Accurately identify and extract LaTeX content, including mathematical formulas, from PDF files.
- **Translate LaTeX**: Translate the extracted LaTeX content into the desired language.
- **Compile Translated LaTeX**: Compile the translated LaTeX back into a new PDF file.

## Getting Started

### Installation

To install `PDFMathTranslate`, follow the instructions in the [Installation](#installation) section.

### Usage

For detailed usage instructions, refer to the [Usage](#usage) section.

## Documentation

For more detailed documentation, visit the [Documentation of Translation Services](#documentation-of-translation-services).

## Community

Join our community to get help, share ideas, and contribute to the project.

## FAQ

Check out the [FAQ](#faq) for answers to common questions.

---

<p align="center">
  <a href="https://pdf2zh-next.com">Home</a>
  •
  <a href="https://pdf2zh-next.com/getting-started/GETTING_STARTED.html">Getting Started</a>
  •
  <a href="https://pdf2zh-next.com/getting-started/ADVANCED.html">Advanced</a>
</p>

---

### TRANSLATED TEXT

 </picture>
</a>
</p align="center">
  <a href="https://pdf2zh-next.com">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://pdf2zh-next.com/logo-dark.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://pdf2zh-next.com/logo-light.svg">
      <img alt="pdf2zh" src="https://pdf2zh-next.com/logo-light.svg" width="300">
    </picture>
  </a>
</p>

<p align="center">
  <a href="https://pdf2zh-next.com/getting-started/INSTALLATION.html">Installation</a>
  •
  <a href="https://pdf2zh-next.com/getting-started/USAGE_cli.html">Kommandozeile</a>
  •
  <a href="https://pdf2zh-next.com/getting-started/USAGE_webui.html">WebUI</a>
  •
  <a href="https://pdf2zh-next.com/getting-started/USAGE_api.html">API</a>
  •
  <a href="https://pdf2zh-next.com/getting-started/SUPPORTED_LANGUAGES.html">Unterstützte Sprachen</a>
  •
  <a href="https://pdf2zh-next.com/getting-started/FAQ.html">Häufig gestellte Fragen</a>
</p>

---

# PDFMathTranslate

`PDFMathTranslate` ist ein Tool, das entwickelt wurde, um LaTeX aus PDFs (insbesondere solchen mit mathematischen Formeln) zu extrahieren und zu übersetzen und sie dann in eine neue PDF mit dem übersetzten Inhalt zu kompilieren.

## Funktionen

- **LaTeX aus PDF extrahieren**: LaTeX-Inhalte, einschließlich mathematischer Formeln, präzise identifizieren und aus PDF-Dateien extrahieren.
- **LaTeX übersetzen**: Die extrahierten LaTeX-Inhalte in die gewünschte Sprache übersetzen.
- **Übersetztes LaTeX kompilieren**: Das übersetzte LaTeX zurück in eine neue PDF-Datei kompilieren.

## Erste Schritte

### Installation

Um `PDFMathTranslate` zu installieren, folgen Sie den Anweisungen im Abschnitt [Installation](#installation).

### Verwendung

Detaillierte Anweisungen zur Verwendung finden Sie im Abschnitt [Verwendung](#verwendung).

## Dokumentation

Für eine detailliertere Dokumentation besuchen Sie die [Dokumentation der Übersetzungsdienste](#dokumentation-der-übersetzungsdienste).

## Gemeinschaft

Treten Sie unserer Gemeinschaft bei, um Hilfe zu erhalten, Ideen auszutauschen und zum Projekt beizutragen.

## Häufig gestellte Fragen

Schauen Sie sich die [Häufig gestellte Fragen](#häufig-gestellte-fragen) für Antworten auf häufige Fragen an.

---

<p align="center">
  <a href="https://pdf2zh-next.com">Startseite</a>
  •
  <a href="https://pdf2zh-next.com/getting-started/GETTING_STARTED.html">Erste Schritte</a>
  •
  <a href="https://pdf2zh-next.com/getting-started/ADVANCED.html">Erweiterte Optionen</a>
</p>

---

<div align="right"> 
<h6><small>Ein Teil des Inhalts dieser Seite wurde von GPT übersetzt und kann Fehler enthalten.</small></h6>