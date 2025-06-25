一些常见问题被频繁提出，因此我们为遇到类似问题的用户提供了以下列表。

## 是否需要 GPU？

- **问题**:  
由于该程序使用人工智能来识别和提取文档，是否需要 GPU？

- **回答**:  
**无需 GPU**。但如果您拥有 GPU，程序将自动调用以提升性能。

## 下载中断？

- **问题**:  
我在下载模型时遇到以下中断错误，该怎么办？

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **回答**:  
网络受到干扰，请使用稳定的网络链接或尝试绕过网络干预。

## 如何更新到最新版本？

- **问题**:  
我想使用最新版本的一些功能，如何更新？

- **答案**:  
`pip install -U pdf2zh`

## 以下文件不存在：example.pdf

- **问题**:  
运行程序时，如果未找到文档，用户会看到以下输出：`The following files do not exist: example.pdf`。

- **解决方案**:
  - 在文件所在目录打开命令行，或
  - 直接在 pdf2zh 后输入文件的完整路径，或
  - 使用交互模式 `pdf2zh -i` 直接拖放文件

## SSL 错误及其他网络问题

- **问题**:  
在中国下载 hugging face 模型时，用户可能会遇到网络错误。例如，在[issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55)和[#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70)中提到的案例。

- **解决方案**:
  - [绕过 GFW](https://github.com/clash-verge-rev/clash-verge-rev).
  - [使用 Hugging Face 镜像站](https://hf-mirror.com/).
  - [使用便携版](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [改用 Docker](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [更新证书](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests)，如[issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55)所述。

## 无法访问本地主机

请参阅下文。

## 使用 0.0.0.0 启动 GUI 时出错

- **问题**:  
在全局模式下使用代理软件可能会阻止 Gradio 正常启动。例如，在[问题 #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77)中。

- **解决方案**:  
使用规则模式

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>本页面的部分内容由 GPT 翻译，可能包含错误。</small></h6>