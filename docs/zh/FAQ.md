以下是一些用户常问的问题，我们为遇到类似情况的用户整理了这份清单。

## 是否需要 GPU？
- **问题**:
## 是否需要 GPU？

由于该程序使用人工智能来识别和提取文档，是否需要 GPU？

- **答案**：
**不需要 GPU。** 但如果您有 GPU，程序会自动使用它以获得更高性能。

## 下载中断了？
- **问题**:
我在下载模型时遇到了以下中断错误。我该怎么办？

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **答案**：
网络受到干扰，请使用稳定的网络链接或尝试绕过网络干预。

## 如何更新到最新版本？
- **问题**:
我想使用最新版本的一些功能，如何更新它？

- **答案**：
`pip install -U pdf2zh`


## 以下文件不存在：example.pdf
- **问题**:
执行程序时，如果未找到文档，用户会看到以下输出：`The following files do not exist: example.pdf`。

- **解决方案**：
  - 在文件所在目录打开命令行，或
  - 直接在 pdf2zh 后输入文件的完整路径，或
  - 使用交互模式 `pdf2zh -i` 直接拖放文件


## SSL 错误与其他网络问题
- **问题**:
在下载 Hugging Face 模型时，中国用户可能会遇到网络错误。例如，在 [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55) 和 [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70) 中。

- **解决方案**：
  - [绕过 GFW](https://github.com/clash-verge-rev/clash-verge-rev)。
  - [使用 Hugging Face 镜像](https://hf-mirror.com/)。
  - [使用便携版](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable)。
  - [改用 Docker](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker)。
  - [更新证书](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests)，如 [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55) 中建议。

If you are unable to access the localhost address (e.g., `http://127.0.0.1:5000`), please check the following:

1. **Ensure the service is running**:
   - Run `pdf2zh --webui` in the terminal and check if there are any error messages.
   - If you see `Running on http://127.0.0.1:5000`, the service is running normally.

2. **Check the port**:
   - The default port is `5000`. If this port is occupied, the service will automatically switch to another port (e.g., `5001`).
   - You can specify a port manually using `pdf2zh --webui --port <port_number>`.

3. **Firewall settings**:
   - Ensure your firewall is not blocking the port. You may need to add an exception for the port in your firewall settings.

4. **Network configuration**:
   - If you are using a VPN or proxy, try disabling it temporarily to see if that resolves the issue.

5. **Browser cache**:
   - Clear your browser cache or try accessing the address in a different browser.

If the issue persists, please [submit an issue](https://github.com/PDFMathTranslate/pdf2zh/issues) with the error message you encountered.

---

## 无法访问本地主机

如果您无法访问本地主机地址（例如 `http://127.0.0.1:5000`），请检查以下内容：

1. **确保服务正在运行**：
   - 在终端中运行 `pdf2zh --webui` 并检查是否有错误消息。
   - 如果看到 `Running on http://127.0.0.1:5000`，则表示服务正常运行。

2. **检查端口**：
   - 默认端口为 `5000`。如果该端口被占用，服务会自动切换到另一个端口（例如 `5001`）。
   - 您可以使用 `pdf2zh --webui --port <端口号>` 手动指定端口。

3. **防火墙设置**：
   - 确保您的防火墙没有阻止该端口。您可能需要在防火墙设置中添加对该端口的例外。

4. **网络配置**：
   - 如果您正在使用 VPN 或代理，请尝试暂时禁用它，看看是否能解决问题。

5. **浏览器缓存**：
   - 清除浏览器缓存或尝试在其他浏览器中访问该地址。

如果问题仍然存在，请[提交问题](https://github.com/PDFMathTranslate/pdf2zh/issues)并提供您遇到的错误消息。
请参阅下文。

## 使用 0.0.0.0 启动 GUI 时出错
- **问题**:
在全局模式下使用代理软件可能会阻止 Gradio 正常启动。例如，在 [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77) 中。

- **解决方案**：
使用规则模式

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>本页面的部分内容由 GPT 翻译，可能包含错误。</small></h6>