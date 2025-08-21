<div align="center">

<img src="./docs/images/banner.png" width="320px"  alt="banner"/>

<h2 id="標題">PDFMathTranslate</h2>

<p>
  <!-- PyPI -->
  <a href="https://pypi.org/project/pdf2zh-next/">
    <img src="https://img.shields.io/pypi/v/pdf2zh-next"></a>
  <a href="https://pepy.tech/projects/pdf2zh-next">
    <img src="https://static.pepy.tech/badge/pdf2zh-next"></a>
  <a href="https://hub.docker.com/repository/docker/awwaawwa/pdfmathtranslate-next/tags">
    <img src="https://img.shields.io/docker/pulls/awwaawwa/pdfmathtranslate-next"></a>
  <a href="https://hellogithub.com/repository/8ec2cfd3ef744762bf531232fa32bc47" target="_blank"><img src="https://api.hellogithub.com/v1/widgets/recommend.svg?rid=8ec2cfd3ef744762bf531232fa32bc47&claim_uid=JQ0yfeBNjaTuqDU&theme=small" alt="精選｜HelloGitHub" /></a>
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
  <a href="https://hosted.weblate.org/engage/pdfmathtranslate-next/">
    <img src="https://hosted.weblate.org/widget/pdfmathtranslate-next/svg-badge.svg" alt="translation status" /></a>
</p>

<a href="https://trendshift.io/repositories/12424" target="_blank"><img src="https://trendshift.io/api/badge/repositories/12424" alt="Byaidu%2FPDFMathTranslate | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>

</div>

PDF 科學論文翻譯與雙語對照。

