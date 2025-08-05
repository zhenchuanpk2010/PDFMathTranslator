<!-- CHUNK ID: chunk_16E46377  CHUNK TYPE: header START_LINE:1 -->
# SiliconFlow

<!-- CHUNK ID: chunk_5EFF4D9F  CHUNK TYPE: header START_LINE:3 -->
## Free Translation Service

<!-- CHUNK ID: chunk_3C2A41A9  CHUNK TYPE: paragraph START_LINE:5 -->
[SiliconFlow](https://siliconflow.cn) provides free translation service for this project.

Currently, the free translation service will use `THUDM/GLM-4-9B-0414` model.

<!-- CHUNK ID: chunk_047D6F23  CHUNK TYPE: header START_LINE:9 -->
### Usage

<!-- CHUNK ID: chunk_FC529C81  CHUNK TYPE: header START_LINE:11 -->
#### cli

<!-- CHUNK ID: chunk_EFB67255  CHUNK TYPE: code_block START_LINE:13 -->
```bash
pdf2zh_next --siliconflowfree example.pdf 
```

<!-- CHUNK ID: chunk_18E35DAE  CHUNK TYPE: header START_LINE:17 -->
#### webui

<!-- CHUNK ID: chunk_0ACD2D6C  CHUNK TYPE: list START_LINE:19 -->
1. Select "SiliconFlowFree" from the "Translation Options" - "Service" dropdown list.
2. Click the Translate button at the bottom of the page to start translation.
3. After translation is complete, you can find the translated PDF file in the "Translated" section at the bottom of the page.


<!-- CHUNK ID: chunk_24653E80  CHUNK TYPE: header START_LINE:24 -->
### Privacy Policy

<!-- CHUNK ID: chunk_E40E083F  CHUNK TYPE: paragraph START_LINE:26 -->
The file content will be sent to the server of the project maintainer [@awwaawwa](https://github.com/awwaawwa), and then forwarded to SiliconFlow for translation.

The maintainers of this project will only collect error information returned by SiliconFlow for debugging related services. Your file content will not be collected.

SiliconFlow Privacy Policy: [简体中文](https://docs.siliconflow.cn/cn/legals/privacy-policy)/[English](https://docs.siliconflow.cn/en/legals/privacy-policy)



<!-- CHUNK ID: chunk_86238772  CHUNK TYPE: header START_LINE:34 -->
## Use other models from SiliconFlow

<!-- CHUNK ID: chunk_6C8B20F2  CHUNK TYPE: paragraph START_LINE:36 -->
[SiliconFlow](https://siliconflow.cn) also provides other models for translation.

<!-- CHUNK ID: chunk_047D6F23  CHUNK TYPE: header START_LINE:38 -->
### Usage

<!-- CHUNK ID: chunk_71BE5099  CHUNK TYPE: list START_LINE:40 -->
1. Register an account at [SiliconFlow](https://siliconflow.cn)

2. Create an API key at [SiliconFlow API Key](https://cloud.siliconflow.cn/me/account/ak). Then, click on the key to copy it.

<!-- CHUNK ID: chunk_FC529C81  CHUNK TYPE: header START_LINE:44 -->
#### cli

<!-- CHUNK ID: chunk_E17980A8  CHUNK TYPE: code_block START_LINE:46 -->
```bash
pdf2zh_next --siliconflow --siliconflow-model "Pro/deepseek-ai/DeepSeek-V3" --siliconflow-api-key <your-api-key> example.pdf
```

<!-- CHUNK ID: chunk_18E35DAE  CHUNK TYPE: header START_LINE:50 -->
#### webui

<!-- CHUNK ID: chunk_22AE44AB  CHUNK TYPE: list START_LINE:52 -->
1. "Translation Options" - **"Service"** dropdown list: Select "SiliconFlow"
2. "Translation Options" - **"Base URL for SiliconFlow API"**: Keep default
3. "Translation Options" - **"SiliconFlow model to use"**: Enter "Pro/deepseek-ai/DeepSeek-V3" or other models
4. "Translation Options" - **"API key for SiliconFlow service"**: Paste your API key
5. Click the Translate button at the bottom of the page to start translation
6. After translation is complete, you can find the translated PDF file in the "Translated" section at the bottom of the page.


<!-- CHUNK ID: chunk_F44132D0  CHUNK TYPE: header START_LINE:60 -->
## Acknowledgement

<!-- CHUNK ID: chunk_ED8820C9  CHUNK TYPE: paragraph START_LINE:62 -->
Thanks to [SiliconFlow](https://siliconflow.cn) for providing free translation service for this project.

