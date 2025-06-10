[**快速开始**](./getting-started.md) > **如何安装** > **uv** _(当前页面)_

---

### 通过 uv 安装 PDFMathTranslate

#### 什么是 uv？如何安装它？

uv 是一个非常快速的 Python 包和项目管理器，用 Rust 编写。
<br>
要安装 uv 到您的计算机，请参阅 [此文章](https://docs.astral.sh/uv/getting-started/installation/)。

---

#### 安装

1. 确保 Python 已安装 (3.10 <= 版本 <= 3.13);

2. 使用以下命令使用我们的包：

    ```bash
    pip install uv
    uv tool install --python 3.13 pdf2zh-next
    ```


!!! Warning

    如果您在运行时提示 `command not found: pdf2zh_next`，请按下面的方法配置环境变量并重试：

    === "macOS and Linux"

        请在 `~/.zshrc` 中追加:

        ```console
        export PATH="$PATH:/Users/Username/.local/bin"
        ```

        之后重启终端

    === "Windows"

        在 PowerShell 中输入:

        ```powershell
        $env:Path = "C:\Users\Username\.local\bin;$env:Path"
        ```

        之后重启 Powershell


安装后，您可以通过 **命令行** 或 **WebUI** 开始翻译。

> [!NOTE]
> 如果您在使用 WebUI 时遇到任何问题，请参阅 [使用 --> WebUI](./USAGE_webui.md)。

> [!NOTE]
> 如果您在使用命令行时遇到任何问题，请参阅 [使用 --> 命令行](./USAGE_commandline.md)。

<div align="right">
<h6><small>此页面部分内容由 GPT 翻译，可能包含错误。</small></h6>