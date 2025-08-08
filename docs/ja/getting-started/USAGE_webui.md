[**開始**](./getting-started.md) > **インストール** > **WebUI** _(現在)_

---

### Webui で PDFMathTranslate を使用する

#### WebUI ページを開く方法：

WebUI インターフェースを開く方法はいくつかあります。**Windows** を使用している場合は、[この記事](./INSTALLATION_winexe.md) を参照してください。

1. Python がインストールされていること（3.10 <= バージョン <= 3.12）

2. パッケージをインストール：

3. ブラウザで使用開始：

    ```bash
    pdf2zh_next --gui
    ```

4. ブラウザが自動的に起動しない場合は、以下にアクセス：

    ```bash
    http://localhost:7860/
    ```

    `PDF` ファイルをウィンドウにドロップして、`Translate` をクリックしてください。

<!-- <img src="./images/gui.gif" width="500"/> -->
<img src='./../images/gui.gif' width="500"/>

### 環境変数

ソース言語とターゲット言語は環境変数を使用して設定できます：

- `PDF2ZH_LANG_FROM`: ソース言語を設定します。デフォルトは「English」です。
- `PDF2ZH_LANG_TO`: ターゲット言語を設定します。デフォルトは「Simplified Chinese」です。

## プレビュー

<img src="./../images/before.png" width="500"/>
<img src="./../images/after.png" width="500"/>

## メンテナンス

[Rongxin](https://github.com/reycn) がメンテナンスする GUI

<div align="right"> 
<h6><small>このページの一部のコンテンツは GPT によって翻訳されており、エラーが含まれている可能性があります。</small></h6>