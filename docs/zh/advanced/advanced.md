[**高级选项**](./introduction.md) > **高级选项** _(当前页面)_

---

<h3 id="toc">目录</h3>

- [命令行参数](#command-line-args)
  - [参数](#args)
  - [GUI 参数](#gui-args)
- [部分翻译](#partial-translation)
- [指定源语言和目标语言](#specify-source-and-target-languages)
- [带例外的翻译](#translate-wih-exceptions)
- [自定义提示](#custom-prompt)
- [自定义配置](#custom-configuration)
- [跳过清理](#skip-clean)
- [翻译缓存](#translation-cache)
- [作为公共服务部署](#deployment-as-a-public-services)
- [认证和欢迎页面](#authentication-and-welcome-page)

---

#### 命令行参数

在命令行中执行翻译命令，以在当前工作目录中生成翻译后的文档 `example-mono.pdf` 和双语文档 `example-dual.pdf`。默认使用 Google 作为翻译服务。更多支持的翻译服务可以在 [这里](https://github.com/PDFMathTranslate/PDFMathTranslate-next/blob/main/docs/ADVANCED.md#services) 找到。

<img src="./../images/cmd_light.svg" width="580px"  alt="cmd"/>

在下表中，我们列出了所有高级选项供参考：

##### 参数

| 选项                            | 功能                                                                   | 示例                                                                                                                 |
| ------------------------------- | ---------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| `files`                         | 本地 PDF 文件路径                                                      | `pdf2zh ~/local.pdf`                                                                                                 |
| `links`                         | 在线文件                                                               | `pdf2zh http://arxiv.org/paper.pdf`                                                                                  |
| `--output`                      | 文件输出目录                                                           | `pdf2zh example.pdf --output /outputpath`                                                                            |
| `--<Services>`                  | 使用[**特定服务**](./Documentation-of-Translation-Services.md)进行翻译 | `pdf2zh example.pdf --openai`<br>`pdf2zh example.pdf --deepseek`                                                     |
| `--help`, `-h`                  | 显示帮助信息并退出                                                     | `pdf2zh -h`                                                                                                          |
| `--config-file`                 | 配置文件路径                                                           | `pdf2zh --config-file /path/to/config/config.toml`                                                                   |
| `--report-interval`             | 进度报告间隔（秒）                                                     | `pdf2zh example.pdf --report-interval 5`                                                                             |
| `--debug`                       | 使用调试日志级别                                                       | `pdf2zh example.pdf --debug`                                                                                         |
| `--gui`                         | 使用图形用户界面                                                       | `pdf2zh --gui`                                                                                                       |
| `--warmup`                      | 仅下载并验证所需资产然后退出                                           | `pdf2zh example.pdf --warmup`                                                                                        |
| `--generate-offline-assets`     | 在指定目录生成离线资产包                                               | `pdf2zh example.pdf --generate-offline-assets /path`                                                                 |
| `--restore-offline-assets`      | 从指定目录恢复离线资产包                                               | `pdf2zh example.pdf --restore-offline-assets /path`                                                                  |
| `--version`                     | 显示当前软件版本并退出                                                  | `pdf2zh --version`                                                                                                   |
| `--pages`                       | 部分文档翻译                                                           | `pdf2zh example.pdf --pages 1,2,1-,-3,3-5`                                                                           |
| `--lang-in`                     | 源语言代码                                                             | `pdf2zh example.pdf --lang-in en`                                                                                    |
| `--lang-out`                    | 目标语言代码                                                           | `pdf2zh example.pdf --lang-out zh`                                                                                   |
| `--min-text-length`             | 最小翻译文本长度                                                       | `pdf2zh example.pdf --min-text-length 5`                                                                             |
| `--rpc-doclayout`               | 文档布局分析的 RPC 服务主机地址                                        |                                                                                                                      |
| `--qps`                         | 翻译服务的 QPS 限制                                                    | `pdf2zh example.pdf --qps 200`                                                                                       |
| `--ignore-cache`                | 忽略翻译缓存                                                           | `pdf2zh example.pdf --ignore-cache`                                                                                  |
| `--custom-system-prompt`        | 自定义系统提示用于翻译。用于 Qwen 3 中的 `/no_think`                   | `pdf2zh example.pdf --custom-system-prompt "/no_think You are a professional, authentic machine translation engine"` |
| `--pool-max-worker`             | 设定翻译池的 worker 数。默认使用 QPS 值                                | `pdf2zh example.pdf --pool-max-worker 100`                                                                            |
| `--no-auto-extract-glossary`    | 禁用自动提取术语表                                                     | `pdf2zh example.pdf --no-auto-extract-glossary`                                                                      |
| `--primary-font-family`         | 覆盖翻译文本的主要字体系列。选项：'serif' 表示衬线字体，'sans-serif' 表示无衬线字体，'script' 表示手写/斜体字体。如果未指定，则根据原始文本属性自动选择字体。 | `pdf2zh example.pdf --primary-font-family serif` |
| `--no-dual`                     | 不输出双语 PDF 文件                                                    | `pdf2zh example.pdf --no-dual`                                                                                       |
| `--no-mono`                     | 不输出单语 PDF 文件                                                    | `pdf2zh example.pdf --no-mono`                                                                                       |
| `--formular-font-pattern`       | 用于识别公式文本的字体模式                                             | `pdf2zh example.pdf --formular-font-pattern "(MS.*)"`                                                                |
| `--formular-char-pattern`       | 用于识别公式文本的字符模式                                             | `pdf2zh example.pdf --formular-char-pattern "(MS.*)"`                                                                |
| `--split-short-line`            | 强制将短行分成不同段落                                                 | `pdf2zh example.pdf --split-short-line`                                                                              |
| `--short-line-split-factor`     | 短行的分割阈值因子                                                     |                                                                                                                      |
| `--skip-clean`                  | 跳过 PDF 清理步骤                                                      | `pdf2zh example.pdf --skip-clean`                                                                                    |
| `--dual-translate-first`        | 在双 PDF 模式下优先放置翻译页                                          | `pdf2zh example.pdf --dual-translate-first`                                                                          |
| `--disable-rich-text-translate` | 禁用富文本翻译                                                         | `pdf2zh example.pdf --disable-rich-text-translate`                                                                   |
| `--enhance-compatibility`       | 启用所有兼容性增强选项                                                 | `pdf2zh example.pdf --enhance-compatibility`                                                                         |
| `--use-alternating-pages-dual`  | 使用交替页面模式进行双 PDF                                             | `pdf2zh example.pdf --use-alternating-pages-dual`                                                                    |
| `--watermark-output-mode`       | PDF 文件的水印输出模式                                                 | `pdf2zh example.pdf --watermark-output-mode "NoWaterMark"`                                                           |
| `--max-pages-per-part`          | 分割翻译的每部分最大页数                                               | `pdf2zh example.pdf --max-pages-per-part 1`                                                                          |
| `--translate-table-text`        | 翻译表格文本（实验性）                                                 | `pdf2zh example.pdf --translate-table-text`                                                                          |
| `--skip-scanned-detection`      | 跳过扫描检测                                                           | `pdf2zh example.pdf --skip-scanned-detection`                                                                        |
| `--ocr-workaround`              | 强制将翻译文本设为黑色并添加白色背景                                   | `pdf2zh example.pdf --ocr-workaround`                                                                                |
| `--auto-enable-ocr-workaround`  | 启用自动 OCR 处理。如果检测到文档严重扫描，将尝试启用 OCR 处理并跳过进一步的扫描检测。详情请参阅文档。（默认值：False） | `pdf2zh example.pdf --auto-enable-ocr-workaround True`                    |
| `--only-include-translated-page`| 仅在输出的 PDF 中包含翻译过的页面。仅在使用 --pages 时生效。 | `pdf2zh example.pdf --pages 1-5 --only-include-translated-page`                    |

##### GUI 参数

| 选项                            | 功能               | 示例                                            |
| ------------------------------- | ------------------ | ----------------------------------------------- |
| `--share`                       | 启用共享模式       | `pdf2zh --gui --share`                          |
| `--auth-file`                   | 认证文件路径       | `pdf2zh --gui --auth-file /path`                |
| `--welcome-page`                | 欢迎 html 文件路径 | `pdf2zh --gui --welcome-page /path`             |
| `--enabled-services`            | 启用的翻译服务     | `pdf2zh --gui --enabled-services "Bing,OpenAI"` |
| `--disable-gui-sensitive-input` | 禁用 GUI 敏感输入  | `pdf2zh --gui --disable-gui-sensitive-input`    |
| `--disable-config-auto-save`    | 禁用自动配置保存   | `pdf2zh --gui --disable-config-auto-save`       |

[⬆️ 返回顶部](#toc)

---

#### 部分翻译

使用 `--pages` 参数翻译文档的一部分。

- 如果页码是连续的，可以这样写：

```bash
pdf2zh_next example.pdf --pages 1-3
```

```bash
pdf2zh_next example.pdf --pages 25-
```

> [!TIP]
> `25-` 包含第 25 页之后的所有页面。如果您的文档有 100 页，这相当于 `25-100`。
> 
> 类似地，`-25` 包含第 25 页之前的所有页面，相当于 `1-25`。

- 如果页面不连续，可以用逗号 `,` 分隔它们。

例如，如果您想翻译第一页和第三页，可以使用以下命令：

```bash
pdf2zh_next example.pdf --pages "1,3"
```

- 如果页面既包括连续又包括不连续的范围，也可以用逗号连接它们，如下所示：

```bash
pdf2zh_next example.pdf --pages "1,3,10-20,25-"
```

此命令将翻译第一页、第三页、第 10-20 页以及第 25 页到最后的所有页面。


[⬆️ 返回顶部](#toc)

---

#### 指定源语言和目标语言

参见 [Google 语言代码](https://developers.google.com/admin-sdk/directory/v1/languages)，[DeepL 语言代码](https://developers.deepl.com/docs/resources/supported-languages)

```bash
pdf2zh_next example.pdf --lang-in en -lang-out ja
```

[⬆️ 返回顶部](#toc)

---

#### 带例外的翻译

使用正则表达式指定需要保留的公式字体和字符：

```bash
pdf2zh_next example.pdf --formular-font-pattern "(CM[^RT].*|MS.*|.*Ital)" --formular-char-pattern "(\(|\||\)|\+|=|\d|[\u0080-\ufaff])"
```

默认保留 `Latex`、`Mono`、`Code`、`Italic`、`Symbol` 和 `Math` 字体：

```bash
pdf2zh_next example.pdf --formular-font-pattern "(CM[^R]|MS.M|XY|MT|BL|RM|EU|LA|RS|LINE|LCIRCLE|TeX-|rsfs|txsy|wasy|stmary|.*Mono|.*Code|.*Ital|.*Sym|.*Math)"
```

[⬆️ 返回顶部](#toc)

---

#### 自定义提示

<!-- Note: System prompt is currently not supported. See [this change](https://github.com/PDFMathTranslate/PDFMathTranslate-next/pull/637). -->

自定义系统提示用于翻译。主要用于在提示中添加 Qwen 3 的 '/no_think' 指令。

```bash
pdf2zh_next example.pdf --custom-system-prompt "/no_think You are a professional and reliable machine translation engine responsible for translating the input text into zh_CN.When translating, strictly follow the instructions below to ensure translation quality and preserve all formatting, tags, and placeholders:"
```

[⬆️ 返回顶部](#toc)

---

#### 自定义配置

有多种方法可以修改和导入配置文件。

> [!NOTE]
> **配置文件层次结构**
>
> 当使用不同方法修改相同参数时，软件将根据以下优先顺序应用更改。
>
> 排名较高的修改将覆盖排名较低的修改。
>
> **cli/gui > 环境变量 > 用户配置文件 > 默认配置文件**

- 通过 **命令行参数** 修改配置

在大多数情况下，您可以直接通过命令行参数传递所需的设置。有关更多信息，请参阅 [命令行参数](#cmd)。

例如，如果您想启用 GUI 窗口，可以使用以下命令：

```bash
pdf2zh_next --gui
```

- 通过 **环境变量** 修改配置

<!-- TODO 放一个环境变量的示意图在这里 -->
您可以将命令行参数中的 `--` 替换为 `PDF2ZH_`，使用 `=` 连接参数，并将 `-` 替换为 `_` 作为环境变量。

例如，如果您想启用 GUI 窗口，可以使用以下命令：

```bash
PDF2ZH_GUI=TRUE pdf2zh_next
```

<img src="./../images/ev_light.svg" width="580px"  alt="env"/>

- 用户指定的 **配置文件**

您可以使用以下命令行参数指定配置文件：

```bash
pdf2zh_next --config-file '/path/config.toml'
```

如果您不确定配置文件格式，请参阅下面描述的默认配置文件。

- **默认配置文件**

默认配置文件位于 `~/.config/pdf2zh`。
请不要修改 `default` 目录中的配置文件。
强烈建议参考此配置文件的内容并使用 **用户指定的配置文件** 来实现您自己的配置文件。


> [!TIP]
> - pdf2zh 2.0 默认会在每次点击 GUI 中的翻译按钮时，自动将当前配置保存至 `~/.config/pdf2zh/config.v3.toml`。下次启动时会默认加载这个配置文件
> - `default` 目录中的配置文件是程序自动生成的，您可以将其复制出来进行修改，但不要直接更改其本身。
> - 配置文件可能带有 "v2"、"v3" 等版本号。此为**配置文件的版本号**，而**不是** pdf2zh 本身的版本号。

[⬆️ 返回顶部](#toc)

---

#### 跳过清理

当此参数设置为 True 时，将跳过 PDF 清理步骤，这可以提高兼容性并避免一些字体处理问题。

用法：

```bash
pdf2zh_next example.pdf --skip-clean
```

或使用环境变量：

```bash
PDF2ZH_SKIP_CLEAN=TRUE pdf2zh_next example.pdf
```

> [!TIP]
> 当启用 `--enhance-compatibility` 时，跳过清理会自动启用。

---

#### 翻译缓存

PDFMathTranslate 缓存翻译文本以提高速度并避免对相同内容的不必要 API 调用。您可以使用 `--ignore-cache` 选项忽略翻译缓存并强制重新翻译。

```bash
pdf2zh_next example.pdf --ignore-cache
```

[⬆️ 返回顶部](#toc)

---

#### 作为公共服务部署

在公共服务上部署 pdf2zh GUI 时，您应按如下所述修改配置文件。

> [!TIP]
> - 在公开部署时，应启用 `disable_gui_sensitive_input` 和 `disable_config_auto_save`。
> - 用*英文逗号* <kbd>,</kbd> 分隔不同的可用服务。

一个可用的配置如下：

```toml title="config.toml"
[basic]
gui = true

[gui_settings]
enabled_services = "Bing,OpenAI"
disable_gui_sensitive_input = true
disable_config_auto_save = true
```

[⬆️ 返回顶部](#toc)

---

#### 认证和欢迎页面

使用认证和欢迎页面指定使用 Web UI 的用户并自定义登录页面：

示例 auth.txt
每行包含两个元素，用户名和密码，用逗号分隔。

```
admin,123456
user1,password1
user2,abc123
guest,guest123
test,test123
```

示例 welcome.html

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
> 只有在认证文件不为空时，欢迎页面才会生效。
> 如果认证文件为空，则不会进行认证。 :)

一个可用的配置如下：

```toml title="config.toml"
[basic]
gui = true

[gui_settings]
auth_file = "/path/to/auth/file"
welcome_page = "/path/to/welcome/html/file"
```

[⬆️ 返回顶部](#toc)

<div align="right">
<h6><small>本页面的部分内容由 GPT 翻译，可能包含错误。</small></h6>