以下是一些經常被詢問的問題，我們為遇到類似問題的使用者提供了這份清單。

## 是否需要 GPU？
- **問題**:
該程式使用人工智慧來辨識與擷取文件，是否需要 GPU？

- **答案**:
**不需要 GPU。** 但如果你有 GPU，程式會自動使用它以獲得更高的效能。

## 下載中斷了嗎？
- **問題**:
我在下載模型時遇到以下中斷錯誤。我該怎麼辦？

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **答案**:
網路正受到干擾，請使用穩定的網路連結或嘗試繞過網路干預。

## 如何更新至最新版本？
- **問題**:
我想使用最新版本的一些功能，如何更新它？

- **答案**:
`pip install -U pdf2zh`


## 以下檔案不存在：example.pdf
- **問題**:
執行程式時，若找不到文件，使用者會看到以下輸出：`The following files do not exist: example.pdf`。

- **解決方案**：
  - 在檔案所在目錄中開啟命令行，或
  - 直接在 pdf2zh 後輸入檔案的完整路徑，或
  - 使用互動模式 `pdf2zh -i` 直接拖放檔案


## SSL 錯誤與其他網路問題
- **問題**:
在下載 hugging face 模型時，中國用戶可能會遇到網路錯誤。例如，在 [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55)、[#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70) 中。

- **解決方案**：
  - [繞過防火長城](https://github.com/clash-verge-rev/clash-verge-rev)。
  - [使用 Hugging Face 鏡像站](https://hf-mirror.com/)。
  - [使用便攜版](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable)。
  - [改用 Docker](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker)。
  - [更新憑證](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests)，如 [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55) 所建議。

## 無法存取本地主機
請參閱下方。

## 使用 0.0.0.0 啟動 GUI 時出現錯誤
- **問題**:
使用全域模式的代理軟體可能會導致 Gradio 無法正常啟動。例如，在 [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77)。

- **解決方案**：
使用規則模式

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>Some content on this page has been translated by GPT and may contain errors.</small></h6>