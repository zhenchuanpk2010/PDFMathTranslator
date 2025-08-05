<div align="center">

<img src="./docs/images/banner.png" width="320px"  alt="banner"/>

<h2 id="标题">PDFMathTranslate</h2>

<p>
  <!-- PyPI -->
  <a href="https://pypi.org/project/pdf2zh-next/">
    <img src="https://img.shields.io/pypi/v/pdf2zh-next"></a>
  <a href="https://pepy.tech/projects/pdf2zh-next">
    <img src="https://static.pepy.tech/badge/pdf2zh-next"></a>
  <a href="https://hub.docker.com/repository/docker/awwaawwa/pdfmathtranslate-next/tags">
    <img src="https://img.shields.io/docker/pulls/awwaawwa/pdfmathtranslate-next"></a>
  <a href="https://hellogithub.com/repository/8ec2cfd3ef744762bf531232fa32bc47" target="_blank"><img src="https://api.hellogithub.com/v1/widgets/recommend.svg?rid=8ec2cfd3ef744762bf531232fa32bc47&claim_uid=JQ0yfeBNjaTuqDU&theme=small" alt="精选｜HelloGitHub" /></a>
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

PDF 学术论文翻译与双语对照。

- 📊 保留公式、图表、目录和批注 _([预览](#预览))_。
- 🌐 支持[多种语言](https://pdf2zh-next.com/supported_languages.html)，以及多样化的[翻译服务](https://pdf2zh-next.com/advanced/Documentation-of-Translation-Services.html)。
- 🤖 提供[命令行工具](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)、[交互式用户界面](https://pdf2zh-next.com/getting-started/USAGE_webui.html)和[Docker](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html)

欢迎通过 [GitHub Issues](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues) 或 [Telegram 群组](https://t.me/+Z9_SgnxmsmA5NzBl) 提供反馈。

如需了解如何贡献代码，请参阅 [贡献指南](https://pdf2zh-next.com/community/Contribution-Guide.html)。

<h2 id="更新日志">更新日志</h2>

- [2025 年 6 月 4 日] 项目更名为 [PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next) 并迁移至此仓库 (by [@awwaawwa](https://github.com/awwaawwa))
- [2025 年 3 月 3 日] 实验性支持新后端 [BabelDOC](https://github.com/funstory-ai/BabelDOC) WebUI 作为实验性选项 (by [@awwaawwa](https://github.com/awwaawwa))
- [2025 年 2 月 22 日] 改进发布 CI 流程并完善 Windows-amd64 可执行文件打包 (by [@awwaawwa](https://github.com/awwaawwa))
- [2024 年 12 月 24 日] 翻译器现支持 [Xinference](https://github.com/xorbitsai/inference) 本地模型 _(by [@imClumsyPanda](https://github.com/imClumsyPanda))_
- [2024 年 12 月 19 日] 通过 `-cp` 参数现支持非 PDF/A 格式文档 _(by [@reycn](https://github.com/reycn))_
- [2024 年 12 月 13 日] 新增后端支持 _(by [@YadominJinta](https://github.com/YadominJinta))_
- [2024 年 12 月 10 日] 翻译器现支持 Azure 平台的 OpenAI 模型 _(by [@yidasanqian](https://github.com/yidasanqian))_

<h2 id="预览">预览</h2>

<div align="center">
<!-- <img src="./docs/images/preview.gif" width="80%"  alt="preview"/> -->
<img src="https://s.immersivetranslate.com/assets/r2-uploads/images/babeldoc-preview.png" width="80%"/>
</div>

<h2 id="demo">在线服务 🌟</h2>

> [!NOTE]
>
> pdf2zh 2.0 目前不提供在线演示

您可以通过以下任一演示试用我们的应用程序：

- [v1.x 公共免费服务](https://pdf2zh.com/) 无需安装即可在线使用 _(推荐)_。
- [Immersive Translate - BabelDOC](https://app.immersivetranslate.com/babel-doc/) 每月 1000 页免费额度 _(推荐)_
<!-- - [Demo hosted on HuggingFace](https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker)
- [Demo hosted on ModelScope](https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate) without installation. -->

请注意，演示环境的计算资源有限，请避免滥用。

<h2 id="安装与使用">安装与使用</h2>

### 如何安装

1. [**Windows EXE**](https://pdf2zh-next.com/getting-started/INSTALLATION_winexe.html) <small>推荐 Windows 用户使用</small>
2. [**Docker**](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html) <small>推荐 Linux 用户使用</small>
3. [**uv** (a Python package manager)](https://pdf2zh-next.com/getting-started/INSTALLATION_uv.html) <small>推荐 macOS 用户使用</small>

---

### 如何使用

1. [使用 **WebUI**](https://pdf2zh-next.com/getting-started/USAGE_webui.html)
2. [使用 **Zotero 插件**](https://github.com/guaguastandup/zotero-pdf2zh) (第三方程序)
3. [使用 **命令行**](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)

针对不同的使用场景，我们提供了多种程序调用方式。更多信息请查看[此页面](./getting-started/getting-started.md)。

<h2 id="usage">高级选项</h2>

详细参数说明请参阅[高级用法文档](https://pdf2zh-next.com/advanced/advanced.html)，获取完整参数列表。

<h2 id="downstream">二次开发 (APIs)</h2>

> [!NOTE]
>
> 当前未提供相关文档。后续会补充，请耐心等待。


<!-- For downstream applications, please refer to our document about [API Details](./docs/APIS.md) for futher information about:

- [Python API](./docs/APIS.md#api-python), how to use the program in other Python programs
- [HTTP API](./docs/APIS.md#api-http), how to communicate with a server with the program installed -->

<h2 id="语言代码">Language Code</h2>

如果你不知道应该使用什么代码来翻译到你需要的语言，请查看[这份文档](https://pdf2zh-next.com/advanced/Language-Codes.html)

<!-- 
<h2 id="todo">TODOs</h2>

- [ ] Parse layout with DocLayNet based models, [PaddleX](https://github.com/PaddlePaddle/PaddleX/blob/17cc27ac3842e7880ca4aad92358d3ef8555429a/paddlex/repo_apis/PaddleDetection_api/object_det/official_categories.py#L81), [PaperMage](https://github.com/allenai/papermage/blob/9cd4bb48cbedab45d0f7a455711438f1632abebe/README.md?plain=1#L102), [SAM2](https://github.com/facebookresearch/sam2)

- [ ] Fix page rotation, table of contents, format of lists

- [ ] Fix pixel formula in old papers

- [ ] Async retry except KeyboardInterrupt

- [ ] Knuth–Plass algorithm for western languages

- [ ] Support non-PDF/A files

- [ ] Plugins of [Zotero](https://github.com/zotero/zotero) and [Obsidian](https://github.com/obsidianmd/obsidian-releases) -->

<h2 id="致谢">致谢</h2>

- [Immersive Translation](https://immersivetranslate.com) 为该项目活跃贡献者提供每月 Pro 会员兑换码赞助，详情见：[CONTRIBUTOR_REWARD.md](https://github.com/funstory-ai/BabelDOC/blob/main/docs/CONTRIBUTOR_REWARD.md)

- [SiliconFlow](https://siliconflow.cn) 为本项目提供基于大语言模型 (LLM) 的免费翻译服务。

- 1.x 版本：[Byaidu/PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate)


- 后端：[BabelDOC](https://github.com/funstory-ai/BabelDOC)

- PDF 库：[PyMuPDF](https://github.com/pymupdf/PyMuPDF)

- PDF 解析：[Pdfminer.six](https://github.com/pdfminer/pdfminer.six)

- PDF 预览：[Gradio PDF](https://github.com/freddyaboulton/gradio-pdf)

- 版面分析：[DocLayout-YOLO](https://github.com/opendatalab/DocLayout-YOLO)

- PDF 标准：[PDF Explained](https://zxyle.github.io/PDF-Explained/), [PDF Cheat Sheets](https://pdfa.org/resource/pdf-cheat-sheets/)

- 多语言字体：参见 [BabelDOC-Assets](https://github.com/funstory-ai/BabelDOC-Assets)

- [Asynchronize](https://github.com/multimeric/Asynchronize/tree/master?tab=readme-ov-file)

- [Rich logging with multiprocessing](https://github.com/SebastianGrans/Rich-multiprocess-logging/tree/main)

- 文档国际化使用 Weblate：[Weblate](https://weblate.org/)

<h2 id="conduct">提交代码前</h2>

我们欢迎贡献者积极参与，让 pdf2zh 变得更好。在您准备提交代码之前，请参阅我们的[行为准则](https://pdf2zh-next.com/community/CODE_OF_CONDUCT.html)和[贡献指南](https://pdf2zh-next.com/community/Contribution-Guide.html)。

<h2 id="contrib">贡献者</h2>

<a href="https://github.com/PDFMathTranslate/PDFMathTranslate-next/graphs/contributors">
  <img src="https://opencollective.com/PDFMathTranslate/contributors.svg?width=890&button=false" />
</a>

![Alt](https://repobeats.axiom.co/api/embed/45529651750579e099960950f757449a410477ad.svg "Repobeats analytics image")

<h2 id="star_hist">Star 历史</h2>

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
  <a href="https://pdf2zh-next.com">Home</a> •
  <a href="https://pdf2zh-next.com/getting-started">Getting Start</a> •
  <a href="https://pdf2zh-next.com/getting-started/INSTALLATION.html">Installation</a> •
  <a href="https://pdf2zh-next.com/getting-started/USAGE_cli.html">Command Line</a> •
  <a href="https://pdf2zh-next.com/getting-started/USAGE_webui.html">Usage</a> •
  <a href="https://pdf2zh-next.com/getting-started/LANGUAGE_CODE.html">Language Code</a> •
  <a href="https://pdf2zh-next.com/getting-started/DOCUMENTATION_TRANSLATION_SERVICES.html">Documentation of Translation Services</a>
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

<p align="center">
  <a href="https://immersivetranslate.com/">
    <img src="https://pdf2zh-next.com/imgs/immersive-translate.png" width="300" alt="Immersive Translate">
  </a>
</p>

<p align="center">
  <a href="https://immersivetranslate.com/">Immersive Translate</a>
</p>

---

### ORIGINAL TEXT

 </picture>
</a>
</p>

<p align="center">
  <a href="https://pdf2zh-next.com">主页</a> •
  <a href="https://pdf2zh-next.com/getting-started">快速开始</a> •
  <a href="https://pdf2zh-next.com/getting-started/INSTALLATION.html">如何安装</a> •
  <a href="https://pdf2zh-next.com/getting-started/USAGE_cli.html">命令行</a> •
  <a href="https://pdf2zh-next.com/getting-started/USAGE_webui.html">如何使用</a> •
  <a href="https://pdf2zh-next.com/getting-started/LANGUAGE_CODE.html">语言代码</a> •
  <a href="https://pdf2zh-next.com/getting-started/DOCUMENTATION_TRANSLATION_SERVICES.html">翻译服务文档</a>
</p>

---

## 开始使用

- [如何安装](#如何安装)
- [如何使用](#如何使用)

## 高级选项

- [支持的语言](#支持的语言)

## 社区

- [常见问题](#常见问题)

---

### 如何安装

### 如何使用

---

<p align="center">
  <a href="https://immersivetranslate.com/">
    <img src="https://pdf2zh-next.com/imgs/immersive-translate.png" width="300" alt="沉浸式翻译">
  </a>
</p>

<p align="center">
  <a href="https://immersivetranslate.com/">沉浸式翻译</a>
</p>

<div align="right"> 
<h6><small>本页面的部分内容由 GPT 翻译，可能包含错误。</small></h6>