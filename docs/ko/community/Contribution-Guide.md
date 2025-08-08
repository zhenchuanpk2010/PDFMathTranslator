# 프로젝트에 기여하기

> [!CAUTION]
>
> 현재 프로젝트 관리자들은 자동화된 문서 국제화를 연구 중입니다. 따라서 문서 국제화/번역과 관련된 PR 은 **절대 허용되지 않습니다**!
>
> 문서 국제화/번역과 관련된 PR 을 제출하지 마세요!

이 프로젝트에 관심을 가져 주셔서 감사합니다! 기여를 시작하기 전에, 원활한 기여를 위해 다음 가이드라인을 꼭 읽어 주시기 바랍니다.

## 허용되지 않는 기여 유형

1. 문서 국제화/번역
2. HTTP API 등과 같은 핵심 인프라 관련 기여
3. "도움 필요 없음"으로 명시적으로 표시된 이슈 ([Byaidu/PDFMathTranslate](Byaidu/PDFMathTranslate) 및 [PDFMathTranslate/PDFMathTranslate-next](PDFMathTranslate/PDFMathTranslate-next) 저장소의 이슈 포함).
4. 유지 관리자가 부적절하다고 판단한 기타 기여
5. 문서 기여이지만 영어 이외의 언어로 된 문서를 변경하는 경우
6. PDF 파일 수정이 필요한 PR

위와 관련된 유형의 PR 은 제출하지 마십시오.

> [!NOTE]
>
> 문서에 기여하고 싶다면 **문서의 영어 버전만 수정해 주세요**. 다른 언어 버전은 기여자들이 직접 번역합니다.

## 기여 프로세스

1. 이 저장소를 포크하고 로컬에 클론합니다.
2. 새로운 브랜치를 생성합니다: `git checkout -b feature/<feature-name>`.
3. 개발을 진행하고 코드가 요구 사항을 충족하는지 확인합니다.
4. 코드를 커밋합니다:
   ```bash
   git add .
   git commit -m "<semantic commit message>"
   ```
5. 자신의 저장소에 푸시합니다: `git push origin feature/<feature-name>`.
6. GitHub 에서 PR 을 생성하고 상세한 설명을 제공한 후 [@awwaawwa](https://github.com/awwaawwa) 에게 리뷰를 요청합니다.
7. 모든 자동화된 검사가 통과되는지 확인합니다.

> [!TIP]
>
> 개발이 완전히 완료될 때까지 기다릴 필요 없이 PR 을 생성할 수 있습니다. 일찍 생성하면 구현을 검토하고 제안을 제공할 수 있습니다.
>
> 소스 코드 또는 관련 사항에 대한 질문이 있으면 aw@funstory.ai 로 메인테이너에게 문의하세요.
>
> 2.0 버전의 리소스 파일은 [BabelDOC](https://github.com/funstory-ai/BabelDOC) 와 공유됩니다. 관련 리소스를 다운로드하는 코드는 BabelDOC 에 있습니다. 새로운 리소스 파일을 추가하려면 BabelDOC 메인테이너에게 aw@funstory.ai 로 문의하세요.

## 기본 요구 사항

<h4 id="sop">1. 워크플로우</h4>

   - `main` 브랜치에서 포크를 생성하고 포크된 브랜치에서 개발을 진행해 주세요.
   - Pull Request(PR) 를 제출할 때 변경 사항에 대한 상세한 설명을 제공해 주세요.
   - PR 이 자동화된 검사를 통과하지 못하는 경우 (`checks failed` 및 빨간색 십자가로 표시됨), 해당 `details` 를 확인하고 제출물을 수정하여 새로운 PR 이 모든 검사를 통과할 수 있도록 해 주세요.


<h4 id="dev&test">2. 개발 및 테스트</h4>

   - 개발 및 테스트를 위해 `pip install -e .` 명령을 사용하세요.


<h4 id="format">3. 코드 포맷팅</h4>

   - `pre-commit` 도구를 구성하고 코드 서식을 위해 `black` 과 `flake8` 을 활성화하세요.


<h4 id="requpdate">4. 종속성 업데이트</h4>

   - 새로운 종속성을 도입하는 경우, `pyproject.toml` 파일의 종속성 목록을 적시에 업데이트해 주세요.


<h4 id="docupdate">5. 문서 업데이트</h4>

   - 새로운 명령줄 옵션을 추가하는 경우, `README.md` 파일의 모든 언어 버전에서 명령줄 옵션 목록을 해당 사항에 맞게 업데이트해 주세요.


<h4 id="commitmsg">6. 커밋 메시지</h4>

   - [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/) 를 사용하세요. 예: `feat(translator): add openai`.


<h4 id="코딩스타일">7. 코딩 스타일</h4>

   - 제출한 코드가 기본적인 코딩 스타일 표준을 준수하는지 확인하세요.
   - 변수 이름에는 snake_case 또는 camelCase 를 사용하세요.


<h4 id="doctypo">8. 문서 서식</h4>

   - `README.md` 포맷팅은 [중국어 카피라이팅 가이드라인](https://github.com/sparanoid/chinese-copywriting-guidelines) 을 따르세요.
   - 영어 및 중국어 문서는 항상 최신 상태로 유지하고, 다른 언어 문서 업데이트는 선택 사항입니다.

## 번역 엔진 추가하기

1. `pdf2zh/config/translate_engine_model.py` 파일에 새로운 번역기 구성 클래스를 추가합니다.
2. 동일한 파일의 `TRANSLATION_ENGINE_SETTING_TYPE` 타입 별칭에 새로운 번역기 구성 클래스의 인스턴스를 추가합니다.
3. `pdf2zh/translator/translator_impl` 폴더에 새로운 번역기 구현 클래스를 추가합니다.

> [!NOTE]
>
> 이 프로젝트는 RPS(초당 요청 수) 가 4 미만인 번역 엔진을 지원할 계획이 없습니다. 해당 엔진에 대한 지원을 제출하지 마십시오.

## 프로젝트 구조

- **config 폴더**: 구성 시스템.
- **translator 폴더**: 번역기 관련 구현.
- **gui.py**: GUI 인터페이스를 제공.
- **const.py**: 일부 상수.
- **main.py**: 명령줄 도구를 제공.
- **high_level.py**: BabelDOC 기반의 고수준 인터페이스.
- **http_api.py**: HTTP API 를 제공 (시작되지 않음).

## 문의하기

질문이 있으시면 Issue 를 통해 피드백을 제출하거나 Telegram 그룹에 참여해 주세요. 기여해 주셔서 감사합니다!

> [!TIP]
>
> [Immersive Translate](https://immersivetranslate.com) 는 이 프로젝트에 활발히 기여하는 분들을 위해 매월 Pro 멤버십 코드를 후원합니다. 자세한 내용은 다음을 참조하세요: [BabelDOC/PDFMathTranslate 기여자 보상 규칙](https://funstory-ai.github.io/BabelDOC/CONTRIBUTOR_REWARD/)

<div align="right"> 
<h6><small>이 페이지의 일부 내용은 GPT 에 의해 번역되었으며 오류가 포함될 수 있습니다.</small></h6>