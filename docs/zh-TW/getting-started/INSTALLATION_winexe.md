[**開始使用**](./getting-started.md) > **如何安裝** > **Windows EXE** _(current)_

---

### 透過 .exe 檔案安裝 PDFMathTranslate

***步驟 1*** | 從 [發佈頁面](https://github.com/PDFMathTranslate/PDFMathTranslate-next/releases) 下載 `pdf2zh-<version>-with-assets-win64.zip`。

> [!TIP]
> **`pdf2zh-<version>-with-assets-win64.zip` 和 `pdf2zh-<version>-win64.zip` 有什麼區別？**
>
> - 如果您是首次下載並使用 PDFMathTranslate，建議下載 `pdf2zh-<version>-with-assets-win64.zip`。
> - 與 `pdf2zh-<version>-win64.zip` 相比，`pdf2zh-<version>-with-assets-win64.zip` 包含了資源文件（如字體和模型）。
> - 不包含資源的版本在運行時也會動態下載資源，但可能因網絡問題導致下載失敗。

***步驟 2*** | 解壓縮 `pdf2zh-<version>-with-assets-win64.zip` 並進入 `pdf2zh` 資料夾。解壓縮需要一些時間，請耐心等待。

***步驟 3*** | 進入 `pdf2zh` 資料夾，然後雙擊 `pdf2zh.exe`。

> [!TIP]
> **無法執行 .exe 檔案**
>
> 如果您在執行 pdf2zh.exe 時遇到問題，請安裝 `https://aka.ms/vs/17/release/vc_redist.x64.exe` 後再試一次。

***步驟 4*** | 雙擊 exe 檔案後，終端機將會彈出。大約半分鐘到一分鐘後，您的預設瀏覽器將會開啟一個網頁。如果沒有發生，您可以嘗試手動訪問 `http://localhost:7860/`。

> [!NOTE]
>
> 如果在使用 WebUI 時遇到任何問題，請參考[此網頁](./USAGE_webui.md)。

***步驟 5*** | 開始使用！

> [!TIP]
> **您可以透過命令行使用 .exe 檔案**
>
> 透過命令行使用 .exe 檔案的方法如下：
>
> - 開啟終端機並導航至包含 .exe 檔案的資料夾：
>
> ```bash
> cd /path/pdf2zh_next/build
> ```
>
> - 呼叫 .exe 檔案：
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
> 如需更多關於命令行使用的資訊，請參考此文章。

<div align="right"> 
<h6><small>Some content on this page has been translated by GPT and may contain errors.</small></h6>