以下是一些用户经常遇到的问题，我们为遇到类似情况的用户提供了这份清单。

## 是否需要 GPU？
- **问题**：
由于该程序使用人工智能来识别和提取文档，是否需要 GPU？

- **回答**:
**不需要 GPU。** 但如果你有 GPU，程序会自动使用它以获得更高性能。

## 下载中断了？
- **问题**：
我在下载模型时遇到了以下中断错误。我该怎么办？

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **回答**:
网络受到干扰，请使用稳定的网络链接或尝试绕过网络干预。

## 如何更新到最新版本？
- **问题**：
我想使用最新版本的一些功能，如何更新它？

- **回答**:
`pip install -U pdf2zh`


## 以下文件不存在：example.pdf
- **问题**:
执行程序时，如果未找到文档，用户会看到以下输出：`The following files do not exist: example.pdf`。

- **解决方案**：
  - 在文件所在目录打开命令行，或
  - 在 pdf2zh 后直接输入文件的完整路径，或
  - 使用交互模式 `pdf2zh -i` 直接拖放文件


## SSL 错误及其他网络问题
- **问题**:
在下载 hugging face 模型时，中国用户可能会遇到网络错误。例如，在 [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55)、[#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70) 中。

- **解决方案**：
  - [绕过 GFW](https://github.com/clash-verge-rev/clash-verge-rev)。
  - [使用 Hugging Face 镜像](https://hf-mirror.com/)。
  - [使用便携版](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable)。
  - [改用 Docker](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker)。
  - [更新证书](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests)，如 [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55) 中建议。

## 无法访问本地主机
请见下文。

## 使用 0.0.0.0 启动 GUI 时出错
- **问题**:
使用全局模式的代理软件可能会阻止 Gradio 正常启动。例如，在 [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77) 中。

- **解决方案**：
使用规则模式

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>本页面的部分内容由 GPT 翻译，可能包含错误。</small></h6>