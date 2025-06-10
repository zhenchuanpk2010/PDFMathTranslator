<div align="center">

<img src="./../images/banner.png" width="320px"  alt="banner"/>

<h2 id="title">PDFMathTranslate</h2>

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

PDF 科学论文翻译和双语对照。

- 📊 保留公式、图表、目录和注释 _([预览](#preview))_。
- 🌐 支持[多种语言](https://pdf2zh-next.com/supported_languages.html)和多样的[翻译服务](https://pdf2zh-next.com/advanced/Documentation-of-Translation-Services.html)。
- 🤖 提供[命令行工具](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)、[交互式用户界面](https://pdf2zh-next.com/getting-started/USAGE_webui.html)和[Docker](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html)

欢迎在[GitHub Issues](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues)或[Telegram 群组](https://t.me/+Z9_SgnxmsmA5NzBl)中提供反馈。

有关如何贡献的详细信息，请查阅[贡献指南](https://pdf2zh-next.com/community/Contribution-Guide.html)。

<h2 id="updates">更新</h2>

- [2025 年 6 月 4 日] 项目重命名并迁移至 [PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next) (由 [@awwaawwa](https://github.com/awwaawwa) 提供)
- [2025 年 3 月 3 日] 新后端 [BabelDOC](https://github.com/funstory-ai/BabelDOC) WebUI 作为实验选项添加 (由 [@awwaawwa](https://github.com/awwaawwa) 提供)
- [2025 年 2 月 22 日] 更好的发布 CI 和打包良好的 windows-amd64 exe (由 [@awwaawwa](https://github.com/awwaawwa) 提供)
- [2024 年 12 月 24 日] 译者现在支持 [Xinference](https://github.com/xorbitsai/inference) 上的本地模型 _(由 [@imClumsyPanda](https://github.com/imClumsyPanda) 提供)_
- [2024 年 12 月 19 日] 现在支持非 PDF/A 文档使用 `-cp` _(由 [@reycn](https://github.com/reycn) 提供)_
- [2024 年 12 月 13 日] 额外支持后端 _(由 [@YadominJinta](https://github.com/YadominJinta) 提供)_
- [2024 年 12 月 10 日] 译者现在支持 Azure 上的 OpenAI 模型 _(由 [@yidasanqian](https://github.com/yidasanqian) 提供)_

<h2 id="preview">预览</h2>

<div align="center">
<!-- <img src="./docs/images/preview.gif" width="80%"  alt="preview"/> -->
<img src="https://s.immersivetranslate.com/assets/r2-uploads/images/babeldoc-preview.png" width="80%"/>
</div>

<h2 id="demo">在线服务 🌟</h2>

> [!NOTE]
>
> pdf2zh 2.0 目前不提供在线演示

您可以通过以下任一演示来试用我们的应用程序：

- [v1.x 公共免费服务](https://pdf2zh.com/) 在线使用，无需安装 _(推荐)_。
- [沉浸式翻译 - BabelDOC](https://app.immersivetranslate.com/babel-doc/) 每月 1000 页免费。_(推荐)_
<!-- - [Demo hosted on HuggingFace](https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker)
- [Demo hosted on ModelScope](https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate) without installation. -->

请注意，演示的计算资源有限，请避免滥用。

<h2 id="install">安装和使用</h2>

### 安装

1. [**Windows EXE**](https://pdf2zh-next.com/getting-started/INSTALLATION_winexe.html) <small>推荐用于 Windows</small>
2. [**Docker**](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html) <small>推荐用于 Linux</small>
3. [**uv** (一个 Python 包管理器)](https://pdf2zh-next.com/getting-started/INSTALLATION_uv.html) <small>推荐用于 macOS</small>

---

### 使用

1. [使用 **WebUI**](https://pdf2zh-next.com/getting-started/USAGE_webui.html)
2. [使用 **Zotero 插件**](https://github.com/guaguastandup/zotero-pdf2zh) (第三方程序)
3. [使用 **命令行**](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)

对于不同的使用场景，我们提供不同的方法来使用我们的程序。请查看[此页面](./getting-started/getting-started.md)以获取更多信息。

<h2 id="usage">高级选项</h2>

有关详细说明，请参阅我们的[高级用法](https://pdf2zh-next.com/advanced/advanced.html)文档以获取每个选项的完整列表。

<h2 id="downstream">二次开发 (API)</h2>

> [!NOTE]
>
> 目前没有提供相关文档。将会在后续补充。请耐心等待。


<!-- For downstream applications, please refer to our document about [API Details](./docs/APIS.md) for futher information about:

- [Python API](./docs/APIS.md#api-python), how to use the program in other Python programs
- [HTTP API](./docs/APIS.md#api-http), how to communicate with a server with the program installed -->

<h2 id="langcode">语言代码</h2>

如果您不知道要使用什么代码来翻译成所需的语言，请查看[此文档](https://pdf2zh-next.com/advanced/Language-Codes.html)

<!-- 
<h2 id="todo">TODOs</h2>

- [ ] 使用 DocLayNet 基于模型解析布局，[PaddleX](https://github.com/PaddlePaddle/PaddleX/blob/17cc27ac3842e7880ca4aad92358d3ef8555429a/paddlex/repo_apis/PaddleDetection_api/object_det/official_categories.py#L81), [PaperMage](https://github.com/allenai/papermage/blob/9cd4bb48cbedab45d0f7a455711438f1632abebe/README.md?plain=1#L102), [SAM2](https://github.com/facebookresearch/sam2)

- [ ] 修复页面旋转、目录、列表格式

- [ ] 修复旧论文中的像素公式

- [ ] 异步重试，除非是 KeyboardInterrupt

- [ ] Knuth–Plass 算法用于西方语言

- [ ] 支持非 PDF/A 文件

- [ ] [Zotero](https://github.com/zotero/zotero) 和 [Obsidian](https://github.com/obsidianmd/obsidian-releases) 的插件 -->

<h2 id="acknowledgement">致谢</h2>

- [沉浸式翻译](https://immersivetranslate.com) 为本项目的活跃贡献者提供每月 Pro 会员兑换码，详情请参阅：[CONTRIBUTOR_REWARD.md](https://github.com/funstory-ai/BabelDOC/blob/main/docs/CONTRIBUTOR_REWARD.md)

- 1.x 版本：[Byaidu/PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate)


- 新后端：[BabelDOC](https://github.com/funstory-ai/BabelDOC)

- 文档合并：[PyMuPDF](https://github.com/pymupdf/PyMuPDF)

- 文档解析：[Pdfminer.six](https://github.com/pdfminer/pdfminer.six)

- 文档提取：[MinerU](https://github.com/opendatalab/MinerU)

- 文档预览：[Gradio PDF](https://github.com/freddyaboulton/gradio-pdf)

- 多线程翻译：[MathTranslate](https://github.com/SUSYUSTC/MathTranslate)

- 布局解析：[DocLayout-YOLO](https://github.com/opendatalab/DocLayout-YOLO)

- 文档标准：[PDF Explained](https://zxyle.github.io/PDF-Explained/), [PDF Cheat Sheets](https://pdfa.org/resource/pdf-cheat-sheets/)

- 多语言字体：[Go Noto Universal](https://github.com/satbyy/go-noto-universal)

- [异步化](https://github.com/multimeric/Asynchronize/tree/master?tab=readme-ov-file)

- [多进程日志记录](https://github.com/SebastianGrans/Rich-multiprocess-logging/tree/main)

<h2 id="conduct">提交代码前</h2>

我们欢迎贡献者积极参与使 pdf2zh 更加完善。在您准备提交代码之前，请参阅我们的[行为准则](https://pdf2zh-next.com/community/CODE_OF_CONDUCT.html)和[贡献指南](https://pdf2zh-next.com/community/Contribution-Guide.html)。

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
 </picture>
</a>
