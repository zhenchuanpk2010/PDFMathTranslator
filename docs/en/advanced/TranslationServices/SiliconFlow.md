# SiliconFlow

## Free Translation Service

[SiliconFlow](https://siliconflow.cn) provides free translation service for this project.

Currently, the free translation service will use `THUDM/GLM-4-9B-0414` model.

### Usage

#### cli

```bash
pdf2zh_next --siliconflowfree example.pdf 
```

#### webui

1. Select "SiliconFlowFree" from the "Translation Options" - "Service" dropdown list.
2. Click the Translate button at the bottom of the page to start translation.
3. After translation is complete, you can find the translated PDF file in the "Translated" section at the bottom of the page.


### Privacy Policy

The file content will be sent to the server of the project maintainer [@awwaawwa](https://github.com/awwaawwa), and then forwarded to SiliconFlow for translation.

The maintainers of this project will only collect error information returned by SiliconFlow for debugging related services. Your file content will not be collected.

SiliconFlow Privacy Policy: [简体中文](https://docs.siliconflow.cn/cn/legals/privacy-policy)/[English](https://docs.siliconflow.cn/en/legals/privacy-policy)



## Use other models from SiliconFlow

[SiliconFlow](https://siliconflow.cn) also provides other models for translation.

### Usage

1. Register an account at [SiliconFlow](https://siliconflow.cn)

2. Create an API key at [SiliconFlow API Key](https://cloud.siliconflow.cn/me/account/ak). Then, click on the key to copy it.

#### cli

```bash
pdf2zh_next --siliconflow --siliconflow-model "Pro/deepseek-ai/DeepSeek-V3" --siliconflow-api-key <your-api-key> example.pdf
```

#### webui

1. "Translation Options" - **"Service"** dropdown list: Select "SiliconFlow"
2. "Translation Options" - **"Base URL for SiliconFlow API"**: Keep default
3. "Translation Options" - **"SiliconFlow model to use"**: Enter "Pro/deepseek-ai/DeepSeek-V3" or other models
4. "Translation Options" - **"API key for SiliconFlow service"**: Paste your API key
5. Click the Translate button at the bottom of the page to start translation
6. After translation is complete, you can find the translated PDF file in the "Translated" section at the bottom of the page.


## Acknowledgement

Thanks to [SiliconFlow](https://siliconflow.cn) for providing free translation service for this project.

