[**开始使用**](./getting-started.md) > **如何安装** > **uv** _(current)_

---

### 通过 uv 安装 PDFMathTranslate

#### 什么是 uv？如何安装它？

uv 是一个用 Rust 编写的极速 Python 包和项目管理器。
<br>
要在您的计算机上安装 uv，请参考[这篇文章](https://docs.astral.sh/uv/getting-started/installation/)。

---

#### 如何安装

1. 已安装 Python（3.10 <= 版本 <= 3.13）；

2. 使用以下命令安装我们的包：

    ```bash
    pip install uv
    uv tool install --python 3.13 pdf2zh-next
    ```

安装完成后，您可以通过**命令行**或**WebUI**开始翻译。

!!! Warning

    如果在运行时看到错误 `command not found: pdf2zh_next`，请按以下方式配置环境变量后重试：

    === "macOS and Linux"

        将以下内容添加到 ~/.zshrc 文件中：

        ```console
        export PATH="$PATH:/Users/Username/.local/bin"
        ```

        然后重启终端

    === "Windows"

        在 PowerShell 中输入以下命令：

        ```powershell
        $env:Path = "C:\Users\Username\.local\bin;$env:Path"
        ```

        然后重启终端

> [!NOTE]
> 如果在使用 WebUI 过程中遇到任何问题，请参考[如何使用 --> WebUI](./USAGE_webui.md)。

> [!NOTE]
> 如果在使用命令行过程中遇到任何问题，请参考[如何使用 --> 命令行](./USAGE_commandline.md)。

<div align="right"> 
<h6><small>本页面的部分内容由 GPT 翻译，可能包含错误。</small></h6>