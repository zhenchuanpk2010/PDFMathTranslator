[**Начало работы**](./getting-started.md) > **Установка** > **Docker** _(текущая)_

---

### Установка PDFMathTranslate через docker

#### Что такое Docker?

[Docker](https://docs.docker.com/get-started/docker-overview/) — это открытая платформа для разработки, доставки и запуска приложений. Docker позволяет отделить ваши приложения от инфраструктуры, чтобы вы могли быстро доставлять программное обеспечение. С Docker вы можете управлять своей инфраструктурой так же, как и приложениями. Используя преимущества методологий Docker для доставки, тестирования и развертывания кода, вы можете значительно сократить задержку между написанием кода и его запуском в производственной среде.

#### Установка

<h4>1. Загрузка и запуск:</h4>

```bash
docker pull awwaawwa/pdfmathtranslate-next
docker run -d -p 7860:7860 awwaawwa/pdfmathtranslate-next
```

> [!NOTE]
> 
> - Если у вас нет доступа к Docker Hub, попробуйте использовать образ на [GitHub Container Registry](https://github.com/PDFMathTranslate/PDFMathTranslate-next/pkgs/container/pdfmathtranslate).
> 
> ```bash
> docker pull ghcr.io/PDFMathTranslate/PDFMathTranslate-next
> docker run -d -p 7860:7860 ghcr.io/PDFMathTranslate/PDFMathTranslate-next
> ```

<h4>2. Введите этот URL в вашем браузере по умолчанию, чтобы открыть страницу WebUI:</h4>

```
http://localhost:7860/
```

> [!NOTE]
> Если у вас возникли проблемы при использовании WebUI, обратитесь к разделу [Использование --> WebUI](./USAGE_webui.md).

> [!NOTE]
> Если у вас возникли проблемы при использовании командной строки, обратитесь к разделу [Использование --> Командная строка](./USAGE_commandline.md).
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
<h6><small>Часть содержимого этой страницы была переведена GPT и может содержать ошибки.</small></h6>