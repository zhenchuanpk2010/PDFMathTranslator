[**開始**](./getting-started.md) > **インストール** > **Docker** _(現在)_

---

### PDFMathTranslateをdockerでインストール

#### Dockerとは何ですか？

[Docker](https://docs.docker.com/get-started/docker-overview/) は、アプリケーションの開発、配布、実行のためのオープンプラットフォームです。Dockerを使用すると、アプリケーションをインフラストラクチャから分離できるため、ソフトウェアを迅速に提供できます。Dockerでは、アプリケーションを管理するのと同じ方法でインフラストラクチャを管理できます。Dockerのコード配布、テスト、デプロイの方法論を活用することで、コードの記述から本番環境での実行までの遅延を大幅に削減できます。

#### インストール

<h4>1. プルして実行:</h4>

```bash
docker pull awwaawwa/pdfmathtranslate-next
docker run -d -p 7860:7860 awwaawwa/pdfmathtranslate-next
```

> [!NOTE]
> 
> - Docker Hubにアクセスできない場合は、[GitHub Container Registry](https://github.com/PDFMathTranslate/PDFMathTranslate-next/pkgs/container/pdfmathtranslate)上のイメージを試してください。
> 
> ```bash
> docker pull ghcr.io/PDFMathTranslate/PDFMathTranslate-next
> docker run -d -p 7860:7860 ghcr.io/PDFMathTranslate/PDFMathTranslate-next
> ```

<h4>2. デフォルトのブラウザでこのURLを入力してWebUIページを開きます:</h4>

```
http://localhost:7860/
```

> [!NOTE]
> WebUIの使用中に問題が発生した場合は、[使い方 --> WebUI](./USAGE_webui.md)を参照してください。

> [!NOTE]
> コマンドラインの使用中に問題が発生した場合は、[使い方 --> コマンドライン](./USAGE_commandline.md)を参照してください。

<!-- 
#### クラウドサービスでのDockerデプロイの場合:

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
<h6><small>このページの一部のコンテンツはGPTによって翻訳されており、エラーが含まれている可能性があります。</small></h6>