- 📊 保留公式、圖表、目錄和註解 _([預覽](#預覽))_。
- 🌐 支援 [多種語言](https://pdf2zh-next.com/supported_languages.html) 和多樣的 [翻譯服務](https://pdf2zh-next.com/advanced/Documentation-of-Translation-Services.html)。
- 🤖 提供 [命令行工具](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)、[互動式用戶界面](https://pdf2zh-next.com/getting-started/USAGE_webui.html) 和 [Docker](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html)

<!-- Feel free to provide feedback in [GitHub Issues](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues) or [Telegram Group](https://t.me/+Z9_SgnxmsmA5NzBl). -->

> [!WARNING]
>
> 本項目基於 [AGPL v3](https://github.com/PDFMathTranslate/PDFMathTranslate-next/blob/main/LICENSE) 許可協議「按原樣」提供，對程序的質量及性能不作任何擔保。**您需自行承擔程序質量與性能的全部風險。** 若程序被發現存在缺陷，您將承擔所有必要的服務、修復或修正費用。
>
> 由於維護者精力有限，我們不提供任何形式的使用協助或問題解決。相關議題將被直接關閉！（歡迎提交改進項目文檔的拉取請求；遵循議題模板的錯誤報告或友善議題不受此限制）


有關如何貢獻的詳細資訊，請參閱 [Contribution Guide](https://pdf2zh-next.com/community/Contribution-Guide.html)。

<h2 id="更新">更新</h2>

- [2025 年 6 月 4 日] 項目更名並遷移至 [PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next)（由 [@awwaawwa](https://github.com/awwaawwa)）
- [2025 年 3 月 3 日] 實驗性支持新後端 [BabelDOC](https://github.com/funstory-ai/BabelDOC) WebUI 作為實驗性選項（由 [@awwaawwa](https://github.com/awwaawwa)）
- [2025 年 2 月 22 日] 更好的發佈 CI 和打包良好的 windows-amd64 exe（由 [@awwaawwa](https://github.com/awwaawwa)）
- [2024 年 12 月 24 日] 翻譯器現在支持 [Xinference](https://github.com/xorbitsai/inference) 上的本地模型（由 [@imClumsyPanda](https://github.com/imClumsyPanda)）
- [2024 年 12 月 19 日] 現在支持使用 `-cp` 處理非 PDF/A 文檔（由 [@reycn](https://github.com/reycn)）
- [2024 年 12 月 13 日] 額外支持後端（由 [@YadominJinta](https://github.com/YadominJinta)）
- [2024 年 12 月 10 日] 翻譯器現在支持 Azure 上的 OpenAI 模型（由 [@yidasanqian](https://github.com/yidasanqian)）

<h2 id="預覽">預覽</h2>

<div align="center">
<!-- <img src="./docs/images/preview.gif" width="80%"  alt="preview"/> -->
<img src="https://s.immersivetranslate.com/assets/r2-uploads/images/babeldoc-preview.png" width="80%"/>
</div>

<h2 id="demo">線上服務 🌟</h2>

> [!NOTE]
>
> pdf2zh 2.0 目前不提供線上演示

您可以使用以下任一示範來試用我們的應用程式：

- [v1.x 公開免費服務](https://pdf2zh.com/) 無需安裝即可在線使用 _(推薦)_。
- [Immersive Translate - BabelDOC](https://app.immersivetranslate.com/babel-doc/) 每月 1000 頁免費額度 _(推薦)_
<!-- - [Demo hosted on HuggingFace](https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker)
- [Demo hosted on ModelScope](https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate) without installation. -->

請注意，示範用的計算資源有限，請避免濫用。

<h2 id="安裝">如何安裝與使用</h2>

### 如何安裝

1. [**Windows EXE**](https://pdf2zh-next.com/getting-started/INSTALLATION_winexe.html) <small>Windows 用戶推薦</small>
2. [**Docker**](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html) <small>Linux 用戶推薦</small>
3. [**uv** (a Python package manager)](https://pdf2zh-next.com/getting-started/INSTALLATION_uv.html) <small>macOS 用戶推薦</small>

---

### 如何使用

1. [使用 **WebUI**](https://pdf2zh-next.com/getting-started/USAGE_webui.html)
2. [使用 **Zotero 插件**](https://github.com/guaguastandup/zotero-pdf2zh) (第三方程序)
3. [使用 **命令行**](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)

針對不同的使用情境，我們提供了多種方法來使用我們的程式。更多資訊請參閱 [此頁面](./getting-started/getting-started.md)。

<h2 id="usage">高級選項</h2>

如需詳細說明，請參閱我們的 [高級使用](https://pdf2zh-next.com/advanced/advanced.html) 文件，以獲取每個選項的完整列表。

<h2 id="downstream">二次開發 (APIs)</h2>

> [!NOTE]
>
> 目前尚未提供相關文檔。後續將會補充，請耐心等待。


<!-- For downstream applications, please refer to our document about [API Details](./docs/APIS.md) for futher information about:

- [Python API](./docs/APIS.md#api-python), how to use the program in other Python programs
- [HTTP API](./docs/APIS.md#api-http), how to communicate with a server with the program installed -->

<h2 id="langcode">語言代碼</h2>

如果你不知道該使用什麼代碼來翻譯到你需要的語言，請查看 [這份文檔](https://pdf2zh-next.com/advanced/Language-Codes.html)

<!-- 
<h2 id="todo">TODOs</h2>

- [ ] Parse layout with DocLayNet based models, [PaddleX](https://github.com/PaddlePaddle/PaddleX/blob/17cc27ac3842e7880ca4aad92358d3ef8555429a/paddlex/repo_apis/PaddleDetection_api/object_det/official_categories.py#L81), [PaperMage](https://github.com/allenai/papermage/blob/9cd4bb48cbedab45d0f7a455711438f1632abebe/README.md?plain=1#L102), [SAM2](https://github.com/facebookresearch/sam2)

- [ ] Fix page rotation, table of contents, format of lists

- [ ] Fix pixel formula in old papers

- [ ] Async retry except KeyboardInterrupt

- [ ] Knuth–Plass algorithm for western languages

- [ ] Support non-PDF/A files

- [ ] Plugins of [Zotero](https://github.com/zotero/zotero) and [Obsidian](https://github.com/obsidianmd/obsidian-releases) -->

<h2 id="致謝">致謝</h2>

- [Immersive Translation](https://immersivetranslate.com) 為本專案的活躍貢獻者提供每月 Pro 會員兌換碼，詳情請見：[CONTRIBUTOR_REWARD.md](https://github.com/funstory-ai/BabelDOC/blob/main/docs/CONTRIBUTOR_REWARD.md)

- [SiliconFlow](https://siliconflow.cn) 為本專案提供免費的翻譯服務，由大型語言模型（LLMs）驅動。

- 1.x 版本：[Byaidu/PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate)


- 後端：[BabelDOC](https://github.com/funstory-ai/BabelDOC)

- PDF 函式庫：[PyMuPDF](https://github.com/pymupdf/PyMuPDF)

- PDF 解析：[Pdfminer.six](https://github.com/pdfminer/pdfminer.six)

- PDF 預覽：[Gradio PDF](https://github.com/freddyaboulton/gradio-pdf)

- 版面解析：[DocLayout-YOLO](https://github.com/opendatalab/DocLayout-YOLO)

- PDF 標準：[PDF Explained](https://zxyle.github.io/PDF-Explained/), [PDF Cheat Sheets](https://pdfa.org/resource/pdf-cheat-sheets/)

- 多語言字型：請參閱 [BabelDOC-Assets](https://github.com/funstory-ai/BabelDOC-Assets)

- [Asynchronize](https://github.com/multimeric/Asynchronize/tree/master?tab=readme-ov-file)

- [Rich logging with multiprocessing](https://github.com/SebastianGrans/Rich-multiprocess-logging/tree/main)

- 使用 [Weblate](https://hosted.weblate.org/projects/pdfmathtranslate-next/) 進行文檔國際化


<h2 id="conduct">提交代碼前</h2>

我們歡迎貢獻者的積極參與，讓 pdf2zh 變得更好。在您準備提交代碼之前，請參考我們的 [行為準則](https://pdf2zh-next.com/community/CODE_OF_CONDUCT.html) 和 [貢獻指南](https://pdf2zh-next.com/community/Contribution-Guide.html)。

<h2 id="contrib">貢獻者</h2>

<a href="https://github.com/PDFMathTranslate/PDFMathTranslate-next/graphs/contributors">
  <img src="https://opencollective.com/PDFMathTranslate/contributors.svg?width=890&button=false" />
</a>

![Alt](https://repobeats.axiom.co/api/embed/45529651750579e099960950f757449a410477ad.svg "Repobeats analytics image")

<h2 id="star_hist">星標歷史</h2>

<a href="https://star-history.com/#PDFMathTranslate/PDFMathTranslate-next&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date" />
   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date"/>
 </picture>
</a>

<div align="right"> 
<h6><small>Some content on this page has been translated by GPT and may contain errors.</small></h6>