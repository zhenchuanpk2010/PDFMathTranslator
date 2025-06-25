[**Opciones avanzadas**](./introduction.md) > **Documentación de servicios de traducción** _(actual)_

---

### Visualización de servicios de traducción disponibles mediante la línea de comandos

Puedes confirmar los servicios de traducción disponibles y su uso imprimiendo el mensaje de ayuda en la línea de comandos.

```bash
pdf2zh_next -h
```

Al final del mensaje de ayuda, puedes ver información detallada sobre los diferentes servicios de traducción.

---

> [!CAUTION]
> El siguiente contenido fue preparado para la versión 1.x de pdf2zh y aún no se ha actualizado para la versión 2.x. Por lo tanto, la información puede estar **desactualizada**.
>
> Este mensaje de advertencia se eliminará una vez que el contenido del artículo se alinee con la nueva versión.

* [Google Translate](https://cloud.google.com/translate/docs)
* [DeepL](https://developers.deepl.com/docs/api-reference/translate)
* [DeepLX](https://github.com/OwO-Network/DeepLX)
* [OpenAI](https://platform.openai.com/docs/api-reference/introduction)
* [Ollama](https://github.com/ollama/ollama/blob/main/docs/api.md)
* [Azure](https://learn.microsoft.com/en-us/azure/ai-services/translator/)
* [Zhipu](https://bigmodel.cn/)
* [DeepSeek](https://api-docs.deepseek.com/)

#### Traducir con diferentes servicios

Hemos proporcionado una tabla detallada sobre las [variables de entorno](https://chatgpt.com/share/6734a83d-9d48-800e-8a46-f57ca6e8bcb4) requeridas para cada servicio de traducción. Asegúrate de configurarlas antes de usar el servicio respectivo.

| **Traductor**       | **Servicio**    | **Variables de entorno**                                             | **Valores predeterminados**                                       | **Notas**                                                                                                                                                                                                                  |
| -------------------- | -------------- | --------------------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Google (Predeterminado)** | `google`       | Ninguna                                                                  | N/A                                                      | Ninguna                                                                                                                                                                                                                       |
| **Bing**             | `bing`         | Ninguno                                                                  | N/A                                                      | Ninguno                                                                                                                                                                                                                       |
| **DeepL**            | `deepl`        | `DEEPL_AUTH_KEY`                                                      | `[Tu clave]`                                             | Consulta [DeepL](https://support.deepl.com/hc/en-us/articles/360020695820-API-Key-for-DeepL-s-API)                                                                                                                              |
| **DeepLX**           | `deeplx`       | `DEEPLX_ENDPOINT`                                                     | `https://api.deepl.com/translate`                        | Ver [DeepLX](https://github.com/OwO-Network/DeepLX)                                                                                                                                                                        |
| **Ollama**           | `ollama`       | `OLLAMA_HOST`, `OLLAMA_MODEL`                                         | `http://127.0.0.1:11434`, `gemma2`                       | Ver [Ollama](https://github.com/ollama/ollama)                                                                                                                                                                             |
| **Xinference**       | `xinference`   | `XINFERENCE_HOST`, `XINFERENCE_MODEL`                                 | `http://127.0.0.1:9997`, `gemma-2-it`                    | Consulta [Xinference](https://github.com/xorbitsai/inference)                                                                                                                                                                   |
| **OpenAI**           | `openai`       | `OPENAI_BASE_URL`, `OPENAI_API_KEY`, `OPENAI_MODEL`                   | `https://api.openai.com/v1`, `[Tu Clave]`, `gpt-4o-mini` | Consulta la [Documentación de OpenAI](https://platform.openai.com/docs/overview)                                                                                                                                                                    |
| **AzureOpenAI**      | `azure-openai` | `AZURE_OPENAI_BASE_URL`, `AZURE_OPENAI_API_KEY`, `AZURE_OPENAI_MODEL` | `[Tu Endpoint]`, `[Tu Clave]`, `gpt-4o-mini`           | Consulta [Azure OpenAI](https://learn.microsoft.com/zh-cn/azure/ai-services/openai/chatgpt-quickstart?tabs=command-line%2Cjavascript-keyless%2Ctypescript-keyless%2Cpython&pivots=programming-language-python)                  |
| **Zhipu**            | `zhipu`        | `ZHIPU_API_KEY`, `ZHIPU_MODEL`                                        | `[Tu Clave]`, `glm-4-flash`                              | Ver [Zhipu](https://open.bigmodel.cn/dev/api/thirdparty-frame/openai-sdk)                                                                                                                                                  |
| **ModelScope**       | `ModelScope`   | `MODELSCOPE_API_KEY`, `MODELSCOPE_MODEL`                              | `[Tu Clave]`, `Qwen/Qwen2.5-Coder-32B-Instruct`          | Consulta [ModelScope](https://www.modelscope.cn/docs/model-service/API-Inference/intro)                                                                                                                                         |
| **Silicon**          | `silicon`      | `SILICON_API_KEY`, `SILICON_MODEL`                                    | `[Tu clave]`, `Qwen/Qwen2.5-7B-Instruct`                 | Consulta [SiliconCloud](https://docs.siliconflow.cn/quickstart)                                                                                                                                                                 |
| **Gemini**           | `gemini`       | `GEMINI_API_KEY`, `GEMINI_MODEL`                                      | `[Tu Clave]`, `gemini-1.5-flash`                         | Consulta [Gemini](https://ai.google.dev/gemini-api/docs/openai)                                                                                                                                                                 |
| **Azure**            | `azure`        | `AZURE_ENDPOINT`, `AZURE_API_KEY`                                     | `https://api.translator.azure.cn`, `[Tu Clave]`          | Consulta [Azure](https://docs.azure.cn/en-us/ai-services/translator/text-translation-overview)                                                                                                                                  |
| **Tencent**          | `tencent`      | `TENCENTCLOUD_SECRET_ID`, `TENCENTCLOUD_SECRET_KEY`                   | `[Tu ID]`, `[Tu Clave]`                                | Consulta [Tencent](https://www.tencentcloud.com/products/tmt?from_qcintl=122110104)                                                                                                                                             |
| **Dify**             | `dify`         | `DIFY_API_URL`, `DIFY_API_KEY`                                        | `[Tu URL de DIFY]`, `[Tu Clave]`                          | Consulta [Dify](https://github.com/langgenius/dify), Tres variables, lang_out, lang_in y text, deben definirse en la entrada del flujo de trabajo de Dify.                                                                                  |
| **AnythingLLM**      | `anythingllm`  | `AnythingLLM_URL`, `AnythingLLM_APIKEY`                               | `[Tu URL de AnythingLLM]`, `[Tu Clave]`                   | Consulta [anything-llm](https://github.com/Mintplex-Labs/anything-llm)                                                                                                                                                          |
| **Argos Translate**  | `argos`        |                                                                       |                                                          | Ver [argos-translate](https://github.com/argosopentech/argos-translate)                                                                                                                                                    |
| **Grok**             | `grok`         | `GORK_API_KEY`, `GORK_MODEL`                                          | `[Tu GORK_API_KEY]`, `grok-2-1212`                     | Consulta [Grok](https://docs.x.ai/docs/overview)                                                                                                                                                                                |
| **Groq**             | `groq`         | `GROQ_API_KEY`, `GROQ_MODEL`                                          | `[Tu GROQ_API_KEY]`, `llama-3-3-70b-versatile`         | Consulta [Groq](https://console.groq.com/docs/models)                                                                                                                                                                           |
| **DeepSeek**         | `deepseek`     | `DEEPSEEK_API_KEY`, `DEEPSEEK_MODEL`                                  | `[Tu DEEPSEEK_API_KEY]`, `deepseek-chat`               | Consulta [DeepSeek](https://www.deepseek.com/)                                                                                                                                                                                  |
| **OpenAI-Liked**     | `openailiked`  | `OPENAILIKED_BASE_URL`, `OPENAILIKED_API_KEY`, `OPENAILIKED_MODEL`    | `url`, `[Tu Clave]`, `nombre del modelo`                        | Ninguno                                                                                                                                                                                                                       |
| **Ali Qwen Translation** | `qwen-mt`  | `ALI_MODEL`, `ALI_API_KEY`, `ALI_DOMAINS`                             | `qwen-mt-turbo`, `[Tu Clave]`, `scientific paper`        | El chino tradicional aún no es compatible, se traducirá al chino simplificado. Más información en [Qwen MT](https://bailian.console.aliyun.com/?spm=5176.28197581.0.0.72e329a4HRxe99#/model-market/detail/qwen-mt-turbo) |

Para modelos de lenguaje grandes que son compatibles con la API de OpenAI pero no están listados en la tabla anterior, puedes configurar variables de entorno utilizando el mismo método descrito para OpenAI en la tabla.

Usa `-s servicio` o `-s servicio:modelo` para especificar el servicio:

```bash
pdf2zh_next example.pdf -s openai:gpt-4o-mini
```

O especifique el modelo con variables de entorno:

```bash
set OPENAI_MODEL=gpt-4o-mini
pdf2zh_next example.pdf -s openai
```

Para usuarios de PowerShell:

```shell
$env:OPENAI_MODEL = gpt-4o-mini
pdf2zh_next example.pdf -s openai
```

<div align="right"> 
<h6><small>Parte del contenido de esta página ha sido traducido por GPT y puede contener errores.</small></h6>