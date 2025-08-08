[**開始**](./getting-started.md) > **インストール** > **uv** _(現在)_

---

### uv 経由で PDFMathTranslate をインストール

#### uv とは？インストール方法は？

uv は Python のパッケージマネージャーで、高速で信頼性の高い依存関係解決を提供します。インストール方法は以下の通りです：

1. **pip を使用してインストール**：
   ```bash
   pip install uv
   ```

2. **conda を使用してインストール**（conda 環境の場合）：
   ```bash
   conda install -c conda-forge uv
   ```

3. **直接ダウンロード**：
   [公式サイト](https://uv.pm/) からお使いの OS に合ったバージョンをダウンロードしてインストールできます。

インストール後、以下のコマンドでバージョンを確認できます：
```bash
uv --version
```

uv は Rust で書かれた非常に高速な Python パッケージおよびプロジェクトマネージャーです。
<br>
uv をコンピュータにインストールするには、[この記事](https://docs.astral.sh/uv/getting-started/installation/) を参照してください。

---

#### インストール

1. Python がインストールされていること（3.10 <= バージョン <= 3.12）；

2. 以下のコマンドを使用してパッケージをインストールします：

    ```bash
    pip install uv
    uv tool install --python 3.12 pdf2zh-next
    ```

インストール後、**コマンドライン**または **WebUI** を介して翻訳を開始できます。

!!! Warning

    `command not found: pdf2zh_next` というエラーが表示された場合、以下のように環境変数を設定して再度お試しください：

    === "macOS と Linux"

        ~/.zshrc に以下を追加：

        ```console
        export PATH="$PATH:/Users/Username/.local/bin"
        ```

        その後、ターミナルを再起動

    === "Windows"

        PowerShell で以下を入力：

        ```powershell
        $env:Path = "C:\Users\Username\.local\bin;$env:Path"
        ```

        その後、ターミナルを再起動

> [!NOTE]
> WebUI の使用中に問題が発生した場合は、[使い方 --> WebUI](./USAGE_webui.md) を参照してください。

> [!NOTE]
> コマンドラインの使用中に問題が発生した場合は、[使い方 --> コマンドライン](./USAGE_commandline.md) を参照してください。

<div align="right"> 
<h6><small>このページの一部のコンテンツは GPT によって翻訳されており、エラーが含まれている可能性があります。</small></h6>