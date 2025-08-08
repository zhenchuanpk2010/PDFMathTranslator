[**开始使用**](./getting-started.md) > **如何安装** > **Docker** _(当前)_

---

### 通过 docker 安装 PDFMathTranslate

#### 什么是 docker？

[Docker](https://docs.docker.com/get-started/docker-overview/) 是一个用于开发、运输和运行应用程序的开放平台。Docker 使您能够将应用程序与基础设施分离，从而可以快速交付软件。通过 Docker，您可以用管理应用程序的方式来管理基础设施。利用 Docker 的代码运输、测试和部署方法，您可以显著减少编写代码与在生产环境中运行代码之间的延迟。

#### 如何安装

<h4>1. 拉取并运行：</h4>

```bash
docker pull awwaawwa/pdfmathtranslate-next
docker run -d -p 7860:7860 awwaawwa/pdfmathtranslate-next
```

> [!NOTE]
> 
> - 如果无法访问 Docker Hub，请尝试使用 [GitHub Container Registry](https://github.com/PDFMathTranslate/PDFMathTranslate-next/pkgs/container/pdfmathtranslate) 上的镜像。
> 
> ```bash
> docker pull ghcr.io/PDFMathTranslate/PDFMathTranslate-next
> docker run -d -p 7860:7860 ghcr.io/PDFMathTranslate/PDFMathTranslate-next
> ```

<h4>2. 在默认浏览器中输入此 URL 以打开 WebUI 页面：</h4>

```
http://localhost:7860/
```

> [!NOTE]
> 如果在使用 WebUI 时遇到任何问题，请参考 [如何使用 --> WebUI](./USAGE_webui.md)。

> [!NOTE]
> 如果在使用命令行时遇到任何问题，请参考 [如何使用 --> 命令行](./USAGE_commandline.md)。
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
<h6><small>本页面的部分内容由 GPT 翻译，可能包含错误。</small></h6>