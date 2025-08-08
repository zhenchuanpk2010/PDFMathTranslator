[**시작하기**](./getting-started.md) > **설치** > **Docker** _(현재)_

---

### docker 를 통해 PDFMathTranslate 설치하기

#### Docker 란 무엇인가?

[Docker](https://docs.docker.com/get-started/docker-overview/) 는 애플리케이션을 개발, 배송 및 실행하기 위한 오픈 플랫폼입니다. Docker 를 사용하면 인프라에서 애플리케이션을 분리하여 소프트웨어를 빠르게 제공할 수 있습니다. Docker 를 사용하면 애플리케이션을 관리하는 것과 같은 방식으로 인프라를 관리할 수 있습니다. Docker 의 코드 배송, 테스트 및 배포 방법론을 활용하면 코드 작성과 프로덕션 환경에서 실행 사이의 지연을 크게 줄일 수 있습니다.

#### 설치

<h4>1. 풀하고 실행하기:</h4>

```bash
docker pull awwaawwa/pdfmathtranslate-next
docker run -d -p 7860:7860 awwaawwa/pdfmathtranslate-next
```

> [!NOTE]
> 
> - Docker Hub 에 접근할 수 없는 경우, [GitHub Container Registry](https://github.com/PDFMathTranslate/PDFMathTranslate-next/pkgs/container/pdfmathtranslate) 의 이미지를 사용해 보세요.
> 
> ```bash
> docker pull ghcr.io/PDFMathTranslate/PDFMathTranslate-next
> docker run -d -p 7860:7860 ghcr.io/PDFMathTranslate/PDFMathTranslate-next
> ```

<h4>2. 기본 브라우저에서 이 URL 을 입력하여 WebUI 페이지를 엽니다:</h4>

```
http://localhost:7860/
```

> [!NOTE]
> WebUI 사용 중 문제가 발생하면 [사용법 --> WebUI](./USAGE_webui.md) 를 참조하세요.

> [!NOTE]
> 명령줄 사용 중 문제가 발생하면 [사용법 --> Command Line](./USAGE_commandline.md) 를 참조하세요.
<!-- 
#### For docker deployment on cloud service:

<div>
<a href="https://www.heroku.com/deploy?template=https://github.com/PDFMathTranslate/PDFMathTranslate-next">
  <img src="https://www.herokucdn.com/deploy/button.svg" alt="Deploy" height="26"></a>
<a href="https://render.com/deploy">
  <img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Koyeb" height="26"></a>
<a href="https://zeabur.com/templates/5FQIGX?referralCode=reycn">
  <img src="https://zeabur.com/button.svg" alt="Deploy on Zeabur" height="26"></a>
<a href="https://app.koyeb.com/deploy?type=git&builder=buildpack&repository=github.com/PDFMathTranslate/PDFMathTranslate-next&branch=main&name=pdf-math-translate">
  <img src="https://www.koyeb.com/static/images/deploy/button.svg" alt="Deploy to Koyeb" height="26"></a>
</div>

-->

<div align="right"> 
<h6><small>이 페이지의 일부 내용은 GPT 에 의해 번역되었으며 오류가 포함될 수 있습니다.</small></h6>