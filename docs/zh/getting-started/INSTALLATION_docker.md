[**快速开始**](./getting-started.md) > **如何安装** > **Docker** _(当前页面)_

---

### 通过 Docker 安装 PDFMathTranslate

#### 什么是 Docker？

[Docker](https://docs.docker.com/get-started/docker-overview/) 是一个开放的平台，用于开发、交付和运行应用程序。Docker 使您能够将应用程序与基础设施分离，以便快速交付软件。使用 Docker，您可以以与管理应用程序相同的方式管理基础设施。通过利用 Docker 的交付、测试和部署代码的方法，您可以显著减少从编写代码到在生产中运行的时间。

#### 安装

<h4>1. 拉取并运行：</h4>

```bash
docker pull awwaawwa/pdfmathtranslate-next
docker run -d -p 7860:7860 awwaawwa/pdfmathtranslate-next
```

> [!NOTE]
>
> - 如果您无法访问 Docker Hub，请尝试 [GitHub Container Registry](https://github.com/PDFMathTranslate/PDFMathTranslate-next/pkgs/container/pdfmathtranslate) 上的镜像。
>
> ```bash
> docker pull ghcr.io/PDFMathTranslate/PDFMathTranslate-next
> docker run -d -p 7860:7860 ghcr.io/PDFMathTranslate/PDFMathTranslate-next
> ```

<h4>2. 在您的默认浏览器中输入此 URL 以打开 WebUI 页面：</h4>

```
http://localhost:7860/
```

> [!NOTE]
> 如果您在使用 WebUI 时遇到任何问题，请参阅 [使用 --> WebUI](./USAGE_webui.md)。

> [!NOTE]
> 如果您在使用命令行时遇到任何问题，请参阅 [使用 --> 命令行](./USAGE_commandline.md)。
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

<div align="right">
<h6><small>Some content on this page has been translated by GPT and may contain errors.</small></h6> -->