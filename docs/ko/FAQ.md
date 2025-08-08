자주 묻는 질문들이 있어, 비슷한 문제를 겪는 사용자들을 위해 목록을 제공했습니다.

## GPU 가 필요한가요?
- **질문**:
프로그램이 인공 지능을 사용하여 문서를 인식하고 추출하기 때문에 GPU 가 필요한가요?

- **답변**:
**GPU 가 필요하지 않습니다.** 하지만 GPU 가 있는 경우 프로그램이 자동으로 이를 사용하여 더 높은 성능을 발휘합니다.

## 다운로드가 중단되었나요?
- **질문**:
모델을 다운로드하는 동안 다음과 같은 중단 오류가 발생했습니다. 어떻게 해야 하나요?

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **답변**:
네트워크에 간섭이 발생하고 있습니다. 안정적인 네트워크 링크를 사용하거나 네트워크 간섭을 우회해 보세요.

## 최신 버전으로 업데이트하는 방법은 무엇인가요?
- **질문**:
최신 버전의 일부 기능을 사용하고 싶은데, 어떻게 업데이트하나요?

- **답변**:
`pip install -U pdf2zh`


## 다음 파일이 존재하지 않습니다: example.pdf
- **문제**:
프로그램을 실행할 때 사용자는 문서를 찾을 수 없는 경우 `다음 파일이 존재하지 않습니다: example.pdf`와 같은 출력을 보게 됩니다.

- **해결 방법**:
  - 파일이 위치한 디렉토리에서 명령줄을 열거나,
  - pdf2zh 뒤에 파일의 전체 경로를 직접 입력하거나,
  - 대화형 모드 `pdf2zh -i`를 사용하여 파일을 직접 드래그 앤 드롭하세요


## SSL 오류 및 기타 네트워크 문제
- **문제**:
허깅 페이스 모델을 다운로드할 때 중국 사용자는 네트워크 오류를 겪을 수 있습니다. 예를 들어, [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55), [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70) 에서 확인할 수 있습니다.

- **해결 방법**:
  - [GFW 우회](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Hugging Face 미러 사용](https://hf-mirror.com/).
  - [포터블 버전 사용](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [대신 Docker 사용](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [인증서 업데이트](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), [이슈 #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55) 에서 제안된 대로.

## 로컬호스트에 접근할 수 없음
아래를 참조하세요.

## 0.0.0.0 를 사용하여 GUI 를 실행하는 중 오류 발생
- **문제**:
전역 모드에서 프록시 소프트웨어를 사용하면 Gradio 가 제대로 시작되지 않을 수 있습니다. 예를 들어, [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77) 에서와 같은 경우가 있습니다.

- **해결 방법**:
규칙 모드 사용

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>이 페이지의 일부 내용은 GPT 에 의해 번역되었으며 오류가 포함될 수 있습니다.</small></h6>