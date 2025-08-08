[**開始使用**](./getting-started.md) > **如何安裝** > **Docker** _(current)_

---

### 透過 docker 安裝 PDFMathTranslate

#### 什麼是 docker？

[Docker](https://docs.docker.com/get-started/docker-overview/) 是一個用於開發、運送和運行應用程式的開放平台。Docker 能讓您將應用程式與基礎架構分離，從而快速交付軟體。透過 Docker，您可以用管理應用程式的相同方式來管理基礎架構。藉由利用 Docker 的運送、測試和部署程式碼方法論，您可以大幅縮短編寫程式碼與在生產環境中運行它之間的延遲。

#### 如何安裝

<h4>1. 拉取並執行：</h4>

```bash
docker pull awwaawwa/pdfmathtranslate-next
docker run -d -p 7860:7860 awwaawwa/pdfmathtranslate-next
```

> [!NOTE]
> 
> - 如果您無法存取 Docker Hub，請嘗試使用 [GitHub Container Registry](https://github.com/PDFMathTranslate/PDFMathTranslate-next/pkgs/container/pdfmathtranslate) 上的映像檔。
> 
> ```bash
> docker pull ghcr.io/PDFMathTranslate/PDFMathTranslate-next
> docker run -d -p 7860:7860 ghcr.io/PDFMathTranslate/PDFMathTranslate-next
> ```

<h4>2. 在您的預設瀏覽器中輸入此 URL 以開啟 WebUI 頁面：</h4>

```
http://localhost:7860/
```

> [!NOTE]
> 如果在使用 WebUI 時遇到任何問題，請參考 [如何使用 --> WebUI](./USAGE_webui.md)。

> [!NOTE]
> 如果在使用命令行時遇到任何問題，請參考 [如何使用 --> 命令行](./USAGE_commandline.md)。
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
<h6><small>Some content on this page has been translated by GPT and may contain errors.</small></h6>