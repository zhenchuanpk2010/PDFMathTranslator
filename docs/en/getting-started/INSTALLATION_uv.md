[**Getting Started**](./getting-started.md) > **Installation** > **uv** _(current)_

---

### Install PDFMathTranslate via uv

#### What is uv? How to install it?

uv is an extremely fast Python package and project manager, written in Rust.
<br>
To install uv on your computer, please refer to [this article](https://docs.astral.sh/uv/getting-started/installation/).

---

#### Installation

1. Python installed (3.10 <= version <= 3.12);

2. Use the following command to use our package:

    ```bash
    pip install uv
    uv tool install --python 3.12 pdf2zh-next
    ```

After installation, you can start translation via the **command line** or **WebUI**.

!!! Warning

    If you see the error `command not found: pdf2zh_next` when running, please configure the environment variables as follows and try again:

    === "macOS and Linux"

        Add the following to your ~/.zshrc:

        ```console
        export PATH="$PATH:/Users/Username/.local/bin"
        ```

        Then restart your terminal

    === "Windows"

        Enter the following in PowerShell:

        ```powershell
        $env:Path = "C:\Users\Username\.local\bin;$env:Path"
        ```

        Then restart your terminal

> [!NOTE]
> If you encounter any issues during use WebUI, please refer to [Usage --> WebUI](./USAGE_webui.md).

> [!NOTE]
> If you encounter any issues during use command line, please refer to [Usage --> Command Line](./USAGE_commandline.md).
