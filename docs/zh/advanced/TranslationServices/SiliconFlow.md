# SiliconFlow

## 免费翻译服务

[SiliconFlow](https://siliconflow.cn) 为本项目提供免费翻译服务。

目前，免费翻译服务将使用 `THUDM/GLM-4-9B-0414` 模型。

### 如何使用

#### 命令行

```bash
pdf2zh_next --siliconflowfree example.pdf 
```

#### Web 界面

1. 从「Translation Options」-「Service」下拉列表中选择「SiliconFlowFree」。  
2. 点击页面底部的「Translate」按钮开始翻译。  
3. 翻译完成后，您可以在页面底部的「Translated」部分找到翻译好的 `PDF` 文件。


### 隐私政策

文件内容将被发送至项目维护者 [@awwaawwa](https://github.com/awwaawwa) 的服务器，随后转发至 SiliconFlow 进行翻译。

本项目维护者仅会收集 SiliconFlow 返回的错误信息用于调试相关服务，不会收集您的文件内容。

SiliconFlow 隐私政策：[简体中文](https://docs.siliconflow.cn/cn/legals/privacy-policy)/[English](https://docs.siliconflow.cn/en/legals/privacy-policy)



## 使用 SiliconFlow 的其他模型

[SiliconFlow](https://siliconflow.cn) 还提供了其他用于翻译的模型。

### 如何使用

1. 在 [SiliconFlow](https://siliconflow.cn) 注册账号

2. 在 [SiliconFlow API Key](https://cloud.siliconflow.cn/me/account/ak) 创建 API 密钥。然后，点击密钥进行复制。

#### 命令行

```bash
pdf2zh_next --siliconflow --siliconflow-model "Pro/deepseek-ai/DeepSeek-V3" --siliconflow-api-key <your-api-key> example.pdf
```

#### Web 界面

1. "翻译选项" - **"服务"** 下拉列表：选择 "SiliconFlow"
2. "翻译选项" - **"SiliconFlow API 基础 URL"**：保持默认
3. "翻译选项" - **"要使用的 SiliconFlow 模型"**：输入 "Pro/deepseek-ai/DeepSeek-V3" 或其他模型
4. "翻译选项" - **"SiliconFlow 服务的 API 密钥"**：粘贴您的 API 密钥
5. 点击页面底部的翻译按钮开始翻译
6. 翻译完成后，您可以在页面底部的 "已翻译" 部分找到翻译好的 PDF 文件。


## 致谢

感谢 [SiliconFlow](https://siliconflow.cn) 为本项目提供免费翻译服务。

<div align="right"> 
<h6><small>本页面的部分内容由 GPT 翻译，可能包含错误。</small></h6>