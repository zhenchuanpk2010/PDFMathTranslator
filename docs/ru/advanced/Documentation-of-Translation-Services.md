[**Расширенные параметры**](./introduction.md) > **Документация служб перевода** _(current)_

---

### Просмотр доступных служб перевода через Командную строку

Вы можете проверить доступные службы перевода и их использование, напечатав сообщение справки в командной строке.

```bash
pdf2zh_next -h
```

В конце сообщения справки вы можете просмотреть подробную информацию о различных службах перевода.

---

> [!CAUTION]
> Следующее содержимое было подготовлено для версии 1.x pdf2zh и еще не обновлено для версии 2.x. Поэтому информация может быть **устаревшей**.
>
> Это предупреждение будет удалено, как только содержимое статьи будет соответствовать новой версии.

* [Google Translate](https://cloud.google.com/translate/docs)
* [DeepL](https://developers.deepl.com/docs/api-reference/translate)
* [DeepLX](https://github.com/OwO-Network/DeepLX)
* [OpenAI](https://platform.openai.com/docs/api-reference/introduction)
* [Ollama](https://github.com/ollama/ollama/blob/main/docs/api.md)
* [Azure](https://learn.microsoft.com/en-us/azure/ai-services/translator/)
* [Zhipu](https://bigmodel.cn/)
* [DeepSeek](https://api-docs.deepseek.com/)

#### Перевод с использованием различных сервисов

Мы предоставили подробную таблицу с необходимыми [переменными окружения](https://chatgpt.com/share/6734a83d-9d48-800e-8a46-f57ca6e8bcb4) для каждой службы перевода. Убедитесь, что вы установили их перед использованием соответствующего сервиса.

| **Переводчик**       | **Сервис**    | **Переменные окружения**                                             | **Значения по умолчанию**                                       | **Примечания**                                                                                                                                                                                                                  |
| -------------------- | -------------- | --------------------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Google (По умолчанию)** | `google`       | None                                                                  | N/A                                                      | None                                                                                                                                                                                                                       |
| **Bing**             | `bing`         | None                                                                  | N/A                                                      | None                                                                                                                                                                                                                       |
| **DeepL**            | `deepl`        | `DEEPL_AUTH_KEY`                                                      | `[Your Key]`                                             | См. [DeepL](https://support.deepl.com/hc/en-us/articles/360020695820-API-Key-for-DeepL-s-API)                                                                                                                              |
| **DeepLX**           | `deeplx`       | `DEEPLX_ENDPOINT`                                                     | `https://api.deepl.com/translate`                        | См. [DeepLX](https://github.com/OwO-Network/DeepLX)                                                                                                                                                                        |
| **Ollama**           | `ollama`       | `OLLAMA_HOST`, `OLLAMA_MODEL`                                         | `http://127.0.0.1:11434`, `gemma2`                       | См. [Ollama](https://github.com/ollama/ollama)                                                                                                                                                                             |
| **Xinference**       | `xinference`   | `XINFERENCE_HOST`, `XINFERENCE_MODEL`                                 | `http://127.0.0.1:9997`, `gemma-2-it`                    | См. [Xinference](https://github.com/xorbitsai/inference)                                                                                                                                                                   |
| **OpenAI**           | `openai`       | `OPENAI_BASE_URL`, `OPENAI_API_KEY`, `OPENAI_MODEL`                   | `https://api.openai.com/v1`, `[Your Key]`, `gpt-4o-mini` | См. [OpenAI](https://platform.openai.com/docs/overview)                                                                                                                                                                    |
| **AzureOpenAI**      | `azure-openai` | `AZURE_OPENAI_BASE_URL`, `AZURE_OPENAI_API_KEY`, `AZURE_OPENAI_MODEL` | `[Your Endpoint]`, `[Your Key]`, `gpt-4o-mini`           | См. [Azure OpenAI](https://learn.microsoft.com/zh-cn/azure/ai-services/openai/chatgpt-quickstart?tabs=command-line%2Cjavascript-keyless%2Ctypescript-keyless%2Cpython&pivots=programming-language-python)                  |
| **Zhipu**            | `zhipu`        | `ZHIPU_API_KEY`, `ZHIPU_MODEL`                                        | `[Your Key]`, `glm-4-flash`                              | См. [Zhipu](https://open.bigmodel.cn/dev/api/thirdparty-frame/openai-sdk)                                                                                                                                                  |
| **ModelScope**       | `ModelScope`   | `MODELSCOPE_API_KEY`, `MODELSCOPE_MODEL`                              | `[Ваш ключ]`, `Qwen/Qwen2.5-Coder-32B-Instruct`          | См. [ModelScope](https://www.modelscope.cn/docs/model-service/API-Inference/intro)                                                                                                                                         |
| **Silicon**          | `silicon`      | `SILICON_API_KEY`, `SILICON_MODEL`                                    | `[Ваш ключ]`, `Qwen/Qwen2.5-7B-Instruct`                 | См. [SiliconCloud](https://docs.siliconflow.cn/quickstart)                                                                                                                                                                 |
| **Gemini**           | `gemini`       | `GEMINI_API_KEY`, `GEMINI_MODEL`                                      | `[Your Key]`, `gemini-1.5-flash`                         | См. [Gemini](https://ai.google.dev/gemini-api/docs/openai)                                                                                                                                                                 |
| **Azure**            | `azure`        | `AZURE_ENDPOINT`, `AZURE_API_KEY`                                     | `https://api.translator.azure.cn`, `[Your Key]`          | См. [Azure](https://docs.azure.cn/en-us/ai-services/translator/text-translation-overview)                                                                                                                                  |
| **Tencent**          | `tencent`      | `TENCENTCLOUD_SECRET_ID`, `TENCENTCLOUD_SECRET_KEY`                   | `[Your ID]`, `[Your Key]`                                | См. [Tencent](https://www.tencentcloud.com/products/tmt?from_qcintl=122110104)                                                                                                                                             |
| **Dify**             | `dify`         | `DIFY_API_URL`, `DIFY_API_KEY`                                        | `[Ваш URL Dify]`, `[Ваш ключ]`                          | См. [Dify](https://github.com/langgenius/dify),Три переменные: lang_out, lang_in и text должны быть определены во входных данных рабочего процесса Dify.                                                                                  |
| **AnythingLLM**      | `anythingllm`  | `AnythingLLM_URL`, `AnythingLLM_APIKEY`                               | `[Your AnythingLLM URL]`, `[Your Key]`                   | См. [anything-llm](https://github.com/Mintplex-Labs/anything-llm)                                                                                                                                                          |
| **Argos Translate**  | `argos`        |                                                                       |                                                          | См. [argos-translate](https://github.com/argosopentech/argos-translate)                                                                                                                                                    |
| **Grok**             | `grok`         | `GORK_API_KEY`, `GORK_MODEL`                                          | `[Your GORK_API_KEY]`, `grok-2-1212`                     | См. [Grok](https://docs.x.ai/docs/overview)                                                                                                                                                                                |
| **Groq**             | `groq`         | `GROQ_API_KEY`, `GROQ_MODEL`                                          | `[Your GROQ_API_KEY]`, `llama-3-3-70b-versatile`         | См. [Groq](https://console.groq.com/docs/models)                                                                                                                                                                           |
| **DeepSeek**         | `deepseek`     | `DEEPSEEK_API_KEY`, `DEEPSEEK_MODEL`                                  | `[Your DEEPSEEK_API_KEY]`, `deepseek-chat`               | См. [DeepSeek](https://www.deepseek.com/)                                                                                                                                                                                  |
| **OpenAI-Liked**     | `openailiked`  | `OPENAILIKED_BASE_URL`, `OPENAILIKED_API_KEY`, `OPENAILIKED_MODEL`    | `url`, `[Your Key]`, `model name`                        | None                                                                                                                                                                                                                       |
| **Ali Qwen Translation** | `qwen-mt`  | `ALI_MODEL`, `ALI_API_KEY`, `ALI_DOMAINS`                             | `qwen-mt-turbo`, `[Your Key]`, `scientific paper`        | Традиционный китайский пока не поддерживается, текст будет переведен на упрощенный китайский. Подробнее см. [Qwen MT](https://bailian.console.aliyun.com/?spm=5176.28197581.0.0.72e329a4HRxe99#/model-market/detail/qwen-mt-turbo) |

Для больших языковых моделей, совместимых с API OpenAI, но не перечисленных в таблице выше, вы можете установить переменные среды, используя тот же метод, что и для OpenAI в таблице.

Используйте `-s service` или `-s service:model` для указания сервиса:

```bash
pdf2zh_next example.pdf -s openai:gpt-4o-mini
```

Или укажите модель с помощью переменных окружения:

```bash
set OPENAI_MODEL=gpt-4o-mini
pdf2zh_next example.pdf -s openai
```

Для пользователей PowerShell:

```shell
$env:OPENAI_MODEL = gpt-4o-mini
pdf2zh_next example.pdf -s openai
```

<div align="right"> 
<h6><small>Часть содержимого этой страницы была переведена GPT и может содержать ошибки.</small></h6>