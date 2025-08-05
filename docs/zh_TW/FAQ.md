一些問題經常被問到，因此我們為遇到類似問題的用戶提供了一份清單。

## 是否需要 GPU？
- **問題**:
由於程式使用人工智慧來辨識與提取文件，是否需要 GPU？

- **回答**:
**不需要 GPU。** 但如果您有 GPU，程式會自動使用它以獲得更高的效能。

## 下載中斷了嗎？
- **問題**:
我在下載模型時遇到以下中斷錯誤。該怎麼辦？

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **回答**:
網路正受到干擾，請使用穩定的網路連結或嘗試繞過網路干預。

## 如何更新至最新版本？
- **問題**:
我想使用最新版本的一些功能，如何更新它？

- **回答**:
`pip install -U pdf2zh`


## 以下檔案不存在：example.pdf
- **問題**:
執行程序時，如果找不到文件，使用者會看到以下輸出：`以下檔案不存在：example.pdf`。

- **解決方案**:
  - 在檔案所在的目錄中開啟命令行，或
  - 直接在 pdf2zh 後輸入檔案的完整路徑，或
  - 使用互動模式 `pdf2zh -i` 直接拖放檔案


If you encounter SSL errors or other network-related issues when using **pdf2zh**, follow these steps to troubleshoot:

1. **Check Your Internet Connection**  
   Ensure that your device is connected to the internet and can access other websites.

2. **Verify the URL**  
   Make sure you are using the correct URL for the service. For example:  
   - `https://pdf2zh-next.com`  
   - `https://api.pdf2zh.com`

3. **Update Your System Time**  
   SSL certificates rely on accurate system time. If your device's time is incorrect, SSL validation may fail.

4. **Disable VPN or Proxy**  
   Some VPNs or proxies may interfere with SSL connections. Try disabling them temporarily.

5. **Clear Browser Cache**  
   Cached SSL certificates might be outdated. Clear your browser cache and restart the browser.

6. **Try Another Browser or Device**  
   If the issue persists, test the service on a different browser or device.

7. **Contact Support**  
   If none of the above steps resolve the issue, reach out to our [Community](#community) for assistance.

---

## SSL 錯誤與其他網路問題

如果您在使用 **pdf2zh** 時遇到 SSL 錯誤或其他與網路相關的問題，請按照以下步驟進行故障排除：

1. **檢查您的網路連線**  
   確保您的裝置已連接到網路，並且可以訪問其他網站。

2. **驗證網址**  
   確認您使用的是正確的服務網址。例如：  
   - `https://pdf2zh-next.com`  
   - `https://api.pdf2zh.com`

3. **更新系統時間**  
   SSL 憑證依賴準確的系統時間。如果您的裝置時間不正確，SSL 驗證可能會失敗。

4. **停用 VPN 或代理**  
   某些 VPN 或代理可能會干擾 SSL 連線。嘗試暫時停用它們。

5. **清除瀏覽器快取**  
   快取的 SSL 憑證可能已過期。清除瀏覽器快取並重新啟動瀏覽器。

6. **嘗試其他瀏覽器或裝置**  
   如果問題仍然存在，請在不同的瀏覽器或裝置上測試服務。

7. **聯繫支援**  
   如果上述步驟均無法解決問題，請聯繫我們的[社區](#社區)以獲得協助。
- **問題**:
在中國下載 hugging face 模型時，使用者可能會遇到網路錯誤。例如，在[issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55)、[#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70)中。

- **解決方案**:
  - [繞過防火長城](https://github.com/clash-verge-rev/clash-verge-rev).
  - [使用 Hugging Face 鏡像](https://hf-mirror.com/).
  - [使用便攜版本](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [改用 Docker](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [更新憑證](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests)，如[問題 #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55)所建議。

## 無法存取本地主機
請參閱下方內容。

## 使用 0.0.0.0 啟動 GUI 時出現錯誤
- **問題**:
在全域模式下使用代理軟體可能會導致 Gradio 無法正常啟動。例如，在 [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77) 中。

- **解決方案**:
使用規則模式

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>Some content on this page has been translated by GPT and may contain errors.</small></h6>