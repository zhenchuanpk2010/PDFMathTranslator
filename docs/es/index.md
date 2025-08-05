<div align="center">

<img src="./docs/images/banner.png" width="320px"  alt="banner"/>

<h2 id="titulo">PDFMathTranslate</h2>

<p>
  <!-- PyPI -->
  <a href="https://pypi.org/project/pdf2zh-next/">
    <img src="https://img.shields.io/pypi/v/pdf2zh-next"></a>
  <a href="https://pepy.tech/projects/pdf2zh-next">
    <img src="https://static.pepy.tech/badge/pdf2zh-next"></a>
  <a href="https://hub.docker.com/repository/docker/awwaawwa/pdfmathtranslate-next/tags">
    <img src="https://img.shields.io/docker/pulls/awwaawwa/pdfmathtranslate-next"></a>
  <a href="https://hellogithub.com/repository/8ec2cfd3ef744762bf531232fa32bc47" target="_blank"><img src="https://api.hellogithub.com/v1/widgets/recommend.svg?rid=8ec2cfd3ef744762bf531232fa32bc47&claim_uid=JQ0yfeBNjaTuqDU&theme=small" alt="Destacado｜HelloGitHub" /></a>
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

Traducción de artículos científicos en PDF y comparación bilingüe.

- 📊 Conserva fórmulas, gráficos, tablas de contenido y anotaciones _([vista previa](#vista-previa))_.
- 🌐 Soporta [múltiples idiomas](https://pdf2zh-next.com/supported_languages.html) y diversos [servicios de traducción](https://pdf2zh-next.com/advanced/Documentation-of-Translation-Services.html).
- 🤖 Ofrece [herramienta de línea de comandos](https://pdf2zh-next.com/getting-started/USAGE_commandline.html), [interfaz de usuario interactiva](https://pdf2zh-next.com/getting-started/USAGE_webui.html) y [Docker](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html)

Siéntete libre de proporcionar comentarios en [GitHub Issues](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues) o [Telegram Group](https://t.me/+Z9_SgnxmsmA5NzBl).

Para obtener detalles sobre cómo contribuir, consulta la [Guía de contribución](https://pdf2zh-next.com/community/Contribution-Guide.html).

<h2 id="actualizaciones">Actualizaciones</h2>

- [4 de junio de 2025] El proyecto se renombra y se traslada a [PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next) (por [@awwaawwa](https://github.com/awwaawwa))
- [3 de marzo de 2025] Soporte experimental para el nuevo backend [BabelDOC](https://github.com/funstory-ai/BabelDOC) WebUI añadido como una opción experimental (por [@awwaawwa](https://github.com/awwaawwa))
- [22 de febrero de 2025] Mejor CI de lanzamiento y exe bien empaquetado para windows-amd64 (por [@awwaawwa](https://github.com/awwaawwa))
- [24 de diciembre de 2024] El traductor ahora soporta modelos locales en [Xinference](https://github.com/xorbitsai/inference) _(por [@imClumsyPanda](https://github.com/imClumsyPanda))_
- [19 de diciembre de 2024] Ahora se soportan documentos no PDF/A usando `-cp` _(por [@reycn](https://github.com/reycn))_
- [13 de diciembre de 2024] Soporte adicional para backend por _(por [@YadominJinta](https://github.com/YadominJinta))_
- [10 de diciembre de 2024] El traductor ahora soporta modelos de OpenAI en Azure _(por [@yidasanqian](https://github.com/yidasanqian))_

<h2 id="vista-previa">Vista previa</h2>

<div align="center">
<!-- <img src="./docs/images/preview.gif" width="80%"  alt="preview"/> -->
<img src="https://s.immersivetranslate.com/assets/r2-uploads/images/babeldoc-preview.png" width="80%"/>
</div>

<h2 id="demo">Servicio en línea 🌟</h2>

> [!NOTE]
>
> pdf2zh 2.0 actualmente no proporciona una demostración en línea

Puedes probar nuestra aplicación utilizando cualquiera de las siguientes demostraciones:

- [Servicio público gratuito v1.x](https://pdf2zh.com/) en línea sin instalación _(recomendado)_.
- [Immersive Translate - BabelDOC](https://app.immersivetranslate.com/babel-doc/) 1000 páginas gratuitas al mes. _(recomendado)_
<!-- - [Demo hosted on HuggingFace](https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker)
- [Demo hosted on ModelScope](https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate) without installation. -->

Tenga en cuenta que los recursos informáticos de la demo son limitados, por lo que le recomendamos evitar su abuso.

<h2 id="install">Instalación y Uso</h2>

### Instalación

1. [**Windows EXE**](https://pdf2zh-next.com/getting-started/INSTALLATION_winexe.html) <small>Recomendado para Windows</small>
2. [**Docker**](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html) <small>Recomendado para Linux</small>
3. [**uv** (un gestor de paquetes de Python)](https://pdf2zh-next.com/getting-started/INSTALLATION_uv.html) <small>Recomendado para macOS</small>

---

### Uso

1. [Usando **WebUI**](https://pdf2zh-next.com/getting-started/USAGE_webui.html)
2. [Usando **Plugin de Zotero**](https://github.com/guaguastandup/zotero-pdf2zh) (Programa de terceros)
3. [Usando **Línea de comandos**](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)

Para diferentes casos de uso, proporcionamos distintos métodos para utilizar nuestro programa. Consulta [esta página](./getting-started/getting-started.md) para obtener más información.

<h2 id="usage">Opciones avanzadas</h2>

Para explicaciones detalladas, consulta nuestro documento sobre [Uso avanzado](https://pdf2zh-next.com/advanced/advanced.html) para obtener una lista completa de cada opción.

<h2 id="downstream">Desarrollo secundario (APIs)</h2>

> [!NOTE]
>
> Actualmente, no se proporciona documentación relevante. Se complementará más adelante. Por favor, espere pacientemente.


<!-- For downstream applications, please refer to our document about [API Details](./docs/APIS.md) for futher information about:

- [Python API](./docs/APIS.md#api-python), how to use the program in other Python programs
- [HTTP API](./docs/APIS.md#api-http), how to communicate with a server with the program installed -->

<h2 id="codigodeidioma">Código de idioma</h2>

Si no sabes qué código usar para traducir al idioma que necesitas, consulta [esta documentación](https://pdf2zh-next.com/advanced/Language-Codes.html)

<!-- 
<h2 id="todo">TODOs</h2>

- [ ] Parse layout with DocLayNet based models, [PaddleX](https://github.com/PaddlePaddle/PaddleX/blob/17cc27ac3842e7880ca4aad92358d3ef8555429a/paddlex/repo_apis/PaddleDetection_api/object_det/official_categories.py#L81), [PaperMage](https://github.com/allenai/papermage/blob/9cd4bb48cbedab45d0f7a455711438f1632abebe/README.md?plain=1#L102), [SAM2](https://github.com/facebookresearch/sam2)

- [ ] Fix page rotation, table of contents, format of lists

- [ ] Fix pixel formula in old papers

- [ ] Async retry except KeyboardInterrupt

- [ ] Knuth–Plass algorithm for western languages

- [ ] Support non-PDF/A files

- [ ] Plugins of [Zotero](https://github.com/zotero/zotero) and [Obsidian](https://github.com/obsidianmd/obsidian-releases) -->

<h2 id="reconocimiento">Reconocimientos</h2>

- [Immersive Translation](https://immersivetranslate.com) patrocina códigos de canje mensuales de membresía Pro para contribuyentes activos de este proyecto, consulta los detalles en: [CONTRIBUTOR_REWARD.md](https://github.com/funstory-ai/BabelDOC/blob/main/docs/CONTRIBUTOR_REWARD.md)

- [SiliconFlow](https://siliconflow.cn) proporciona un servicio de traducción gratuito para este proyecto, impulsado por modelos de lenguaje grandes (LLMs).

- Versión 1.x: [Byaidu/PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate)


- backend: [BabelDOC](https://github.com/funstory-ai/BabelDOC)

- Biblioteca PDF: [PyMuPDF](https://github.com/pymupdf/PyMuPDF)

- Análisis de PDF: [Pdfminer.six](https://github.com/pdfminer/pdfminer.six)

- Vista previa de PDF: [Gradio PDF](https://github.com/freddyaboulton/gradio-pdf)

- Análisis de diseño: [DocLayout-YOLO](https://github.com/opendatalab/DocLayout-YOLO)

- Estándares PDF: [PDF Explained](https://zxyle.github.io/PDF-Explained/), [PDF Cheat Sheets](https://pdfa.org/resource/pdf-cheat-sheets/)

- Fuente multilingüe: consulta [BabelDOC-Assets](https://github.com/funstory-ai/BabelDOC-Assets)

- [Asynchronize](https://github.com/multimeric/Asynchronize/tree/master?tab=readme-ov-file)

- [Registro enriquecido con multiprocesamiento](https://github.com/SebastianGrans/Rich-multiprocess-logging/tree/main)

- Documentación i18n usando Weblate: [Weblate](https://weblate.org/)

<h2 id="conduct">Antes de enviar tu código</h2>

Agradecemos la participación activa de los colaboradores para mejorar pdf2zh. Antes de que estés listo para enviar tu código, consulta nuestro [Código de Conducta](https://pdf2zh-next.com/community/CODE_OF_CONDUCT.html) y [Guía de Contribución](https://pdf2zh-next.com/community/Contribution-Guide.html).

<h2 id="contrib">Colaboradores</h2>

<a href="https://github.com/PDFMathTranslate/PDFMathTranslate-next/graphs/contributors">
  <img src="https://opencollective.com/PDFMathTranslate/contributors.svg?width=890&button=false" />
</a>

![Alt](https://repobeats.axiom.co/api/embed/45529651750579e099960950f757449a410477ad.svg "Repobeats analytics image")

<h2 id="historial_de_estrellas">Historial de estrellas</h2>

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

<h1 align="center">PDFMathTranslate</h1>

<p align="center">
  <a href="https://pdf2zh-next.com">Home</a> •
  <a href="https://pdf2zh-next.com/getting-started">Getting Start</a> •
  <a href="https://pdf2zh-next.com/installation">Installation</a> •
  <a href="https://pdf2zh-next.com/usage">Usage</a> •
  <a href="https://pdf2zh-next.com/language-code">Language Code</a> •
  <a href="https://pdf2zh-next.com/documentation-of-translation-services">Documentation of Translation Services</a>
</p>

---

## Getting Started

- [Installation](#installation)
- [Usage](#usage)

## Advanced

- [Supported Languages](#supported-languages)

## Community

- [FAQ](#faq)

---

### Installation

### Usage

---

## License

MIT © [pdf2zh](https://pdf2zh-next.com)

---

### TRANSLATED TEXT

</picture>
</a>
<p align="center">
  <a href="https://pdf2zh-next.com">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="https://pdf2zh-next.com/logo-dark.svg">
      <source media="(prefers-color-scheme: light)" srcset="https://pdf2zh-next.com/logo-light.svg">
      <img alt="pdf2zh" src="https://pdf2zh-next.com/logo-light.svg" width="300">
    </picture>
  </a>
</p>

<h1 align="center">PDFMathTranslate</h1>

<p align="center">
  <a href="https://pdf2zh-next.com">Inicio</a> •
  <a href="https://pdf2zh-next.com/getting-started">Empezar</a> •
  <a href="https://pdf2zh-next.com/installation">Instalación</a> •
  <a href="https://pdf2zh-next.com/usage">Uso</a> •
  <a href="https://pdf2zh-next.com/language-code">Código de idioma</a> •
  <a href="https://pdf2zh-next.com/documentation-of-translation-services">Documentación de servicios de traducción</a>
</p>

---

## Empezar

- [Instalación](#instalación)
- [Uso](#uso)

## Opciones avanzadas

- [Idiomas soportados](#idiomas-soportados)

## Comunidad

- [Preguntas frecuentes](#preguntas-frecuentes)

---

### Instalación

### Uso

---

## Licencia

MIT © [pdf2zh](https://pdf2zh-next.com)

---

<div align="right"> 
<h6><small>Parte del contenido de esta página ha sido traducido por GPT y puede contener errores.</small></h6>