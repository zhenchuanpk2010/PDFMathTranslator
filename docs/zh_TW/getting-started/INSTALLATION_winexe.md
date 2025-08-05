[**開始使用**](./getting-started.md) > **如何安裝** > **Windows EXE** _(current)_

---

### 透過 .exe 文件安裝 PDFMathTranslate

***步驟 1*** | 從 [release page](https://github.com/PDFMathTranslate/PDFMathTranslate-next/releases) 下載 `pdf2zh-<version>-with-assets-win64.zip`。

> [!TIP]
> **`pdf2zh-<version>-with-assets-win64.zip` 和 `pdf2zh-<version>-win64.zip` 有什麼區別？**
>
> - 如果你是第一次下載並使用 PDFMathTranslate，建議下載 `pdf2zh-<version>-with-assets-win64.zip`。
> - 與 `pdf2zh-<version>-win64.zip` 相比，`pdf2zh-<version>-with-assets-win64.zip` 包含了資源文件（例如字體和模型）。
> - 不包含資源的版本在運行時也會動態下載資源，但由於網絡問題可能會導致下載失敗。

***步驟 2*** | 解壓縮 `pdf2zh-<version>-with-assets-win64.zip` 並進入 `pdf2zh` 資料夾。解壓縮需要一些時間，請耐心等待。

***步驟 3*** | 進入 `pdf2zh` 資料夾，然後雙擊 `pdf2zh.exe`。

> [!TIP]
> **無法執行 .exe 文件**
>
> 如果您在執行 pdf2zh.exe 時遇到問題，請安裝 `https://aka.ms/vs/17/release/vc_redist.x64.exe` 後再試一次。

***步驟 4*** | 雙擊 exe 文件後會彈出終端。大約半分鐘到一分鐘後，您的默認瀏覽器會打開一個網頁。如果沒有發生這種情況，您可以嘗試手動訪問 `http://localhost:7860/`。

> [!NOTE]
>
> 如果在使用 WebUI 時遇到任何問題，請參考[此網頁](./USAGE_webui.md)。

***步驟 5*** | 開始使用！

> [!TIP]
> **您可以透過命令行使用 .exe 文件**
>
> 透過命令行使用 .exe 文件的方法如下：
>
> - 打開終端機並導航至包含 .exe 文件的資料夾：
>
> ```bash
> cd /path/pdf2zh_next/build
> ```
>
> - 呼叫 .exe 文件：
>
> ```bash
> ./pdf2zh_next.exe "document.pdf"
> ```
>
> 您可以正常使用其他命令行參數：
>
> ```bash
> ./pdf2zh_next.exe "document.pdf" --lang-in en --lang-out ja
> ```
>
> 如需更多關於命令行使用的資訊，請參考這篇文章。

<div align="right"> 
<h6><small>Some content on this page has been translated by GPT and may contain errors.</small></h6>