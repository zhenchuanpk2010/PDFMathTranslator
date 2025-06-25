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


<a href="https://t.me/+Z9_SgnxmsmA5NzBl">
    <img src="https://img.shields.io/badge/Telegram-2CA5E0?style=flat-squeare&logo=telegram&logoColor=white"></a>

<!-- License -->
  <a href="./LICENSE">
    <img src="https://img.shields.io/github/license/PDFMathTranslate/PDFMathTranslate-next"></a>
</p>

<a href="https://trendshift.io/repositories/12424" target="_blank"><img src="https://trendshift.io/api/badge/repositories/12424" alt="Byaidu%2FPDFMathTranslate | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>

</div>

PDF 과학 논문 번역 및 이중 언어 비교.

- 📊 수식, 차트, 목차 및 주석 보존 _([미리보기](#preview))_.
- 🌐 [다양한 언어](https://pdf2zh-next.com/supported_languages.html) 지원 및 다양한 [번역 서비스](https://pdf2zh-next.com/advanced/Documentation-of-Translation-Services.html).
- 🤖 [명령줄 도구](https://pdf2zh-next.com/getting-started/USAGE_commandline.html), [대화형 사용자 인터페이스](https://pdf2zh-next.com/getting-started/USAGE_webui.html), [Docker](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html) 제공

[GitHub Issues](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues) 또는 [Telegram Group](https://t.me/+Z9_SgnxmsmA5NzBl)에서 피드백을 제공해 주세요.

기여 방법에 대한 자세한 내용은 [기여 가이드](https://pdf2zh-next.com/community/Contribution-Guide.html)를 참조하세요.

<h2 id="updates">업데이트</h2>

- [2025년 6월 4일] 프로젝트 이름 변경 및 [PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next)로 이동 (by [@awwaawwa](https://github.com/awwaawwa))
- [2025년 3월 3일] 새로운 백엔드 [BabelDOC](https://github.com/funstory-ai/BabelDOC) WebUI 실험적 지원 추가 (by [@awwaawwa](https://github.com/awwaawwa))
- [2025년 2월 22일] 개선된 릴리스 CI 및 잘 패키징된 windows-amd64 exe (by [@awwaawwa](https://github.com/awwaawwa))
- [2024년 12월 24일] 번역기가 [Xinference](https://github.com/xorbitsai/inference)의 로컬 모델 지원 _(by [@imClumsyPanda](https://github.com/imClumsyPanda))_
- [2024년 12월 19일] `-cp`를 사용하여 비 PDF/A 문서 지원 _(by [@reycn](https://github.com/reycn))_
- [2024년 12월 13일] 추가 백엔드 지원 _(by [@YadominJinta](https://github.com/YadominJinta))_
- [2024년 12월 10일] 번역기가 Azure의 OpenAI 모델 지원 _(by [@yidasanqian](https://github.com/yidasanqian))_

<h2 id="preview">미리보기</h2>

<div align="center">
<!-- <img src="./docs/images/preview.gif" width="80%"  alt="preview"/> -->


<img src="https://s.immersivetranslate.com/assets/r2-uploads/images/babeldoc-preview.png" width="80%"/>
</div>

<h2 id="demo">온라인 서비스 🌟</h2>

> [!NOTE]
>
> pdf2zh 2.0은 현재 온라인 데모를 제공하지 않습니다.

다음 데모 중 하나를 사용하여 저희 애플리케이션을 시험해 볼 수 있습니다:

- [v1.x 공개 무료 서비스](https://pdf2zh.com/) 설치 없이 온라인에서 이용 가능 _(권장)_.
- [Immersive Translate - BabelDOC](https://app.immersivetranslate.com/babel-doc/) 매월 1000페이지 무료 이용 가능 _(권장)_

<!-- - [HuggingFace에서 호스팅된 데모](https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker)
- [ModelScope에서 호스팅된 데모](https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate) 설치 없이 사용 가능. -->

데모의 컴퓨팅 리소스는 제한적이므로 남용하지 않도록 주의해 주세요.

<h2 id="install">설치 및 사용법</h2>

### 설치

1. [**Windows EXE**](https://pdf2zh-next.com/getting-started/INSTALLATION_winexe.html) <small>Windows에 권장</small>
2. [**Docker**](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html) <small>Linux에 권장</small>
3. [**uv** (a Python package manager)](https://pdf2zh-next.com/getting-started/INSTALLATION_uv.html) <small>macOS에 권장</small>

---

### 사용법

1. [**WebUI** 사용하기](https://pdf2zh-next.com/getting-started/USAGE_webui.html)
2. [**Zotero 플러그인** 사용하기](https://github.com/guaguastandup/zotero-pdf2zh) (서드파티 프로그램)
3. [**명령줄** 사용하기](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)

다양한 사용 사례에 따라 프로그램을 사용하는 별도의 방법을 제공합니다. 자세한 내용은 [이 페이지](./getting-started/getting-started.md)를 확인하세요.

<h2 id="usage">고급 옵션</h2>

자세한 설명은 각 옵션의 전체 목록을 확인할 수 있는 [고급 사용법](https://pdf2zh-next.com/advanced/advanced.html) 문서를 참조하세요.

<h2 id="downstream">2차 개발 (APIs)</h2>

> [!NOTE]
>
> 현재 관련 문서가 제공되지 않습니다. 나중에 보충될 예정이니, 잠시만 기다려 주세요.

<!-- 다운스트림 애플리케이션의 경우, 다음에 대한 자세한 정보는 [API 세부 사항](./docs/APIS.md) 문서를 참조하세요:

- [Python API](./docs/APIS.md#api-python), 다른 Python 프로그램에서 이 프로그램을 사용하는 방법
- [HTTP API](./docs/APIS.md#api-http), 프로그램이 설치된 서버와 통신하는 방법 -->

<h2 id="langcode">언어 코드</h2>

필요한 언어로 번역하기 위해 어떤 코드를 사용해야 할지 모르겠다면 [이 문서](https://pdf2zh-next.com/advanced/Language-Codes.html)를 확인하세요.

<!-- 
<h2 id="todo">할 일</h2>

- [ ] DocLayNet 기반 모델로 레이아웃 파싱, [PaddleX](https://github.com/PaddlePaddle/PaddleX/blob/17cc27ac3842e7880ca4aad92358d3ef8555429a/paddlex/repo_apis/PaddleDetection_api/object_det/official_categories.py#L81), [PaperMage](https://github.com/allenai/papermage/blob/9cd4bb48cbedab45d0f7a455711438f1632abebe/README.md?plain=1#L102), [SAM2](https://github.com/facebookresearch/sam2)

- [ ] 페이지 회전, 목차, 목록 형식 수정

- [ ] 오래된 논문의 픽셀 공식 수정

- [ ] KeyboardInterrupt를 제외한 비동기 재시도

- [ ] 서양 언어를 위한 Knuth–Plass 알고리즘

- [ ] PDF/A가 아닌 파일 지원

- [ ] [Zotero](https://github.com/zotero/zotero) 및 [Obsidian](https://github.com/obsidianmd/obsidian-releases) 플러그인 -->

<h2 id="acknowledgement">감사의 말</h2>

- [Immersive Translation](https://immersivetranslate.com)은 이 프로젝트에 활발히 기여하는 기여자들을 위해 매월 Pro 멤버십 교환 코드를 후원합니다. 자세한 내용은 [CONTRIBUTOR_REWARD.md](https://github.com/funstory-ai/BabelDOC/blob/main/docs/CONTRIBUTOR_REWARD.md)에서 확인하세요.

- 1.x 버전: [Byaidu/PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate)

- 새로운 백엔드: [BabelDOC](https://github.com/funstory-ai/BabelDOC)

- 문서 병합: [PyMuPDF](https://github.com/pymupdf/PyMuPDF)

- 문서 파싱: [Pdfminer.six](https://github.com/pdfminer/pdfminer.six)

- 문서 추출: [MinerU](https://github.com/opendatalab/MinerU)

- 문서 미리보기: [Gradio PDF](https://github.com/freddyaboulton/gradio-pdf)

- 멀티스레드 번역: [MathTranslate](https://github.com/SUSYUSTC/MathTranslate)

- 레이아웃 파싱: [DocLayout-YOLO](https://github.com/opendatalab/DocLayout-YOLO)

- 문서 표준: [PDF Explained](https://zxyle.github.io/PDF-Explained/), [PDF Cheat Sheets](https://pdfa.org/resource/pdf-cheat-sheets/)

- 다국어 폰트: [Go Noto Universal](https://github.com/satbyy/go-noto-universal)

- [Asynchronize](https://github.com/multimeric/Asynchronize/tree/master?tab=readme-ov-file)

- [Rich logging with multiprocessing](https://github.com/SebastianGrans/Rich-multiprocess-logging/tree/main)

<h2 id="conduct">코드 제출 전에</h2>

pdf2zh를 더 나은 프로젝트로 만들기 위해 기여자들의 적극적인 참여를 환영합니다. 코드를 제출하기 전에 [행동 강령](https://pdf2zh-next.com/community/CODE_OF_CONDUCT.html)과 [기여 가이드](https://pdf2zh-next.com/community/Contribution-Guide.html)를 참조해 주세요.

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
<h6><small>이 페이지의 일부 내용은 GPT에 의해 번역되었으며 오류가 포함될 수 있습니다.</small></h6>