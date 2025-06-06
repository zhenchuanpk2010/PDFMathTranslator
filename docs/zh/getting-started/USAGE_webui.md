[**快速开始**](./getting-started.md) > **如何使用** > **WebUI** _(当前页面)_

---

### 通过 WebUI 使用 PDFMathTranslate

#### 如何打开 WebUI 页面：

> 有几种方法可以打开 WebUI 界面。如果您使用 **Windows**，请参阅 [此文章](./INSTALLATION_winexe.md);

1. 确保 Python 已安装 (3.10 <= 版本 <= 3.13)

2. 安装我们的包：

3. 在浏览器中开始使用：

    ```bash
    pdf2zh_next --gui
    ```

4. 如果您的浏览器没有自动启动，请转到

    ```bash
    http://localhost:7860/
    ```

> 将 PDF 文件拖放到窗口中并点击 `Translate`。

<!-- <img src="./images/gui.gif" width="500"/> -->
<img src='./../images/gui.gif' width="500"/>

### 环境变量

> 您可以使用环境变量设置源和目标语言：

> - `PDF2ZH_LANG_FROM`: 设置源语言。默认为 "English"。
> - `PDF2ZH_LANG_TO`: 设置目标语言。默认为 "Simplified Chinese"。

## 预览

<img src="./../images/before.png" width="500"/>
<img src="./../images/after.png" width="500"/>

## 维护

GUI 由 [Rongxin](https://github.com/reycn) 维护