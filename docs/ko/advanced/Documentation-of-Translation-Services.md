[**고급 옵션**](./introduction.md) > **번역 서비스 문서** _(current)_

---

### 명령줄을 통해 사용 가능한 번역 서비스 확인하기

사용 가능한 번역 서비스와 사용법을 확인하려면 명령줄에서 도움말 메시지를 출력하면 됩니다.

```bash
pdf2zh_next -h
```

도움말 메시지의 끝에서 다양한 번역 서비스에 대한 자세한 정보를 확인할 수 있습니다.

---

> [!CAUTION]
> 다음 내용은 pdf2zh 버전 1.x 를 위해 준비되었으며, 아직 버전 2.x 로 업데이트되지 않았습니다. 따라서 정보가 **구식**일 수 있습니다.
>
> 이 경고 메시지는 문서 내용이 새 버전과 일치하게 되면 제거될 예정입니다.

* [Google Translate](https://cloud.google.com/translate/docs)
* [DeepL](https://developers.deepl.com/docs/api-reference/translate)
* [DeepLX](https://github.com/OwO-Network/DeepLX)
* [OpenAI](https://platform.openai.com/docs/api-reference/introduction)
* [Ollama](https://github.com/ollama/ollama/blob/main/docs/api.md)
* [Azure](https://learn.microsoft.com/en-us/azure/ai-services/translator/)
* [Zhipu](https://bigmodel.cn/)
* [DeepSeek](https://api-docs.deepseek.com/)

#### 다른 서비스로 번역하기

각 번역 서비스에 필요한 [환경 변수](https://chatgpt.com/share/6734a83d-9d48-800e-8a46-f57ca6e8bcb4)에 대한 상세한 표를 제공했습니다. 해당 서비스를 사용하기 전에 반드시 설정하세요.

| **번역기**           | **서비스**     | **환경 변수**                                                         | **기본값**                                               | **참고 사항**                                                                                                                                                                                                              |
| -------------------- | -------------- | --------------------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Google (기본값)**  | `google`       | 없음                                                                  | 해당 없음                                               | 없음                                                                                                                                                                                                                       |
| **Bing**             | `bing`         | None                                                                  | N/A                                                      | None                                                                                                                                                                                                                       |
| **DeepL**            | `deepl`        | `DEEPL_AUTH_KEY`                                                      | `[Your Key]`                                             | [DeepL](https://support.deepl.com/hc/en-us/articles/360020695820-API-Key-for-DeepL-s-API) 참조                                                                                                                              |
| **DeepLX**           | `deeplx`       | `DEEPLX_ENDPOINT`                                                     | `https://api.deepl.com/translate`                        | [DeepLX](https://github.com/OwO-Network/DeepLX) 참조                                                                                                                                                                        |
| **Ollama**           | `ollama`       | `OLLAMA_HOST`, `OLLAMA_MODEL`                                         | `http://127.0.0.1:11434`, `gemma2`                       | [Ollama](https://github.com/ollama/ollama) 참조                                                                                                                                                                             |
| **Xinference**       | `xinference`   | `XINFERENCE_HOST`, `XINFERENCE_MODEL`                                 | `http://127.0.0.1:9997`, `gemma-2-it`                    | [Xinference](https://github.com/xorbitsai/inference) 참조                                                                                                                                                                   |
| **OpenAI**           | `openai`       | `OPENAI_BASE_URL`, `OPENAI_API_KEY`, `OPENAI_MODEL`                   | `https://api.openai.com/v1`, `[Your Key]`, `gpt-4o-mini` | [OpenAI](https://platform.openai.com/docs/overview) 참조                                                                                                                                                                    |
| **AzureOpenAI**      | `azure-openai` | `AZURE_OPENAI_BASE_URL`, `AZURE_OPENAI_API_KEY`, `AZURE_OPENAI_MODEL` | `[Your Endpoint]`, `[Your Key]`, `gpt-4o-mini`           | [Azure OpenAI](https://learn.microsoft.com/zh-cn/azure/ai-services/openai/chatgpt-quickstart?tabs=command-line%2Cjavascript-keyless%2Ctypescript-keyless%2Cpython&pivots=programming-language-python) 참조                  |
| **Zhipu**            | `zhipu`        | `ZHIPU_API_KEY`, `ZHIPU_MODEL`                                        | `[Your Key]`, `glm-4-flash`                              | [Zhipu](https://open.bigmodel.cn/dev/api/thirdparty-frame/openai-sdk) 참조                                                                                                                                                  |
| **ModelScope**       | `ModelScope`   | `MODELSCOPE_API_KEY`, `MODELSCOPE_MODEL`                              | `[Your Key]`, `Qwen/Qwen2.5-Coder-32B-Instruct`          | [ModelScope](https://www.modelscope.cn/docs/model-service/API-Inference/intro) 참조                                                                                                                                         |
| **Silicon**          | `silicon`      | `SILICON_API_KEY`, `SILICON_MODEL`                                    | `[Your Key]`, `Qwen/Qwen2.5-7B-Instruct`                 | [SiliconCloud](https://docs.siliconflow.cn/quickstart) 문서 참조                                                                                                                                                                 |
| **Gemini**           | `gemini`       | `GEMINI_API_KEY`, `GEMINI_MODEL`                                      | `[Your Key]`, `gemini-1.5-flash`                         | [Gemini](https://ai.google.dev/gemini-api/docs/openai) 참조                                                                                                                                                                 |
| **Azure**            | `azure`        | `AZURE_ENDPOINT`, `AZURE_API_KEY`                                     | `https://api.translator.azure.cn`, `[Your Key]`          | [Azure](https://docs.azure.cn/en-us/ai-services/translator/text-translation-overview) 참조                                                                                                                                  |
| **Tencent**          | `tencent`      | `TENCENTCLOUD_SECRET_ID`, `TENCENTCLOUD_SECRET_KEY`                   | `[Your ID]`, `[Your Key]`                                | [Tencent](https://www.tencentcloud.com/products/tmt?from_qcintl=122110104) 참조                                                                                                                                             |
| **Dify**             | `dify`         | `DIFY_API_URL`, `DIFY_API_KEY`                                        | `[Your DIFY URL]`, `[Your Key]`                          | [Dify](https://github.com/langgenius/dify) 참조, Dify 의 워크플로우 입력에서 lang_out, lang_in, text 세 가지 변수를 정의해야 합니다.                                                                                  |
| **AnythingLLM**      | `anythingllm`  | `AnythingLLM_URL`, `AnythingLLM_APIKEY`                               | `[Your AnythingLLM URL]`, `[Your Key]`                   | [anything-llm](https://github.com/Mintplex-Labs/anything-llm) 참조                                                                                                                                                          |
| **Argos Translate**  | `argos`        |                                                                       |                                                          | [argos-translate](https://github.com/argosopentech/argos-translate) 참조                                                                                                                                                    |
| **Grok**             | `grok`         | `GORK_API_KEY`, `GORK_MODEL`                                          | `[Your GORK_API_KEY]`, `grok-2-1212`                     | [Grok](https://docs.x.ai/docs/overview) 참조                                                                                                                                                                                |
| **Groq**             | `groq`         | `GROQ_API_KEY`, `GROQ_MODEL`                                          | `[Your GROQ_API_KEY]`, `llama-3-3-70b-versatile`         | [Groq](https://console.groq.com/docs/models) 참조                                                                                                                                                                           |
| **DeepSeek**         | `deepseek`     | `DEEPSEEK_API_KEY`, `DEEPSEEK_MODEL`                                  | `[Your DEEPSEEK_API_KEY]`, `deepseek-chat`               | [DeepSeek](https://www.deepseek.com/) 참조                                                                                                                                                                                  |
| **OpenAI-Liked**     | `openailiked`  | `OPENAILIKED_BASE_URL`, `OPENAILIKED_API_KEY`, `OPENAILIKED_MODEL`    | `url`, `[Your Key]`, `model name`                        | None                                                                                                                                                                                                                       |
| **Ali Qwen Translation** | `qwen-mt`  | `ALI_MODEL`, `ALI_API_KEY`, `ALI_DOMAINS`                             | `qwen-mt-turbo`, `[Your Key]`, `scientific paper`        | 번체 중국어는 아직 지원되지 않으며, 간체 중국어로 번역됩니다. 자세한 내용은 [Qwen MT](https://bailian.console.aliyun.com/?spm=5176.28197581.0.0.72e329a4HRxe99#/model-market/detail/qwen-mt-turbo) 참조 |

위의 표에 나열되지 않았지만 OpenAI API 와 호환되는 대규모 언어 모델의 경우, 표에 설명된 OpenAI 와 동일한 방법으로 환경 변수를 설정할 수 있습니다.

`-s service` 또는 `-s service:model`을 사용하여 서비스를 지정하세요:

```bash
pdf2zh_next example.pdf -s openai:gpt-4o-mini
```

또는 환경 변수로 모델을 지정하세요:

```bash
set OPENAI_MODEL=gpt-4o-mini
pdf2zh_next example.pdf -s openai
```

PowerShell 사용자의 경우:

```shell
$env:OPENAI_MODEL = gpt-4o-mini
pdf2zh_next example.pdf -s openai
```

<div align="right"> 
<h6><small>이 페이지의 일부 내용은 GPT 에 의해 번역되었으며 오류가 포함될 수 있습니다.</small></h6>