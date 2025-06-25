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

<a href="https://t.me/+Z9_SgnxmsmA5NzBl">
    <img src="https://img.shields.io/badge/Telegram-2CA5E0?style=flat-squeare&logo=telegram&logoColor=white"></a>

<!-- License -->
  <a href="./LICENSE">
    <img src="https://img.shields.io/github/license/PDFMathTranslate/PDFMathTranslate-next"></a>
</p>

<a href="https://trendshift.io/repositories/12424" target="_blank"><img src="https://trendshift.io/api/badge/repositories/12424" alt="Byaidu%2FPDFMathTranslate | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>

</div>

PDF 科研论文翻译与双语对照。

- 📊 保留公式、图表、目录和批注 _([效果预览](#preview))_；
- 🌐 支持[多种语言](https://pdf2zh-next.com/supported_languages.html)，提供多样化的[翻译服务](https://pdf2zh-next.com/advanced/翻译服务文档.html)；
- 🤖 提供[命令行工具](https://pdf2zh-next.com/开始使用/USAGE_commandline.html)、[交互式界面](https://pdf2zh-next.com/开始使用/USAGE_webui.html)和[Docker](https://pdf2zh-next.com/开始使用/如何安装_docker.html)。

欢迎通过[GitHub Issues](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues)或[Telegram 群组](https://t.me/+Z9_SgnxmsmA5NzBl)反馈问题。

贡献指南详见[贡献说明](https://pdf2zh-next.com/社区/Contribution-Guide.html)。

<h2 id="updates">更新日志</h2>

- [2025 年 6 月 4 日] 项目更名为[PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next)并迁移至此（by [@awwaawwa](https://github.com/awwaawwa)）
- [2025 年 3 月 3 日] 实验性支持新后端[BabelDOC](https://github.com/funstory-ai/BabelDOC)，新增 WebUI 作为实验选项（by [@awwaawwa](https://github.com/awwaawwa)）
- [2025 年 2 月 22 日] 优化发布 CI 流程，完善 Windows-amd64 可执行文件打包（by [@awwaawwa](https://github.com/awwaawwa)）
- [2024 年 12 月 24 日] 翻译器新增支持[Xinference](https://github.com/xorbitsai/inference)本地模型（by [@imClumsyPanda](https://github.com/imClumsyPanda)）
- [2024 年 12 月 19 日] 通过`-cp`参数支持非 PDF/A 文档（by [@reycn](https://github.com/reycn)）
- [2024 年 12 月 13 日] 新增后端支持（by [@YadominJinta](https://github.com/YadominJinta)）
- [2024 年 12 月 10 日] 翻译器新增支持 Azure 平台的 OpenAI 模型（by [@yidasanqian](https://github.com/yidasanqian)）

<h2 id="preview">效果预览</h2>

<div align="center">
<!-- <img src="./docs/images/preview.gif" width="80%"  alt="preview"/> -->


<img src="https://s.immersivetranslate.com/assets/r2-uploads/images/babeldoc-preview.png" width="80%"/>
</div>

<h2 id="在线服务">在线服务 🌟</h2>

> [!NOTE]
>
> pdf2zh 2.0 目前不提供在线演示

您可以通过以下任一演示尝试我们的应用：

- [v1.x 公共免费服务](https://pdf2zh.com/) 无需安装即可在线使用 _(推荐)_  
- [沉浸式翻译 - BabelDOC](https://app.immersivetranslate.com/babel-doc/) 每月 1000 页免费额度 _(推荐)_

<!-- - [HuggingFace 上的演示](https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker)
- [ModelScope 上的演示](https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate) 无需安装。 -->

请注意，演示环境的计算资源有限，请避免滥用。

<h2 id="如何安装">如何安装和使用</h2>

### 如何安装

1. [**Windows 可执行文件**](https://pdf2zh-next.com/快速开始/如何安装_winexe.html) <small>推荐 Windows 用户使用</small>  
2. [**Docker**](https://pdf2zh-next.com/快速开始/如何安装_docker.html) <small>推荐 Linux 用户使用</small>  
3. [**uv** (Python 包管理器)](https://pdf2zh-next.com/快速开始/如何安装_uv.html) <small>推荐 macOS 用户使用</small>

---

### 如何使用

1. [使用 **WebUI**](https://pdf2zh-next.com/getting-started/USAGE_webui.html)
2. [使用 **Zotero 插件**](https://github.com/guaguastandup/zotero-pdf2zh) (第三方程序)
3. [使用 **命令行**](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)

针对不同使用场景，我们提供了多种程序调用方式。更多信息请查阅[此页面](./getting-started/getting-started.md)。

<h2 id="usage">高级选项</h2>

完整参数说明请参阅[高级用法文档](https://pdf2zh-next.com/advanced/advanced.html)查看所有可选配置项。

<h2 id="downstream">二次开发 (APIs)</h2>

> [!NOTE]
>
> 目前未提供相关文档。后续会补充，请耐心等待。

<!-- 对于下游应用，请参阅我们的 [API 详情](./docs/APIS.md) 文档以获取更多信息：

- [Python API](./docs/APIS.md#api-python)，如何在其他 Python 程序中使用该工具
- [HTTP API](./docs/APIS.md#api-http)，如何与安装了该工具的服务端进行通信 -->

<h2 id="语言代码">Language Code</h2>

如果您不知道需要翻译的目标语言应使用什么代码，请查阅[此文档](https://pdf2zh-next.com/advanced/Language-Codes.html)

<!-- 
<h2 id="todo">待办事项</h2>

- [ ] 使用基于 DocLayNet 的模型解析布局，[PaddleX](https://github.com/PaddlePaddle/PaddleX/blob/17cc27ac3842e7880ca4aad92358d3ef8555429a/paddlex/repo_apis/PaddleDetection_api/object_det/official_categories.py#L81), [PaperMage](https://github.com/allenai/papermage/blob/9cd4bb48cbedab45d0f7a455711438f1632abebe/README.md?plain=1#L102), [SAM2](https://github.com/facebookresearch/sam2)

- [ ] 修复页面旋转、目录结构、列表格式

- [ ] 修复旧论文中的像素公式

- [ ] 异步重试（除键盘中断外）

- [ ] 西文排版 Knuth–Plass 算法

- [ ] 支持非 PDF/A 文件

- [ ] [Zotero](https://github.com/zotero/zotero) 与 [Obsidian](https://github.com/obsidianmd/obsidian-releases) 插件支持 -->

<h2 id="致谢">致谢</h2>

- [沉浸式翻译](https://immersivetranslate.com) 为本项目活跃贡献者每月赞助 Pro 会员兑换码，详情见：[CONTRIBUTOR_REWARD.md](https://github.com/funstory-ai/BabelDOC/blob/main/docs/CONTRIBUTOR_REWARD.md)

- 1.x 版本：[Byaidu/PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate)

- 新后端：[BabelDOC](https://github.com/funstory-ai/BabelDOC)

- 文档合并：[PyMuPDF](https://github.com/pymupdf/PyMuPDF)

- 文档解析：[Pdfminer.six](https://github.com/pdfminer/pdfminer.six)

- 文档提取：[MinerU](https://github.com/opendatalab/MinerU)

- 文档预览：[Gradio PDF](https://github.com/freddyaboulton/gradio-pdf)

- 多线程翻译：[MathTranslate](https://github.com/SUSYUSTC/MathTranslate)

- 版面分析：[DocLayout-YOLO](https://github.com/opendatalab/DocLayout-YOLO)

- 文档标准：[PDF Explained](https://zxyle.github.io/PDF-Explained/), [PDF Cheat Sheets](https://pdfa.org/resource/pdf-cheat-sheets/)

- 多语言字体：[Go Noto Universal](https://github.com/satbyy/go-noto-universal)

- [异步处理](https://github.com/multimeric/Asynchronize/tree/master?tab=readme-ov-file)

- [多进程富日志](https://github.com/SebastianGrans/Rich-multiprocess-logging/tree/main)

<h2 id="conduct">提交代码前</h2>

我们欢迎贡献者积极参与让 pdf2zh 变得更好。在您准备提交代码前，请参阅我们的[行为准则](https://pdf2zh-next.com/community/CODE_OF_CONDUCT.html)和[贡献指南](https://pdf2zh-next.com/community/Contribution-Guide.html)。

<h2 id="contrib">贡献者</h2>

<a href="https://github.com/PDFMathTranslate/PDFMathTranslate-next/graphs/contributors">
  <img src="https://opencollective.com/PDFMathTranslate/contributors.svg?width=890&button=false" />
</a>

![Alt](https://repobeats.axiom.co/api/embed/45529651750579e099960950f757449a410477ad.svg "Repobeats分析图像")

<h2 id="star_hist">Star 历史</h2>

<a href="https://star-history.com/#PDFMathTranslate/PDFMathTranslate-next&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date" />
   <img alt="Star 历史图表" src="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date"/>
 </picture>
</a>

<div align="right"> 
<h6><small>本页面的部分内容由 GPT 翻译，可能包含错误。</small></h6>