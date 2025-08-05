[**開始**](./getting-started.md) > **インストール** > **uv** _(現在)_

---

### uv 経由で PDFMathTranslate をインストール

#### uv とは何ですか？ インストール方法は？

uv は Python のパッケージマネージャーで、`pip` や `pip-tools` の代替として高速で効率的なパッケージ管理を提供します。インストール方法は以下の通りです：

1. **Python のインストール**: uv を使用するには Python 3.7 以降が必要です。まだインストールしていない場合は、[Python 公式サイト](https://www.python.org/downloads/) からダウンロードしてください。

2. **uv のインストール**: 以下のコマンドを実行して uv をインストールします：
   ```bash
   pip install uv
   ```

3. **動作確認**: インストールが完了したら、以下のコマンドでバージョンを確認します：
   ```bash
   uv --version
   ```

これで uv が使用可能になります。`pip` と同じように `uv pip install パッケージ名` でパッケージをインストールできますが、より高速に動作します。

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

インストール後、**コマンドライン**または **WebUI** 経由で翻訳を開始できます。

!!! Warning

    `command not found: pdf2zh_next` というエラーが表示された場合、以下の手順で環境変数を設定して再度お試しください：

    === "macOS および Linux"

        ~/.zshrc に以下を追加：

        ```console
        export PATH="$PATH:/Users/Username/.local/bin"
        ```

        その後、ターミナルを再起動

    === "Windows"

        PowerShell で以下を実行：

        ```powershell
        $env:Path = "C:\Users\Username\.local\bin;$env:Path"
        ```

        その後、ターミナルを再起動

> [!NOTE]
> WebUI の使用中に問題が発生した場合は、[使い方 --> WebUI](./USAGE_webui.md) を参照してください。

> [!NOTE]
> コマンドラインの使用中に問題が発生した場合は、[使い方 --> コマンドライン](./USAGE_commandline.md) を参照してください。

<div align="right"> 
<h6><small>このページの一部のコンテンツはGPTによって翻訳されており、エラーが含まれている可能性があります。</small></h6>