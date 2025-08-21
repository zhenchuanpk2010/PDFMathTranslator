<div align="center">

<img src="./docs/images/banner.png" width="320px"  alt="banner"/>

<h2 id="제목">PDFMathTranslate</h2>

<p>
  <!-- PyPI -->
  <a href="https://pypi.org/project/pdf2zh-next/">
    <img src="https://img.shields.io/pypi/v/pdf2zh-next"></a>
  <a href="https://pepy.tech/projects/pdf2zh-next">
    <img src="https://static.pepy.tech/badge/pdf2zh-next"></a>
  <a href="https://hub.docker.com/repository/docker/awwaawwa/pdfmathtranslate-next/tags">
    <img src="https://img.shields.io/docker/pulls/awwaawwa/pdfmathtranslate-next"></a>
  <a href="https://hellogithub.com/repository/8ec2cfd3ef744762bf531232fa32bc47" target="_blank"><img src="https://api.hellogithub.com/v1/widgets/recommend.svg?rid=8ec2cfd3ef744762bf531232fa32bc47&claim_uid=JQ0yfeBNjaTuqDU&theme=small" alt="추천｜HelloGitHub" /></a>
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

PDF 과학 논문 번역 및 이중 언어 비교.

- 📊 수식, 차트, 목차 및 주석 보존 _([미리보기](#미리보기))_.
- 🌐 [다양한 언어](https://pdf2zh-next.com/supported_languages.html) 및 다양한 [번역 서비스](https://pdf2zh-next.com/advanced/Documentation-of-Translation-Services.html) 지원.
- 🤖 [명령줄 도구](https://pdf2zh-next.com/getting-started/USAGE_commandline.html), [대화형 사용자 인터페이스](https://pdf2zh-next.com/getting-started/USAGE_webui.html), [Docker](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html) 제공

<!-- Feel free to provide feedback in [GitHub Issues](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues) or [Telegram Group](https://t.me/+Z9_SgnxmsmA5NzBl). -->

> [!WARNING]
>
> 이 프로젝트는 [AGPL v3](https://github.com/PDFMathTranslate/PDFMathTranslate-next/blob/main/LICENSE) 라이선스 하에 "있는 그대로" 제공되며, 프로그램의 품질과 성능에 대한 어떠한 보증도 제공되지 않습니다. **프로그램의 품질과 성능에 대한 모든 위험은 사용자 본인이 부담합니다.** 프로그램에 결함이 발견될 경우, 필요한 모든 서비스, 수리 또는 수정 비용은 사용자 본인이 책임져야 합니다.
>
> 유지보수 담당자의 제한된 에너지로 인해, 우리는 어떠한 형태의 사용 지원이나 문제 해결도 제공하지 않습니다. 관련 이슈는 즉시 닫힐 것입니다! (프로젝트 문서 개선을 위한 풀 리퀘스트는 환영합니다; 이슈 템플릿을 준수하는 버그 또는 친절한 이슈는 이 정책의 영향을 받지 않습니다)


자세한 기여 방법은 [기여 가이드](https://pdf2zh-next.com/community/Contribution-Guide.html) 를 참조하세요.

<h2 id="업데이트">업데이트</h2>

- [2025 년 6 월 4 일] 프로젝트 이름이 변경되어 [PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next) 로 이동했습니다 (by [@awwaawwa](https://github.com/awwaawwa))
- [2025 년 3 월 3 일] 새로운 백엔드 [BabelDOC](https://github.com/funstory-ai/BabelDOC) WebUI 에 대한 실험적 지원이 추가되었습니다 (by [@awwaawwa](https://github.com/awwaawwa))
- [2025 년 2 월 22 일] 개선된 릴리스 CI 와 잘 패키징된 windows-amd64 exe 가 추가되었습니다 (by [@awwaawwa](https://github.com/awwaawwa))
- [2024 년 12 월 24 일] 번역기가 이제 [Xinference](https://github.com/xorbitsai/inference) 의 로컬 모델을 지원합니다 _(by [@imClumsyPanda](https://github.com/imClumsyPanda))_
- [2024 년 12 월 19 일] `-cp` 를 사용하여 비-PDF/A 문서가 이제 지원됩니다 _(by [@reycn](https://github.com/reycn))_
- [2024 년 12 월 13 일] 추가 백엔드 지원이 추가되었습니다 _(by [@YadominJinta](https://github.com/YadominJinta))_
- [2024 년 12 월 10 일] 번역기가 이제 Azure 의 OpenAI 모델을 지원합니다 _(by [@yidasanqian](https://github.com/yidasanqian))_

<h2 id="미리보기">미리보기</h2>

<div align="center">
<!-- <img src="./docs/images/preview.gif" width="80%"  alt="preview"/> -->
<img src="https://s.immersivetranslate.com/assets/r2-uploads/images/babeldoc-preview.png" width="80%"/>
</div>

<h2 id="demo">온라인 서비스 🌟</h2>

> [!NOTE]
>
> pdf2zh 2.0 은 현재 온라인 데모를 제공하지 않습니다

다음 데모 중 하나를 사용하여 저희 애플리케이션을 시험해 볼 수 있습니다:

- [v1.x 공개 무료 서비스](https://pdf2zh.com/) 설치 없이 온라인에서 이용 가능 _(권장)_.
- [Immersive Translate - BabelDOC](https://app.immersivetranslate.com/babel-doc/) 매월 1000 페이지 무료 이용 가능 _(권장)_
<!-- - [Demo hosted on HuggingFace](https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker)
- [Demo hosted on ModelScope](https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate) without installation. -->

데모의 컴퓨팅 리소스는 제한되어 있으므로 남용하지 않도록 주의해 주세요.

<h2 id="설치">설치 및 사용법</h2>

### 설치

1. [**Windows EXE**](https://pdf2zh-next.com/getting-started/INSTALLATION_winexe.html) <small>Windows 용 추천</small>
2. [**Docker**](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html) <small>Linux 용 추천</small>
3. [**uv** (a Python package manager)](https://pdf2zh-next.com/getting-started/INSTALLATION_uv.html) <small>macOS 용 추천</small>

---

### 사용법

1. [**WebUI** 사용](https://pdf2zh-next.com/getting-started/USAGE_webui.html)
2. [**Zotero 플러그인** 사용](https://github.com/guaguastandup/zotero-pdf2zh) (서드파티 프로그램)
3. [**명령줄** 사용](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)

다양한 사용 사례에 따라 우리 프로그램을 사용하는 별도의 방법을 제공합니다. 더 많은 정보는 [이 페이지](./getting-started/getting-started.md) 를 확인하세요.

<h2 id="usage">고급 옵션</h2>

자세한 설명은 각 옵션의 전체 목록을 확인하기 위해 [고급 사용법](https://pdf2zh-next.com/advanced/advanced.html) 문서를 참조하세요.

<h2 id="downstream">2 차 개발 (API)</h2>

> [!NOTE]
>
> 현재 관련 문서가 제공되지 않습니다. 나중에 보충될 예정이니, 조금만 기다려 주세요.


<!-- For downstream applications, please refer to our document about [API Details](./docs/APIS.md) for futher information about:

- [Python API](./docs/APIS.md#api-python), how to use the program in other Python programs
- [HTTP API](./docs/APIS.md#api-http), how to communicate with a server with the program installed -->

<h2 id="langcode">언어 코드</h2>

필요한 언어로 번역하기 위해 어떤 코드를 사용해야 할지 모르겠다면 [이 문서](https://pdf2zh-next.com/advanced/Language-Codes.html) 를 확인하세요.

<!-- 
<h2 id="todo">TODOs</h2>

- [ ] Parse layout with DocLayNet based models, [PaddleX](https://github.com/PaddlePaddle/PaddleX/blob/17cc27ac3842e7880ca4aad92358d3ef8555429a/paddlex/repo_apis/PaddleDetection_api/object_det/official_categories.py#L81), [PaperMage](https://github.com/allenai/papermage/blob/9cd4bb48cbedab45d0f7a455711438f1632abebe/README.md?plain=1#L102), [SAM2](https://github.com/facebookresearch/sam2)

- [ ] Fix page rotation, table of contents, format of lists

- [ ] Fix pixel formula in old papers

- [ ] Async retry except KeyboardInterrupt

- [ ] Knuth–Plass algorithm for western languages

- [ ] Support non-PDF/A files

- [ ] Plugins of [Zotero](https://github.com/zotero/zotero) and [Obsidian](https://github.com/obsidianmd/obsidian-releases) -->

<h2 id="acknowledgement">감사의 말</h2>

- [Immersive Translation](https://immersivetranslate.com) 은 이 프로젝트에 활발히 기여하는 기여자들을 위해 매월 Pro 멤버십 교환 코드를 후원합니다. 자세한 내용은 [CONTRIBUTOR_REWARD.md](https://github.com/funstory-ai/BabelDOC/blob/main/docs/CONTRIBUTOR_REWARD.md) 에서 확인하세요.

- [SiliconFlow](https://siliconflow.cn) 는 이 프로젝트를 위해 대규모 언어 모델 (LLM) 로 구동되는 무료 번역 서비스를 제공합니다.

- 1.x 버전: [Byaidu/PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate)


- 백엔드: [BabelDOC](https://github.com/funstory-ai/BabelDOC)

- PDF 라이브러리: [PyMuPDF](https://github.com/pymupdf/PyMuPDF)

- PDF 파싱: [Pdfminer.six](https://github.com/pdfminer/pdfminer.six)

- PDF 미리보기: [Gradio PDF](https://github.com/freddyaboulton/gradio-pdf)

- 레이아웃 파싱: [DocLayout-YOLO](https://github.com/opendatalab/DocLayout-YOLO)

- PDF 표준: [PDF Explained](https://zxyle.github.io/PDF-Explained/), [PDF Cheat Sheets](https://pdfa.org/resource/pdf-cheat-sheets/)

- 다국어 폰트: [BabelDOC-Assets](https://github.com/funstory-ai/BabelDOC-Assets) 참조

- [Asynchronize](https://github.com/multimeric/Asynchronize/tree/master?tab=readme-ov-file)

- [Rich logging with multiprocessing](https://github.com/SebastianGrans/Rich-multiprocess-logging/tree/main)

- 문서 국제화 (i18n) 는 [Weblate](https://hosted.weblate.org/projects/pdfmathtranslate-next/) 를 사용합니다.


<h2 id="conduct">코드 제출 전에</h2>

우리는 pdf2zh 를 더 나은 방향으로 발전시키기 위해 기여자들의 적극적인 참여를 환영합니다. 코드를 제출하기 전에 [행동 강령](https://pdf2zh-next.com/community/CODE_OF_CONDUCT.html) 과 [기여 가이드](https://pdf2zh-next.com/community/Contribution-Guide.html) 를 참고해 주세요.

<h2 id="contrib">기여자</h2>

<a href="https://github.com/PDFMathTranslate/PDFMathTranslate-next/graphs/contributors">
  <img src="https://opencollective.com/PDFMathTranslate/contributors.svg?width=890&button=false" />
</a>

![Alt](https://repobeats.axiom.co/api/embed/45529651750579e099960950f757449a410477ad.svg "Repobeats analytics image")

<h2 id="star_hist">스타 히스토리</h2>

<a href="https://star-history.com/#PDFMathTranslate/PDFMathTranslate-next&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date" />
   <img alt="Star History Chart" src="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date"/>
 </picture>
</a>

<div align="right"> 
<h6><small>이 페이지의 일부 내용은 GPT 에 의해 번역되었으며 오류가 포함될 수 있습니다.</small></h6>