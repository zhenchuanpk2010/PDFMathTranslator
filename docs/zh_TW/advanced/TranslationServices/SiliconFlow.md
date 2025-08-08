# SiliconFlow

## 免費翻譯服務

[SiliconFlow](https://siliconflow.cn) 為本專案提供免費翻譯服務。

目前，免費翻譯服務將使用 `THUDM/GLM-4-9B-0414` 模型。

### 如何使用

#### 命令行

```bash
pdf2zh_next --siliconflowfree example.pdf 
```

#### Web 使用者介面

1. 從「翻譯選項」-「服務」下拉選單中選擇「SiliconFlowFree」。
2. 點擊頁面底部的「翻譯」按鈕開始翻譯。
3. 翻譯完成後，您可以在頁面底部的「已翻譯」區塊中找到翻譯後的 `PDF` 文件。


### 隱私政策

檔案內容將會傳送至專案維護者 [@awwaawwa](https://github.com/awwaawwa) 的伺服器，然後轉發至 SiliconFlow 進行翻譯。

本專案維護者僅會收集 SiliconFlow 返回的錯誤資訊用於調試相關服務，不會收集您的檔案內容。

SiliconFlow 隱私政策：[简体中文](https://docs.siliconflow.cn/cn/legals/privacy-policy)/[English](https://docs.siliconflow.cn/en/legals/privacy-policy)



## 使用 SiliconFlow 的其他模型

[SiliconFlow](https://siliconflow.cn) 也提供其他翻譯模型。

### 如何使用

1. 在 [SiliconFlow](https://siliconflow.cn) 註冊一個帳號

2. 在 [SiliconFlow API Key](https://cloud.siliconflow.cn/me/account/ak) 創建一個 API 金鑰。然後，點擊金鑰以複製它。

#### 命令行

```bash
pdf2zh_next --siliconflow --siliconflow-model "Pro/deepseek-ai/DeepSeek-V3" --siliconflow-api-key <your-api-key> example.pdf
```

#### Web 使用者介面

1. "翻譯選項" - **"服務"** 下拉選單：選擇 "SiliconFlow"
2. "翻譯選項" - **"SiliconFlow API 基礎 URL"**：保持預設
3. "翻譯選項" - **"要使用的 SiliconFlow 模型"**：輸入 "Pro/deepseek-ai/DeepSeek-V3" 或其他模型
4. "翻譯選項" - **"SiliconFlow 服務的 API 金鑰"**：貼上您的 API 金鑰
5. 點擊頁面底部的「翻譯」按鈕開始翻譯
6. 翻譯完成後，您可以在頁面底部的「已翻譯」區塊找到翻譯好的 `PDF` 文件。


## 致謝

感謝 [SiliconFlow](https://siliconflow.cn) 為本專案提供免費翻譯服務。

<div align="right"> 
<h6><small>Some content on this page has been translated by GPT and may contain errors.</small></h6>