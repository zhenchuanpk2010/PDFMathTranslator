[**快速開始**](./getting-started.md) > **如何安裝** > **WebUI** _(current)_

---

### 透過 Webui 使用 PDFMathTranslate

#### 如何開啟 WebUI 頁面：

有幾種方法可以開啟 WebUI 介面。如果您使用的是 **Windows**，請參考[這篇文章](./INSTALLATION_winexe.md);

1. 已安裝 Python (版本需介於 3.10 至 3.13 之間)

2. 安裝我們的套件：

3. 在瀏覽器中開始使用：

    ```bash
    pdf2zh_next --gui
    ```

4. 若瀏覽器未自動開啟，請前往

    ```bash
    http://localhost:7860/
    ```

    將 PDF 檔案拖放至視窗中並點擊 `Translate`。

<!-- <img src="./images/gui.gif" width="500"/> -->
<img src='./../images/gui.gif' width="500"/>

### 環境變數

你可以透過環境變數設定來源與目標語言：

- `PDF2ZH_LANG_FROM`: 設定來源語言。預設為 "English"。
- `PDF2ZH_LANG_TO`: 設定目標語言。預設為 "Simplified Chinese"。

## 預覽

<img src="./../images/before.png" width="500"/>
<img src="./../images/after.png" width="500"/>

## 維護

GUI 由 [Rongxin](https://github.com/reycn) 維護

<div align="right"> 
<h6><small>Some content on this page has been translated by GPT and may contain errors.</small></h6>