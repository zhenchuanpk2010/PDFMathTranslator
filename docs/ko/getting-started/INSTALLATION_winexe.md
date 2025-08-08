[**시작하기**](./getting-started.md) > **설치** > **Windows EXE** _(현재)_

---

### .exe 파일로 PDFMathTranslate 설치하기

***1 단계*** | [릴리스 페이지](https://github.com/PDFMathTranslate/PDFMathTranslate-next/releases) 에서 `pdf2zh-<version>-with-assets-win64.zip` 을 다운로드하세요.

> [!TIP]
> **`pdf2zh-<version>-with-assets-win64.zip` 와 `pdf2zh-<version>-win64.zip` 의 차이점은 무엇인가요?**
>
> - PDFMathTranslate 를 처음 다운로드하여 사용하는 경우 `pdf2zh-<version>-with-assets-win64.zip` 을 다운로드하는 것이 권장됩니다.
> - `pdf2zh-<version>-with-assets-win64.zip` 은 `pdf2zh-<version>-win64.zip` 에 비해 리소스 파일 (예: 폰트 및 모델) 을 포함하고 있습니다.
> - 리소스가 없는 버전도 실행 시 동적으로 리소스를 다운로드하지만, 네트워크 문제로 인해 다운로드가 실패할 수 있습니다.

***2 단계*** | `pdf2zh-<version>-with-assets-win64.zip` 파일의 압축을 풀고 `pdf2zh` 폴더로 이동합니다. 압축 해제에는 시간이 소요될 수 있으니 기다려 주세요.

***3 단계*** | `pdf2zh` 폴더로 이동한 후 `pdf2zh.exe` 파일을 더블클릭합니다.

> [!TIP]
> **.exe 파일 실행 불가**
>
> pdf2zh.exe 실행에 문제가 있는 경우, `https://aka.ms/vs/17/release/vc_redist.x64.exe` 를 설치한 후 다시 시도해 주세요.

***4 단계*** | exe 파일을 더블 클릭한 후 터미널이 팝업됩니다. 약 30 초에서 1 분 후 기본 브라우저에서 웹페이지가 열립니다. 이렇게 되지 않으면 `http://localhost:7860/` 에 수동으로 접속해 볼 수 있습니다.

> [!NOTE]
>
> WebUI 사용 중 문제가 발생하면 [이 웹페이지](./USAGE_webui.md) 를 참조하세요.

***5 단계*** | 즐기세요!

> [!TIP]
> **.exe 파일을 명령줄에서 사용할 수 있습니다**
>
> 다음과 같이 명령줄을 통해 .exe 파일을 사용하세요:
>
> - 터미널을 실행하고 .exe 파일이 있는 폴더로 이동합니다:
>
> ```bash
> cd /path/pdf2zh_next/build
> ```
>
> - .exe 파일을 호출합니다:
>
> ```bash
> ./pdf2zh_next.exe "document.pdf"
> ```
>
> 다른 명령줄 매개변수도 정상적으로 사용할 수 있습니다:
>
> ```bash
> ./pdf2zh_next.exe "document.pdf" --lang-in en --lang-out ja
> ```
>
> 명령줄 사용법에 대한 더 많은 정보가 필요하다면, 이 문서를 참조하세요.

<div align="right"> 
<h6><small>이 페이지의 일부 내용은 GPT 에 의해 번역되었으며 오류가 포함될 수 있습니다.</small></h6>