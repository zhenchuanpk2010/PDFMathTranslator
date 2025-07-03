[**高級選項**](./introduction.md) > **高級選項** _(current)_

---

<h3 id="toc">目錄</h3>

- [命令行參數](#命令行參數)
- [部分翻譯](#部分翻譯)
- [指定來源與目標語言](#指定來源與目標語言)
- [翻譯例外情況](#翻譯例外情況)
- [自定義提示](#自定義提示)
- [自訂配置](#自訂配置)
- [跳過清理](#跳過清理)
- [翻譯緩存](#翻譯緩存)
- [部署為公共服務](#部署為公共服務)
- [認證與歡迎頁面](#認證與歡迎頁面)
- [詞彙表支援](#詞彙表支援)

---

#### 命令行參數

在命令行中執行翻譯指令，於當前工作目錄下生成翻譯後的文檔 `example-mono.pdf` 與雙語文檔 `example-dual.pdf`。預設使用 Google 作為翻譯服務。更多支援的翻譯服務可參考[此處](https://github.com/PDFMathTranslate/PDFMathTranslate-next/blob/main/docs/ADVANCED.md#services)。

<img src="./../images/cmd_light.svg" width="580px"  alt="cmd"/>

在下表中，我們列出了所有高級選項以供參考：

##### 參數

| 選項                          | 功能                                                                               | 範例                                                                                                              |
| ------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| `files`                         | 本地 PDF 文件路徑                                                                    | `pdf2zh ~/local.pdf`                                                                                                 |
| `links`                         | 線上文件                                                                           | `pdf2zh http://arxiv.org/paper.pdf`                                                                                  |
| `--output`                      | 檔案輸出目錄                                                             | `pdf2zh example.pdf --output /outputpath`                                                                            |
| `--<Services>`                  | 使用[**特定服務**](./翻譯服務文檔.md)進行翻譯 | `pdf2zh example.pdf --openai`<br>`pdf2zh example.pdf --deepseek`                                                     |
| `--help`, `-h`                  | 顯示幫助訊息並退出                                                             | `pdf2zh -h`                                                                                                          |
| `--config-file`                 | 設定檔案的路徑                                                         | `pdf2zh --config-file /path/to/config/config.toml`                                                                   |
| `--report-interval`             | 進度報告間隔（秒）                                                    | `pdf2zh example.pdf --report-interval 5`                                                                             |
| `--debug`                       | 使用除錯日誌等級                                                                | `pdf2zh example.pdf --debug`                                                                                         |
| `--gui`                         | 與圖形介面互動                                                                      | `pdf2zh --gui`                                                                                                       |
| `--warmup`                      | 僅下載並驗證所需資源後退出                                     | `pdf2zh example.pdf --warmup`                                                                                        |
| `--generate-offline-assets`     | 在指定目錄中生成離線資源包                             | `pdf2zh example.pdf --generate-offline-assets /path`                                                                 |
| `--restore-offline-assets`      | 從指定目錄恢復離線資源包                            | `pdf2zh example.pdf --restore-offline-assets /path`                                                                  |
| `--version`                     | 顯示版本後退出                                                                 | `pdf2zh --version`                                                                                                   |
| `--pages`                       | 部分文件翻譯                                                           | `pdf2zh example.pdf --pages 1,2,1-,-3,3-5`                                                                           |
| `--lang-in`                     | 來源語言的語言代碼                                                            | `pdf2zh example.pdf --lang-in en`                                                                                    |
| `--lang-out`                    | 目標語言的語言代碼                                                            | `pdf2zh example.pdf --lang-out zh-CN`                                                                                |
| `--min-text-length`             | 最小翻譯文字長度                                                       | `pdf2zh example.pdf --min-text-length 5`                                                                             |
| `--rpc-doclayout`               | 用於文件佈局分析的 RPC 服務主機地址                                  |                                                                                                                      |
| `--qps`                         | 翻譯服務的 QPS 限制                                                      | `pdf2zh example.pdf --qps 200`                                                                                       |
| `--ignore-cache`                | 忽略翻譯緩存                                                               | `pdf2zh example.pdf --ignore-cache`                                                                                  |
| `--custom-system-prompt`        | 翻譯用的自定義系統提示。適用於 Qwen 3 的 `/no_think` 功能                   | `pdf2zh example.pdf --custom-system-prompt "/no_think You are a professional, authentic machine translation engine"` |
| `--pool-max-worker`             | 翻譯池的最大工作線程數。若未設置，將使用 qps 作為工作線程數量 | `pdf2zh example.pdf --pool-max-worker 100`                                                                |
| `--no-auto-extract-glossary`    | 禁用自動提取詞彙表                                                          | `pdf2zh example.pdf --no-auto-extract-glossary`                                                                      |
| `--primary-font-family`         | 覆蓋翻譯文字的主要字體家族。選項：'serif' 代表襯線字體，'sans-serif' 代表無襯線字體，'script' 代表手寫/斜體字體。若未指定，則根據原始文字屬性自動選擇字體。 | `pdf2zh example.pdf --primary-font-family serif` |
| `--no-dual`                     | 不輸出雙語 PDF 文件                                                      | `pdf2zh example.pdf --no-dual`                                                                                       |
| `--no-mono`                     | 不輸出單語種 PDF 文件                                                    | `pdf2zh example.pdf --no-mono`                                                                                       |
| `--formular-font-pattern`       | 用於識別公式文字的字體模式                                                  | `pdf2zh example.pdf --formular-font-pattern "(MS.*)"`                                                                |
| `--formular-char-pattern`       | 用於識別公式文字的字元模式                                             | `pdf2zh example.pdf --formular-char-pattern "(MS.*)"`                                                                |
| `--split-short-line`            | 強制將短行拆分為不同段落                                       | `pdf2zh example.pdf --split-short-line`                                                                              |
| `--short-line-split-factor`     | 短行分割閾值因子                                                 |                                                                                                                      |
| `--skip-clean`                  | 跳過 PDF 清理步驟                                                                 | `pdf2zh example.pdf --skip-clean`                                                                                    |
| `--dual-translate-first`        | 在雙 PDF 模式下優先放置翻譯頁                                          | `pdf2zh example.pdf --dual-translate-first`                                                                                            |
| `--disable-rich-text-translate` | 停用富文本翻譯                                                          | `pdf2zh example.pdf --disable-rich-text-translate`                                                                   |
| `--enhance-compatibility`       | 啟用所有相容性增強選項                                           | `pdf2zh example.pdf --enhance-compatibility`                                                                         |
| `--use-alternating-pages-dual`  | 使用交替頁面模式處理雙頁 PDF                                                | `pdf2zh example.pdf --use-alternating-pages-dual`                                                                    |
| `--watermark-output-mode`       | PDF 檔案的水印輸出模式                                                    | `pdf2zh example.pdf --watermark-output-mode "NoWaterMark"`                                                           |
| `--max-pages-per-part`          | 分割翻譯時每部分的最大頁數                                           | `pdf2zh example.pdf --max-pages-per-part 1`                                                                          |
| `--translate-table-text`        | 翻譯表格文字（實驗性功能）                                                    | `pdf2zh example.pdf --translate-table-text`                                                                          |
| `--skip-scanned-detection`      | 跳過掃描檢測                                                                 | `pdf2zh example.pdf --skip-scanned-detection`                                                                        |
| `--ocr-workaround`              | 強制將翻譯後的文字設為黑色並添加白色背景                             | `pdf2zh example.pdf --ocr-workaround`                                                                                |
| `--auto-enable-ocr-workaround`  | 啟用自動 OCR 解決方案。若檢測到文件為重度掃描文件，將嘗試啟用 OCR 處理並跳過後續掃描檢測。詳情請參閱文檔。(預設值：False) | `pdf2zh example.pdf --auto-enable-ocr-workaround True`                    |
| `--only-include-translated-page`| 僅在輸出 PDF 中包含已翻譯的頁面。僅在 --pages 參數使用時生效。 | `pdf2zh example.pdf --pages 1-5 --only-include-translated-page`                                                       |
| `--glossaries`                  | 自訂翻譯詞彙表。                                                      | `pdf2zh example.pdf --glossaries "glossary1.csv,glossary2.csv,glossary3.csv"`                                         |
| `--save-auto-extracted-glossary`| 儲存自動提取的詞彙表。                                                | `pdf2zh example.pdf --save-auto-extracted-glossary`                                                                   |


##### 圖形介面參數

| 選項                          | 功能                               | 範例                                         |
| ------------------------------- | -------------------------------------- | ----------------------------------------------- |
| `--share`                       | 啟用分享模式                    | `pdf2zh --gui --share`                          |
| `--auth-file`                   | 認證檔案路徑        | `pdf2zh --gui --auth-file /path`                |
| `--welcome-page`                | 歡迎頁面 html 文件路徑          | `pdf2zh --gui --welcome-page /path`             |
| `--enabled-services`            | 啟用的翻譯服務           | `pdf2zh --gui --enabled-services "Bing,OpenAI"` |
| `--disable-gui-sensitive-input` | 禁用圖形介面敏感輸入            | `pdf2zh --gui --disable-gui-sensitive-input`    |
| `--disable-config-auto-save`    | 禁用自動配置保存 | `pdf2zh --gui --disable-config-auto-save`       |
| `--server-port`                 | WebUI 端口                             | `pdf2zh --gui --server-port 7860`               |

[⬆️ 返回頂部](#toc)

---

#### 部分翻譯

使用 `--pages` 參數來翻譯文件的一部分。

- 如果頁碼是連續的，可以這樣寫：

```bash
pdf2zh_next example.pdf --pages 1-3
```

```bash
pdf2zh_next example.pdf --pages 25-
```

> [!TIP]
> `25-` 包含第 25 頁之後的所有頁面。如果您的文件有 100 頁，這等同於 `25-100`。
> 
> 同理，`-25` 包含第 25 頁之前的所有頁面，這等同於 `1-25`。

- 如果頁面不是連續的，可以使用逗號 `,` 來分隔它們。

舉例來說，如果您想翻譯第一頁和第三頁，可以使用以下命令：

```bash
pdf2zh_next example.pdf --pages "1,3"
```

- 如果頁面同時包含連續與非連續範圍，你也可以用逗號連接它們，像這樣：

```bash
pdf2zh_next example.pdf --pages "1,3,10-20,25-"
```

此命令將翻譯第一頁、第三頁、第 10 至 20 頁，以及從第 25 頁開始的所有頁面。


[⬆️ 回到頂部](#toc)

---

#### 指定來源與目標語言

參見 [Google 語言代碼](https://developers.google.com/admin-sdk/directory/v1/languages)、[DeepL 語言代碼](https://developers.deepl.com/docs/resources/supported-languages)

```bash
pdf2zh_next example.pdf --lang-in en -lang-out ja
```

[⬆️ 返回頂部](#toc)

---

#### 翻譯例外情況

使用正則表達式來指定需要保留的公式字體與字符：

```bash
pdf2zh_next example.pdf --formular-font-pattern "(CM[^RT].*|MS.*|.*Ital)" --formular-char-pattern "(\(|\||\)|\+|=|\d|[\u0080-\ufaff])"
```

預設保留 `Latex`、`Mono`、`Code`、`Italic`、`Symbol` 與 `Math` 字體：

```bash
pdf2zh_next example.pdf --formular-font-pattern "(CM[^R]|MS.M|XY|MT|BL|RM|EU|LA|RS|LINE|LCIRCLE|TeX-|rsfs|txsy|wasy|stmary|.*Mono|.*Code|.*Ital|.*Sym|.*Math)"
```

[⬆️ 返回頂部](#toc)

---

#### 自定義提示

<!-- Note: System prompt is currently not supported. See [this change](https://github.com/PDFMathTranslate/PDFMathTranslate-next/pull/637). -->

用於翻譯的自定義系統提示。主要用於在提示中添加 Qwen 3 的 '/no_think' 指令。

```bash
pdf2zh_next example.pdf --custom-system-prompt "/no_think You are a professional and reliable machine translation engine responsible for translating the input text into zh_CN.When translating, strictly follow the instructions below to ensure translation quality and preserve all formatting, tags, and placeholders:"
```

[⬆️ 返回頂部](#toc)

---

#### 自訂配置

有多種方式可以修改並導入配置文件。

> [!NOTE]
> **設定檔層級結構**
>
> 當使用不同方法修改同一參數時，軟體將依照以下優先順序套用變更。
>
> 較高優先層級的修改會覆蓋較低層級的設定。
>
> **命令行/圖形介面 > 環境變數 > 使用者設定檔 > 預設設定檔**

- 透過**命令行參數**修改配置

在大多數情況下，您可以直接通過命令行參數傳遞所需的設置。更多信息請參考[命令行參數](#cmd)。

例如，如果您想啟用圖形介面窗口，可以使用以下命令：

```bash
pdf2zh_next --gui
```

- 透過**環境變數**修改配置

你可以將命令列參數中的 `--` 替換為 `PDF2ZH_`，使用 `=` 連接參數，並將 `-` 替換為 `_` 作為環境變數。

例如，如果你想啟用圖形介面視窗，可以使用以下命令：

```bash
PDF2ZH_GUI=TRUE pdf2zh_next
```

<img src="./../images/ev_light.svg" width="580px"  alt="env"/>

- 使用者指定的**設定檔**

你可以使用以下命令行參數來指定配置檔案：

```bash
pdf2zh_next --config-file '/path/config.toml'
```

如果您不確定配置文件的格式，請參考下方描述的默認配置文件。

- **預設配置文件**

預設的配置文件位於 `~/.config/pdf2zh`。
請勿修改 `default` 目錄中的配置文件。
強烈建議參考此配置文件的內容，並使用**自訂配置**來實現您自己的配置文件。

> [!TIP]
> - 預設情況下，pdf2zh 2.0 每次在圖形介面點擊翻譯按鈕時，會自動將當前配置保存至 `~/.config/pdf2zh/config.v3.toml`。此配置文件將在下次啟動時自動載入。
> - `default` 目錄中的配置文件由程式自動生成。您可以複製它們進行修改，但請勿直接修改這些文件。
> - 配置文件中可能包含 "v2"、"v3" 等版本號。這些是**配置文件的版本號**，**並非** pdf2zh 本身的版本號。


[⬆️ 返回頂部](#toc)

---

#### 跳過清理

當此參數設為 True 時，將跳過 PDF 清理步驟，這可以提高兼容性並避免一些字體處理問題。

使用方法：

```bash
pdf2zh_next example.pdf --skip-clean
```

或者使用環境變數：

```bash
PDF2ZH_SKIP_CLEAN=TRUE pdf2zh_next example.pdf
```

> [!TIP]
> 當啟用 `--enhance-compatibility` 時，跳過清理會自動啟用。

---

#### 翻譯緩存

PDFMathTranslate 會緩存已翻譯的文本以提高速度，並避免對相同內容進行不必要的 API 調用。你可以使用 `--ignore-cache` 選項來忽略翻譯緩存並強制重新翻譯。

```bash
pdf2zh_next example.pdf --ignore-cache
```

[⬆️ 返回頂部](#toc)

---

#### 部署為公共服務

當在公共服務上部署 pdf2zh 圖形介面時，您應按照以下說明修改配置文件。

> [!TIP]
> - 公開部署時，應同時啟用 `disable_gui_sensitive_input` 和 `disable_config_auto_save`。
> - 使用*英文逗號* <kbd>,</kbd> 分隔不同的可用服務。

一個可用的配置如下：

```toml title="config.toml"
[basic]
gui = true

[gui_settings]
enabled_services = "Bing,OpenAI"
disable_gui_sensitive_input = true
disable_config_auto_save = true
```

[⬆️ 返回頂部](#toc)

---

#### 認證與歡迎頁面

當使用認證與歡迎頁面來指定哪些用戶可以使用 Web UI 並自訂登入頁面時：

範例 auth.txt
每行包含兩個元素，用戶名和密碼，以逗號分隔。

```
admin,123456
user1,password1
user2,abc123
guest,guest123
test,test123
```

example welcome.html

```html
<!DOCTYPE html>
<html>
<head>
    <title>Simple HTML</title>
</head>
<body>
    <h1>Hello, World!</h1>
    <p>Welcome to my simple HTML page.</p>
</body>
</html>
```

> [!NOTE]
> 僅在認證檔案不為空白時，歡迎頁面才會生效。
> 若認證檔案為空白，則不會有任何認證程序。 :)

一個可用的配置如下：

```toml title="config.toml"
[basic]
gui = true

[gui_settings]
auth_file = "/path/to/auth/file"
welcome_page = "/path/to/welcome/html/file"
```

[⬆️ 返回頂部](#toc)

---

#### 詞彙表支援

PDFMathTranslate 支援詞彙表功能。詞彙表檔案應為 `csv` 格式。
檔案中包含三欄位。以下是一個示範詞彙表檔案：

| source | target  | tgt_lng |
|--------|---------|---------|
| AutoML | 自动 ML  | zh-CN   |
| a,a    | a       | zh-CN   |
| "      | "       | zh-CN   |


對於命令行用戶：
您可以使用多個文件作為詞彙表。不同文件之間應以 `,` 分隔。

```bash
pdf2zh_next example.pdf --glossaries "glossary1.csv,glossary2.csv,glossary3.csv"
```

對於 WebUI 使用者：

您現在可以上傳自己的詞彙表檔案。上傳檔案後，您可以點擊檔案名稱查看內容，內容會顯示在下方。

[⬆️ 回到頂部](#toc)

<div align="right"> 
<h6><small>Some content on this page has been translated by GPT and may contain errors.</small></h6>