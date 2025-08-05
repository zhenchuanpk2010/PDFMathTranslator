[**開始**](./getting-started.md) > **インストール** > **uv** _(現在)_

---

### uv 経由で PDFMathTranslate をインストール

#### uv とは何ですか？インストール方法は？

`uv` は Python パッケージマネージャーで、`pip` や `conda` の代替として設計されています。高速で信頼性が高く、依存関係の解決が優れていることが特徴です。

**インストール方法：**

1. **Python 3.8 以上**がインストールされていることを確認してください。
2. 以下のコマンドを実行して `uv` をインストールします：

```bash
pip install uv
```

または、最新バージョンを直接インストールする場合は：

```bash
pip install --upgrade uv
```

3. インストールが完了したら、以下のコマンドでバージョンを確認できます：

```bash
uv --version
```

これで `uv` がシステムにインストールされ、使用できるようになります。

uv は Rust で書かれた非常に高速な Python パッケージおよびプロジェクトマネージャーです。
<br>
コンピューターに uv をインストールするには、[この記事](https://docs.astral.sh/uv/getting-started/installation/)を参照してください。

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

    `command not found: pdf2zh_next` というエラーが表示された場合、以下のように環境変数を設定して再度試してください:

    === "macOS と Linux"

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
> WebUI の使用中に問題が発生した場合は、[使い方 --> WebUI](./USAGE_webui.md) を参照してください。

> [!NOTE]
> コマンドラインの使用中に問題が発生した場合は、[使い方 --> コマンドライン](./USAGE_commandline.md) を参照してください。

<div align="right"> 
<h6><small>このページの一部のコンテンツは GPT によって翻訳されており、エラーが含まれている可能性があります。</small></h6>