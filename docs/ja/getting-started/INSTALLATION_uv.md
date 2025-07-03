[**始め方**](./始め方.md) > **インストール** > **uv** _(current)_

---

### uv 経由で PDFMathTranslate をインストール

#### uv とは何ですか？インストール方法は？

uv は Rust で書かれた非常に高速な Python パッケージおよびプロジェクトマネージャーです。
<br>
uv をコンピュータにインストールするには、[この記事](https://docs.astral.sh/uv/getting-started/installation/)を参照してください。

---

#### インストール

1. Python がインストールされていること（3.10 <= バージョン <= 3.13）;

2. 以下のコマンドを使用してパッケージを利用します：

    ```bash
    pip install uv
    uv tool install --python 3.13 pdf2zh-next
    ```

インストール後、**コマンドライン**または**WebUI**を介して翻訳を開始できます。

!!! Warning

    `command not found: pdf2zh_next` というエラーが表示された場合、以下のように環境変数を設定して再度試してください:

    === "macOS and Linux"

        ~/.zshrc に以下を追加:

        ```console
        export PATH="$PATH:/Users/Username/.local/bin"
        ```

        その後、ターミナルを再起動

    === "Windows"

        PowerShell で以下を入力:

        ```powershell
        $env:Path = "C:\Users\Username\.local\bin;$env:Path"
        ```

        その後、ターミナルを再起動

> [!NOTE]
> WebUI 使用中に問題が発生した場合は、[使い方 --> WebUI](./USAGE_webui.md)を参照してください。

> [!NOTE]
> コマンドライン使用中に問題が発生した場合は、[使い方 --> コマンドライン](./USAGE_commandline.md)を参照してください。

<div align="right"> 
<h6><small>このページの一部のコンテンツは GPT によって翻訳されており、エラーが含まれている可能性があります。</small></h6>