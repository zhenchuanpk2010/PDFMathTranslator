一些問題經常被問到，因此我們為遇到類似問題的用戶提供了以下列表。

## 是否需要 GPU？
- **問題**:
## 是否需要 GPU？

由於程式使用人工智慧來識別與提取文件，是否需要 GPU？

- **答案**:
**不需要 GPU。** 但如果您有 GPU，程式會自動使用它以獲得更高的效能。

## 下載中斷了嗎？
- **問題**:
我在下載模型時遇到以下中斷錯誤。該怎麼辦？

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
執行程序時，如果找不到文件，用戶會看到以下輸出：`以下檔案不存在：example.pdf`。

- **解決方案**：
  - 在檔案所在的目錄中打開命令行，或
  - 直接在 pdf2zh 後輸入檔案的完整路徑，或
  - 使用互動模式 `pdf2zh -i` 直接拖放檔案


## SSL 錯誤與其他網路問題
- **問題**:
在下載 hugging face 模型時，中國用戶可能會遇到網路錯誤。例如，在 [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55) 和 [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70) 中。

- **解決方案**：
  - [繞過防火長城](https://github.com/clash-verge-rev/clash-verge-rev)。
  - [使用 Hugging Face 鏡像](https://hf-mirror.com/)。
  - [使用便攜版本](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable)。
  - [改用 Docker](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker)。
  - [更新憑證](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests)，如[問題 #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55)中所建議。

If you are unable to access the localhost address (e.g., `http://127.0.0.1:5000`), please check the following:

1. **Check if the service is running**  
   Run the following command in the terminal to check if the service is running:  
   ```bash
   ps aux | grep pdf2zh
   ```
   If the service is not running, start it with:  
   ```bash
   pdf2zh --webui
   ```

2. **Check the port**  
   The default port is `5000`. If the port is occupied, you can specify another port with:  
   ```bash
   pdf2zh --webui --port 5001
   ```

3. **Check the firewall**  
   Ensure that your firewall is not blocking the port. For example, on Ubuntu, you can allow the port with:  
   ```bash
   sudo ufw allow 5000
   ```

4. **Check the network**  
   If you are using a proxy or VPN, try disabling it temporarily.

5. **Check the browser**  
   Try accessing the address in a different browser or in incognito mode.

If the issue persists, please [open an issue](https://github.com/PDFMathTranslate/pdf2zh/issues) on GitHub.

---

## 無法訪問本地主機

如果您無法訪問本地主機地址（例如 `http://127.0.0.1:5000`），請檢查以下內容：

1. **檢查服務是否正在運行**  
   在終端中運行以下命令以檢查服務是否正在運行：  
   ```bash
   ps aux | grep pdf2zh
   ```
   如果服務未運行，請使用以下命令啟動：  
   ```bash
   pdf2zh --webui
   ```

2. **檢查端口**  
   默認端口為 `5000`。如果端口被佔用，您可以指定另一個端口：  
   ```bash
   pdf2zh --webui --port 5001
   ```

3. **檢查防火牆**  
   確保您的防火牆沒有阻止該端口。例如，在 Ubuntu 上，您可以使用以下命令允許該端口：  
   ```bash
   sudo ufw allow 5000
   ```

4. **檢查網絡**  
   如果您正在使用代理或 VPN，請嘗試暫時禁用它們。

5. **檢查瀏覽器**  
   嘗試在不同的瀏覽器或隱私模式下訪問該地址。

如果問題仍然存在，請在 GitHub 上[提交問題](https://github.com/PDFMathTranslate/pdf2zh/issues)。
請參閱下方內容。

## 使用 0.0.0.0 啟動 GUI 時出現錯誤
- **問題**:
在全局模式下使用代理軟體可能會導致 Gradio 無法正常啟動。例如，在[問題 #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77)中。

- **解決方案**：
使用規則模式

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>Some content on this page has been translated by GPT and may contain errors.</small></h6>