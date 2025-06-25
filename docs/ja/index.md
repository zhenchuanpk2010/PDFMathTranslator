<div align="center">

<img src="./docs/images/banner.png" width="320px"  alt="banner"/>

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

<a href="https://t.me/+Z9_SgnxmsmA5NzBl">
    <img src="https://img.shields.io/badge/Telegram-2CA5E0?style=flat-squeare&logo=telegram&logoColor=white"></a>

<!-- License -->
  <a href="./LICENSE">
    <img src="https://img.shields.io/github/license/PDFMathTranslate/PDFMathTranslate-next"></a>
</p>

<a href="https://trendshift.io/repositories/12424" target="_blank"><img src="https://trendshift.io/api/badge/repositories/12424" alt="Byaidu%2FPDFMathTranslate | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>

</div>

PDF科学論文の翻訳とバイリンガル比較。

- 📊 数式、チャート、目次、注釈を保持 _([プレビュー](#プレビュー))_。
- 🌐 [複数言語](https://pdf2zh-next.com/supported_languages.html)をサポートし、多様な[翻訳サービス](https://pdf2zh-next.com/advanced/翻訳サービスドキュメント.html)に対応。
- 🤖 [コマンドラインツール](https://pdf2zh-next.com/始め方/USAGE_commandline.html)、[インタラクティブユーザーインターフェース](https://pdf2zh-next.com/始め方/USAGE_webui.html)、[Docker](https://pdf2zh-next.com/始め方/インストール_docker.html)を提供。

[GitHub Issues](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues) または [Telegram Group](https://t.me/+Z9_SgnxmsmA5NzBl) でフィードバックをお寄せください。

貢献方法の詳細については、[貢献ガイド](https://pdf2zh-next.com/コミュニティ/Contribution-Guide.html)をご覧ください。

<h2 id="updates">更新情報</h2>

- [2025年6月4日] プロジェクト名を変更し、[PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next) に移動 (by [@awwaawwa](https://github.com/awwaawwa))
- [2025年3月3日] 新しいバックエンド [BabelDOC](https://github.com/funstory-ai/BabelDOC) の実験的サポートを追加、WebUIを実験的オプションとして追加 (by [@awwaawwa](https://github.com/awwaawwa))
- [2025年2月22日] リリースCIの改善とWindows-amd64用のexeファイルの適切なパッケージ化 (by [@awwaawwa](https://github.com/awwaawwa))
- [2024年12月24日] [Xinference](https://github.com/xorbitsai/inference) 上のローカルモデルをサポート _(by [@imClumsyPanda](https://github.com/imClumsyPanda))_
- [2024年12月19日] `-cp` を使用して非PDF/Aドキュメントをサポート _(by [@reycn](https://github.com/reycn))_
- [2024年12月13日] 追加のバックエンドサポートを追加 _(by [@YadominJinta](https://github.com/YadominJinta))_
- [2024年12月10日] Azure上のOpenAIモデルをサポート _(by [@yidasanqian](https://github.com/yidasanqian))_

<h2 id="preview">プレビュー</h2>

<div align="center">
<!-- <img src="./docs/images/preview.gif" width="80%"  alt="preview"/> -->


<img src="https://s.immersivetranslate.com/assets/r2-uploads/images/babeldoc-preview.png" width="80%"/>
</div>

<h2 id="demo">オンラインサービス 🌟</h2>

> [!NOTE]
>
> pdf2zh 2.0 は現在オンラインデモを提供していません

以下のデモのいずれかを使用してアプリケーションをお試しください:

- [v1.x パブリック無料サービス](https://pdf2zh.com/) インストール不要でオンライン利用可能 _(推奨)_  
- [Immersive Translate - BabelDOC](https://app.immersivetranslate.com/babel-doc/) 月間1000ページ無料 _(推奨)_

<!-- - [HuggingFaceでホストされたデモ](https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker)
- [インストール不要なModelScopeでホストされたデモ](https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate) -->

デモの計算リソースは限られているため、乱用は避けてください。

<h2 id="install">インストールと使い方</h2>

### インストール

1. [**Windows EXE**](https://pdf2zh-next.com/getting-started/INSTALLATION_winexe.html) <small>Windowsにおすすめ</small>  
2. [**Docker**](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html) <small>Linuxにおすすめ</small>  
3. [**uv** (Pythonパッケージマネージャー)](https://pdf2zh-next.com/getting-started/INSTALLATION_uv.html) <small>macOSにおすすめ</small>

---

### 使い方

1. [**WebUI**の使用](https://pdf2zh-next.com/getting-started/USAGE_webui.html)
2. [**Zotero Plugin**の使用](https://github.com/guaguastandup/zotero-pdf2zh) (サードパーティプログラム)
3. [**コマンドライン**の使用](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)

さまざまな使用ケースに対応するため、当プログラムには複数の利用方法が用意されています。詳細は[このページ](./getting-started/getting-started.md)をご覧ください。

<h2 id="usage">高度な設定</h2>

各オプションの詳細な説明については、[高度な設定](https://pdf2zh-next.com/advanced/advanced.html)のドキュメントを参照してください。

<h2 id="downstream">二次開発 (API)</h2>

> [!NOTE]
>
> 現在、関連するドキュメントは提供されていません。後日追加される予定です。今しばらくお待ちください。

<!-- 下流アプリケーションについては、以下の詳細情報について、[APIの詳細](./docs/APIS.md)を参照してください:

- [Python API](./docs/APIS.md#api-python), 他のPythonプログラムでこのプログラムを使用する方法
- [HTTP API](./docs/APIS.md#api-http), プログラムがインストールされたサーバーと通信する方法 -->

<h2 id="langcode">言語コード</h2>

必要な言語に翻訳する際にどのコードを使用すべきかわからない場合は、[このドキュメント](https://pdf2zh-next.com/advanced/Language-Codes.html)を参照してください

<!-- 
<h2 id="todo">TODOs</h2>

- [ ] DocLayNetベースのモデルでレイアウトを解析、[PaddleX](https://github.com/PaddlePaddle/PaddleX/blob/17cc27ac3842e7880ca4aad92358d3ef8555429a/paddlex/repo_apis/PaddleDetection_api/object_det/official_categories.py#L81), [PaperMage](https://github.com/allenai/papermage/blob/9cd4bb48cbedab45d0f7a455711438f1632abebe/README.md?plain=1#L102), [SAM2](https://github.com/facebookresearch/sam2)

- [ ] ページの回転、目次、リストのフォーマットを修正

- [ ] 古い論文のピクセル式を修正

- [ ] KeyboardInterruptを除く非同期リトライ

- [ ] 西洋言語向けKnuth–Plassアルゴリズム

- [ ] 非PDF/Aファイルのサポート

- [ ] [Zotero](https://github.com/zotero/zotero)と[Obsidian](https://github.com/obsidianmd/obsidian-releases)のプラグイン -->

<h2 id="acknowledgement">謝辞</h2>

- [Immersive Translation](https://immersivetranslate.com) は、このプロジェクトの積極的な貢献者に対して月額Proメンバーシップの引き換えコードをスポンサーしています。詳細はこちら: [CONTRIBUTOR_REWARD.md](https://github.com/funstory-ai/BabelDOC/blob/main/docs/CONTRIBUTOR_REWARD.md)

- 1.x バージョン: [Byaidu/PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate)

- 新しいバックエンド: [BabelDOC](https://github.com/funstory-ai/BabelDOC)

- ドキュメント結合: [PyMuPDF](https://github.com/pymupdf/PyMuPDF)

- ドキュメント解析: [Pdfminer.six](https://github.com/pdfminer/pdfminer.six)

- ドキュメント抽出: [MinerU](https://github.com/opendatalab/MinerU)

- ドキュメントプレビュー: [Gradio PDF](https://github.com/freddyaboulton/gradio-pdf)

- マルチスレッド翻訳: [MathTranslate](https://github.com/SUSYUSTC/MathTranslate)

- レイアウト解析: [DocLayout-YOLO](https://github.com/opendatalab/DocLayout-YOLO)

- ドキュメント標準: [PDF Explained](https://zxyle.github.io/PDF-Explained/), [PDF Cheat Sheets](https://pdfa.org/resource/pdf-cheat-sheets/)

- 多言語フォント: [Go Noto Universal](https://github.com/satbyy/go-noto-universal)

- [Asynchronize](https://github.com/multimeric/Asynchronize/tree/master?tab=readme-ov-file)

- [Rich logging with multiprocessing](https://github.com/SebastianGrans/Rich-multiprocess-logging/tree/main)

<h2 id="conduct">コードを提出する前に</h2>

pdf2zhをより良くするために、貢献者の積極的な参加を歓迎します。コードを提出する準備が整う前に、[行動規範](https://pdf2zh-next.com/community/CODE_OF_CONDUCT.html)と[貢献ガイド](https://pdf2zh-next.com/community/Contribution-Guide.html)を参照してください。

<h2 id="contrib">貢献者</h2>

<a href="https://github.com/PDFMathTranslate/PDFMathTranslate-next/graphs/contributors">
  <img src="https://opencollective.com/PDFMathTranslate/contributors.svg?width=890&button=false" />
</a>

![Alt](https://repobeats.axiom.co/api/embed/45529651750579e099960950f757449a410477ad.svg "Repobeats analytics image")

<h2 id="star_hist">スターの歴史</h2>

<a href="https://star-history.com/#PDFMathTranslate/PDFMathTranslate-next&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date" />
   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date"/>
 </picture>
</a>

<div align="right"> 
<h6><small>このページの一部のコンテンツはGPTによって翻訳されており、エラーが含まれている可能性があります。</small></h6>