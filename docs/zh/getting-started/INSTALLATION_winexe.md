[**开始使用**](./getting-started.md) > **如何安装** > **Windows EXE** _(current)_

---

### 通过 .exe 文件安装 PDFMathTranslate

***步骤 1*** | 从 [release page](https://github.com/PDFMathTranslate/PDFMathTranslate-next/releases) 下载 `pdf2zh-<version>-with-assets-win64.zip`。

> [!TIP]
> **`pdf2zh-<version>-with-assets-win64.zip` 和 `pdf2zh-<version>-win64.zip` 有什么区别？**
>
> - 如果你是首次下载并使用 PDFMathTranslate，建议下载 `pdf2zh-<version>-with-assets-win64.zip`。
> - 相比 `pdf2zh-<version>-win64.zip`，`pdf2zh-<version>-with-assets-win64.zip` 包含了资源文件（如字体和模型）。
> - 不含资源的版本在运行时也会动态下载资源，但可能会因网络问题导致下载失败。

***步骤 2*** | 解压 `pdf2zh-<version>-with-assets-win64.zip` 并进入 `pdf2zh` 文件夹。解压需要一些时间，请耐心等待。

***步骤 3*** | 进入 `pdf2zh` 文件夹，然后双击 `pdf2zh.exe`。

> [!TIP]
> **无法运行 .exe 文件**
>
> 如果您在运行 pdf2zh.exe 时遇到问题，请安装 `https://aka.ms/vs/17/release/vc_redist.x64.exe` 后重试。

***步骤 4*** | 双击 exe 文件后，终端窗口会弹出。大约半分钟到一分钟后，默认浏览器会打开一个网页。如果未自动打开，可以尝试手动访问 `http://localhost:7860/`。

> [!NOTE]
>
> 如果在使用 WebUI 过程中遇到任何问题，请参考 [此网页](./USAGE_webui.md)。

***步骤 5*** | 尽情享受吧！

> [!TIP]
> **你可以通过命令行使用 .exe 文件**
>
> 通过命令行使用 .exe 文件的步骤如下：
>
> - 打开终端并导航至包含 .exe 文件的文件夹：
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
> 你可以正常使用其他命令行参数：
>
> ```bash
> ./pdf2zh_next.exe "document.pdf" --lang-in en --lang-out ja
> ```
>
> 如需了解更多关于命令行使用的信息，请参考这篇文章。

<div align="right"> 
<h6><small>本页面的部分内容由 GPT 翻译，可能包含错误。</small></h6>