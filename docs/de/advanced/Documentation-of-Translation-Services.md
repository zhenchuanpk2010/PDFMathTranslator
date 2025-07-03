[**Erweiterte Optionen**](./introduction.md) > **Dokumentation der Übersetzungsdienste** _(aktuell)_

---

### Anzeige verfügbarer Übersetzungsdienste über die Kommandozeile

Sie können die verfügbaren Übersetzungsdienste und ihre Verwendung bestätigen, indem Sie die Hilfenachricht in der Kommandozeile ausgeben.

```bash
pdf2zh_next -h
```

Am Ende der Hilfenachricht können Sie detaillierte Informationen zu den verschiedenen Übersetzungsdiensten einsehen.

---

> [!CAUTION]
> Der folgende Inhalt wurde für Version 1.x von pdf2zh vorbereitet und wurde noch nicht für Version 2.x aktualisiert. Daher können die Informationen **veraltet** sein.
>
> Diese Warnmeldung wird entfernt, sobald der Artikelinhalt mit der neuen Version übereinstimmt.

* [Google Translate](https://cloud.google.com/translate/docs)
* [DeepL](https://developers.deepl.com/docs/api-reference/translate)
* [DeepLX](https://github.com/OwO-Network/DeepLX)
* [OpenAI](https://platform.openai.com/docs/api-reference/introduction)
* [Ollama](https://github.com/ollama/ollama/blob/main/docs/api.md)
* [Azure](https://learn.microsoft.com/en-us/azure/ai-services/translator/)
* [Zhipu](https://bigmodel.cn/)
* [DeepSeek](https://api-docs.deepseek.com/)

#### Übersetzen mit verschiedenen Diensten

Wir haben eine detaillierte Tabelle zu den erforderlichen [Umgebungsvariablen](https://chatgpt.com/share/6734a83d-9d48-800e-8a46-f57ca6e8bcb4) für jeden Übersetzungsdienst bereitgestellt. Stellen Sie sicher, dass Sie diese einrichten, bevor Sie den jeweiligen Dienst nutzen.

| **Translator**       | **Service**    | **Environment Variables**                                             | **Default Values**                                       | **Notes**                                                                                                                                                                                                                  |
| -------------------- | -------------- | --------------------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Google (Standard)** | `google`       | Keine                                                                 | N/A                                                      | Keine                                                                                                                                                                                                                      |
| **Bing**             | `bing`         | None                                                                  | N/A                                                      | None                                                                                                                                                                                                                       |
| **DeepL**            | `deepl`        | `DEEPL_AUTH_KEY`                                                      | `[Your Key]`                                             | Siehe [DeepL](https://support.deepl.com/hc/en-us/articles/360020695820-API-Key-for-DeepL-s-API)                                                                                                                              |
| **DeepLX**           | `deeplx`       | `DEEPLX_ENDPOINT`                                                     | `https://api.deepl.com/translate`                        | Siehe [DeepLX](https://github.com/OwO-Network/DeepLX)                                                                                                                                                                        |
| **Ollama**           | `ollama`       | `OLLAMA_HOST`, `OLLAMA_MODEL`                                         | `http://127.0.0.1:11434`, `gemma2`                       | Siehe [Ollama](https://github.com/ollama/ollama)                                                                                                                                                                             |
| **Xinference**       | `xinference`   | `XINFERENCE_HOST`, `XINFERENCE_MODEL`                                 | `http://127.0.0.1:9997`, `gemma-2-it`                    | Siehe [Xinference](https://github.com/xorbitsai/inference)                                                                                                                                                                   |
| **OpenAI**           | `openai`       | `OPENAI_BASE_URL`, `OPENAI_API_KEY`, `OPENAI_MODEL`                   | `https://api.openai.com/v1`, `[Ihr Schlüssel]`, `gpt-4o-mini` | Siehe [OpenAI](https://platform.openai.com/docs/overview)                                                                                                                                                                    |
| **AzureOpenAI**      | `azure-openai` | `AZURE_OPENAI_BASE_URL`, `AZURE_OPENAI_API_KEY`, `AZURE_OPENAI_MODEL` | `[Ihr Endpunkt]`, `[Ihr Schlüssel]`, `gpt-4o-mini`           | Siehe [Azure OpenAI](https://learn.microsoft.com/zh-cn/azure/ai-services/openai/chatgpt-quickstart?tabs=command-line%2Cjavascript-keyless%2Ctypescript-keyless%2Cpython&pivots=programming-language-python)                  |
| **Zhipu**            | `zhipu`        | `ZHIPU_API_KEY`, `ZHIPU_MODEL`                                        | `[Your Key]`, `glm-4-flash`                              | Siehe [Zhipu](https://open.bigmodel.cn/dev/api/thirdparty-frame/openai-sdk)                                                                                                                                                  |
| **ModelScope**       | `ModelScope`   | `MODELSCOPE_API_KEY`, `MODELSCOPE_MODEL`                              | `[Your Key]`, `Qwen/Qwen2.5-Coder-32B-Instruct`          | Siehe [ModelScope](https://www.modelscope.cn/docs/model-service/API-Inference/intro)                                                                                                                                         |
| **Silicon**          | `silicon`      | `SILICON_API_KEY`, `SILICON_MODEL`                                    | `[Your Key]`, `Qwen/Qwen2.5-7B-Instruct`                 | Siehe [SiliconCloud](https://docs.siliconflow.cn/quickstart)                                                                                                                                                                 |
| **Gemini**           | `gemini`       | `GEMINI_API_KEY`, `GEMINI_MODEL`                                      | `[Your Key]`, `gemini-1.5-flash`                         | Siehe [Gemini](https://ai.google.dev/gemini-api/docs/openai)                                                                                                                                                                 |
| **Azure**            | `azure`        | `AZURE_ENDPOINT`, `AZURE_API_KEY`                                     | `https://api.translator.azure.cn`, `[Your Key]`          | Siehe [Azure](https://docs.azure.cn/en-us/ai-services/translator/text-translation-overview)                                                                                                                                  |
| **Tencent**          | `tencent`      | `TENCENTCLOUD_SECRET_ID`, `TENCENTCLOUD_SECRET_KEY`                   | `[Your ID]`, `[Your Key]`                                | Siehe [Tencent](https://www.tencentcloud.com/products/tmt?from_qcintl=122110104)                                                                                                                                             |
| **Dify**             | `dify`         | `DIFY_API_URL`, `DIFY_API_KEY`                                        | `[Ihre DIFY URL]`, `[Ihr Schlüssel]`                          | Siehe [Dify](https://github.com/langgenius/dify), Drei Variablen, lang_out, lang_in und text, müssen im Workflow-Input von Dify definiert werden.                                                                                  |
| **AnythingLLM**      | `anythingllm`  | `AnythingLLM_URL`, `AnythingLLM_APIKEY`                               | `[Ihre AnythingLLM URL]`, `[Ihr Schlüssel]`                   | Siehe [anything-llm](https://github.com/Mintplex-Labs/anything-llm)                                                                                                                                                          |
| **Argos Translate**  | `argos`        |                                                                       |                                                          | Siehe [argos-translate](https://github.com/argosopentech/argos-translate)                                                                                                                                                    |
| **Grok**             | `grok`         | `GORK_API_KEY`, `GORK_MODEL`                                          | `[Your GORK_API_KEY]`, `grok-2-1212`                     | Siehe [Grok](https://docs.x.ai/docs/overview)                                                                                                                                                                                |
| **Groq**             | `groq`         | `GROQ_API_KEY`, `GROQ_MODEL`                                          | `[Your GROQ_API_KEY]`, `llama-3-3-70b-versatile`         | Siehe [Groq](https://console.groq.com/docs/models)                                                                                                                                                                           |
| **DeepSeek**         | `deepseek`     | `DEEPSEEK_API_KEY`, `DEEPSEEK_MODEL`                                  | `[Your DEEPSEEK_API_KEY]`, `deepseek-chat`               | Siehe [DeepSeek](https://www.deepseek.com/)                                                                                                                                                                                  |
| **OpenAI-Liked**     | `openailiked`  | `OPENAILIKED_BASE_URL`, `OPENAILIKED_API_KEY`, `OPENAILIKED_MODEL`    | `url`, `[Your Key]`, `model name`                        | None                                                                                                                                                                                                                       |
| **Ali Qwen Translation** | `qwen-mt`  | `ALI_MODEL`, `ALI_API_KEY`, `ALI_DOMAINS`                             | `qwen-mt-turbo`, `[Your Key]`, `scientific paper`        | Traditionelles Chinesisch wird noch nicht unterstützt, es wird in vereinfachtes Chinesisch übersetzt. Weitere Informationen finden Sie unter [Qwen MT](https://bailian.console.aliyun.com/?spm=5176.28197581.0.0.72e329a4HRxe99#/model-market/detail/qwen-mt-turbo) |

Für große Sprachmodelle, die mit der OpenAI API kompatibel sind, aber nicht in der obigen Tabelle aufgeführt sind, können Sie Umgebungsvariablen mit der gleichen Methode festlegen, die für OpenAI in der Tabelle beschrieben ist.

Verwenden Sie `-s service` oder `-s service:model`, um den Dienst anzugeben:

```bash
pdf2zh_next example.pdf -s openai:gpt-4o-mini
```

Oder geben Sie das Modell mit Umgebungsvariablen an:

```bash
set OPENAI_MODEL=gpt-4o-mini
pdf2zh_next example.pdf -s openai
```

Für PowerShell-Benutzer:

```shell
$env:OPENAI_MODEL = gpt-4o-mini
pdf2zh_next example.pdf -s openai
```

<div align="right"> 
<h6><small>Ein Teil des Inhalts dieser Seite wurde von GPT übersetzt und kann Fehler enthalten.</small></h6>