[**快速開始**](./getting-started.md) > **如何安裝** > **uv** _(current)_

---

### 透過 uv 安裝 PDFMathTranslate

#### 什麼是 uv？如何安裝它？

uv 是一個極其快速的 Python 套件和專案管理器，使用 Rust 編寫。
<br>
要在您的電腦上安裝 uv，請參考[這篇文章](https://docs.astral.sh/uv/getting-started/installation/)。

---

#### 如何安裝

1. 已安裝 Python（版本需介於 3.10 至 3.12 之間）；

2. 使用以下命令來安裝我們的套件：

    ```bash
    pip install uv
    uv tool install --python 3.12 pdf2zh-next
    ```

安裝完成後，您可以透過**命令行**或**WebUI**開始翻譯。

!!! Warning

    如果在執行時看到錯誤 `command not found: pdf2zh_next`，請按照以下方式配置環境變量後重試：

    === "macOS 和 Linux"

        將以下內容添加到您的 ~/.zshrc 中：

        ```console
        export PATH="$PATH:/Users/Username/.local/bin"
        ```

        然後重新啟動終端

    === "Windows"

        在 PowerShell 中輸入以下內容：

        ```powershell
        $env:Path = "C:\Users\Username\.local\bin;$env:Path"
        ```

        然後重新啟動終端

> [!NOTE]
> 如果在使用 WebUI 時遇到任何問題，請參考[如何使用 --> WebUI](./USAGE_webui.md)。

> [!NOTE]
> 如果在使用命令行時遇到任何問題，請參考[如何使用 --> 命令行](./USAGE_commandline.md)。

<div align="right"> 
<h6><small>Some content on this page has been translated by GPT and may contain errors.</small></h6>