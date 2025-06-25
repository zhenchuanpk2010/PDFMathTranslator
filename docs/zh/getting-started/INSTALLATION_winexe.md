[**开始使用**](./getting-started.md) > **如何安装** > **Windows EXE** _(当前)_

---

### 通过 .exe 文件安装 PDFMathTranslate

***步骤 1*** | 从[发布页面](https://github.com/PDFMathTranslate/PDFMathTranslate-next/releases)下载 `pdf2zh-<version>-with-assets-win64.zip`。

> [!TIP]
> **`pdf2zh-<version>-with-assets-win64.zip` 和 `pdf2zh-<version>-win64.zip` 有什么区别？**
>
> - 如果您是首次下载并使用 PDFMathTranslate，建议下载 `pdf2zh-<version>-with-assets-win64.zip`。
> - 与 `pdf2zh-<version>-win64.zip` 相比，`pdf2zh-<version>-with-assets-win64.zip` 包含了资源文件（如字体和模型）。
> - 不含资源的版本在运行时也会动态下载资源，但由于网络问题可能导致下载失败。

***步骤 2*** | 解压 `pdf2zh-<version>-with-assets-win64.zip` 并进入 `pdf2zh` 文件夹。解压需要一些时间，请耐心等待。

***步骤 3*** | 进入 `pdf2zh` 文件夹，然后双击 `pdf2zh.exe`。

> [!TIP]
> **无法运行.exe 文件**
>
> 如果在运行 pdf2zh.exe 时遇到问题，请安装 `https://aka.ms/vs/17/release/vc_redist.x64.exe` 后重试。

***步骤 4*** | 双击 exe 文件后终端窗口将弹出。约半分钟至一分钟后，默认浏览器会自动打开网页。若未自动跳转，可手动访问 `http://localhost:7860/`。

> [!NOTE]
>
> 如果在使用 WebUI 时遇到任何问题，请参考[此网页](./USAGE_webui.md)。

***步骤 5*** | 尽情享用！

> [!TIP]
> **您可以通过命令行使用 .exe 文件**
>
> 通过命令行使用 .exe 文件的方法如下：
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
> 您可以正常使用其他命令行参数：
>
> ```bash
> ./pdf2zh_next.exe "document.pdf" --lang-in en --lang-out ja
> ```
>
> 如需了解更多关于命令行使用的信息，请参阅此文章。

<div align="right"> 
<h6><small>本页面的部分内容由 GPT 翻译，可能包含错误。</small></h6>