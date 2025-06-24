[**快速开始**](./getting-started.md) > **如何安装** > **Windows EXE** _(当前页面)_

---

### 通过 .exe 文件安装 PDFMathTranslate

***Step 1*** | 从 [发布页面](https://github.com/PDFMathTranslate/PDFMathTranslate-next/releases) 下载 `pdf2zh-<version>-with-assets-win64.zip`。

> [!TIP]
> **`pdf2zh-<version>-with-assets-win64.zip` 和 `pdf2zh-<version>-win64.zip` 有什么区别？**
>
> - 如果您是第一次下载和使用 PDFMathTranslate，建议下载 `pdf2zh-<version>-with-assets-win64.zip`。
> - `pdf2zh-<version>-with-assets-win64.zip` 包含资源文件（例如字体和模型），而 `pdf2zh-<version>-win64.zip` 不包含。
> - 没有资产的版本在运行时也会动态下载资源，但由于网络问题，下载可能会失败。

***Step 2*** | 解压 `pdf2zh-<version>-with-assets-win64.zip` 并导航到 `pdf2zh` 文件夹。解压需要一段时间，请耐心等待。

***Step 3*** | 导航到 `pdf2zh` 文件夹，然后双击 `pdf2zh.exe`。
>
> 如果您在运行 pdf2zh.exe 时遇到问题，请安装 `https://aka.ms/vs/17/release/vc_redist.x64.exe` 并重试。

***Step 4*** | 双击 exe 文件后，将弹出一个终端。大约半分钟后，您的默认浏览器将打开一个网页。如果未发生，您可以尝试手动访问 `http://localhost:7860/`。

> [!NOTE]
> 如果您在使用 WebUI 时遇到任何问题，请参阅 [使用 --> WebUI](./USAGE_webui.md)。

***Step 5*** | 享受！

> [!TIP]
> **您可以通过命令行使用 .exe 文件**
>
> 通过命令行使用 .exe 文件如下：
>
> - 启动您的终端并导航到包含 .exe 文件的文件夹：
>
> ```bash
> cd /path/pdf2zh_next/build
> ```
>
> - 调用 .exe 文件：
>
> ```bash
> ./pdf2zh_next.exe "document.pdf"
> ```
>
> 您还可以使用其他命令行参数：
>
> ```bash
> ./pdf2zh_next.exe "document.pdf" --lang-in en --lang-out ja
> ```
>
> 如果您需要更多关于命令行使用的信息，请参阅此文章。

<div align="right">
<h6><small>此页面部分内容由 GPT 翻译，可能包含错误。</small></h6>