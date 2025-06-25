[**開始**](./getting-started.md) > **インストール** > **WebUI** _(現在のページ)_

---

### Webui で PDFMathTranslate を使用する

#### WebUIページを開く方法:

WebUIインターフェースを開く方法はいくつかあります。**Windows**を使用している場合は、[この記事](./INSTALLATION_winexe.md)を参照してください。

1. Pythonがインストールされていること（3.10 <= バージョン <= 3.13）

2. パッケージをインストール:

3. ブラウザで使い始める:

    ```bash
    pdf2zh_next --gui
    ```

4. ブラウザが自動的に起動しない場合は、次のURLにアクセスしてください。

    ```bash
    http://localhost:7860/
    ```

    PDFファイルをウィンドウにドロップし、`Translate`をクリックします。

<!-- <img src="./images/gui.gif" width="500"/> -->
<img src='./../images/gui.gif' width="500"/>

### 環境変数

ソース言語とターゲット言語は環境変数を使用して設定できます:

- `PDF2ZH_LANG_FROM`: ソース言語を設定します。デフォルトは「English」です。
- `PDF2ZH_LANG_TO`: ターゲット言語を設定します。デフォルトは「Simplified Chinese」です。

## プレビュー

<img src="./../images/before.png" width="500"/>
<img src="./../images/after.png" width="500"/>

## メンテナンス

GUIは[Rongxin](https://github.com/reycn)によってメンテナンスされています

<div align="right"> 
<h6><small>このページの一部のコンテンツはGPTによって翻訳されており、エラーが含まれている可能性があります。</small></h6>