一些問題經常被問到，因此我們為遇到類似問題的用戶提供了以下列表。

## 是否需要 GPU？
- **問題**:
## 是否需要 GPU？

- **答案**:
**不需要 GPU。** 但如果您有 GPU，程式會自動使用它以獲得更高的效能。

## 下載中斷了嗎？
- **問題**:
我在下載模型時遇到以下中斷錯誤。我該怎麼辦？

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **答案**:
網路受到干擾，請使用穩定的網路連結或嘗試繞過網路干預。

## 如何更新至最新版本？
- **問題**:
我想使用最新版本的一些功能，如何更新它？

- **答案**:
`pip install -U pdf2zh`


## 以下檔案不存在：example.pdf
- **問題**:
執行程序時，如果找不到文件，使用者會看到以下輸出：`以下檔案不存在：example.pdf`。

- **解決方案**：
  - 在檔案所在的目錄中開啟命令行，或
  - 直接在 pdf2zh 後輸入檔案的完整路徑，或
  - 使用互動模式 `pdf2zh -i` 直接拖放檔案


If you encounter SSL errors or other network-related issues while using pdf2zh, follow these steps to troubleshoot:

1. **Check Your Internet Connection**  
   Ensure that your device is connected to the internet. Try accessing other websites to confirm.

2. **Update Your System's CA Certificates**  
   SSL errors often occur due to outdated or missing CA certificates. Update them using your system's package manager:
   - **Ubuntu/Debian**: `sudo apt-get install --reinstall ca-certificates`
   - **CentOS/RHEL**: `sudo yum reinstall ca-certificates`
   - **macOS**: Use `brew` or manually update via Keychain Access.

3. **Disable SSL Verification (Temporary Fix)**  
   If the issue persists, you can temporarily disable SSL verification by adding `--no-check-certificate` to your command.  
   Example:  
   ```bash
   pdf2zh --no-check-certificate input.pdf
   ```

4. **Use a VPN or Proxy**  
   Some network restrictions may block pdf2zh's services. Try using a VPN or proxy to bypass these restrictions.

5. **Check Firewall/Antivirus Settings**  
   Firewalls or antivirus software might interfere with the connection. Temporarily disable them to test.

6. **Contact Support**  
   If none of the above works, [contact our support team](mailto:support@pdf2zh.com) with details of the error.

---

### TRANSLATED TEXT

## SSL 錯誤與其他網路問題

如果您在使用 pdf2zh 時遇到 SSL 錯誤或其他與網路相關的問題，請按照以下步驟進行故障排除：

1. **檢查您的網路連線**  
   確保您的裝置已連接到網路。嘗試訪問其他網站以確認。

2. **更新系統的 CA 憑證**  
   SSL 錯誤通常是由於過期或缺失的 CA 憑證所導致。請使用系統的套件管理器更新它們：
   - **Ubuntu/Debian**: `sudo apt-get install --reinstall ca-certificates`
   - **CentOS/RHEL**: `sudo yum reinstall ca-certificates`
   - **macOS**: 使用 `brew` 或透過 Keychain Access 手動更新。

3. **暫時停用 SSL 驗證**  
   如果問題仍然存在，您可以透過在命令中加入 `--no-check-certificate` 來暫時停用 SSL 驗證。  
   範例：  
   ```bash
   pdf2zh --no-check-certificate input.pdf
   ```

4. **使用 VPN 或代理**  
   某些網路限制可能會阻擋 pdf2zh 的服務。嘗試使用 VPN 或代理來繞過這些限制。

5. **檢查防火牆/防毒軟體設定**  
   防火牆或防毒軟體可能會干擾連線。暫時停用它們以進行測試。

6. **聯繫支援團隊**  
   如果以上方法均無效，請[聯繫我們的支援團隊](mailto:support@pdf2zh.com)並提供錯誤的詳細資訊。
- **問題**:
在下載 hugging face 模型時，中國的使用者可能會遇到網路錯誤。例如，在 [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55)、[#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70) 中。

- **解決方案**:
  - [繞過防火牆](https://github.com/clash-verge-rev/clash-verge-rev).
  - [使用 Hugging Face 鏡像](https://hf-mirror.com/).
  - [使用便攜版](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [改用 Docker](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [更新憑證](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests)，如 [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55) 中所建議。

## 無法訪問本地主機
請參閱下方內容。

## 使用 0.0.0.0 啟動 GUI 時出錯
- **問題**:
在全域模式下使用代理軟體可能會導致 Gradio 無法正常啟動。例如，在 [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77) 中提到的情況。

- **解決方案**：
使用規則模式

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>Some content on this page has been translated by GPT and may contain errors.</small></h6>