[**Options avancées**](./introduction.md) > **Documentation des services de traduction** _(current)_

---

### Visualiser les services de traduction disponibles via la Ligne de commande

Vous pouvez confirmer les services de traduction disponibles et leur utilisation en affichant le message d'aide dans la ligne de commande.

```bash
pdf2zh_next -h
```

À la fin du message d'aide, vous pouvez visualiser des informations détaillées sur les différents services de traduction.

---

> [!CAUTION]
> Le contenu suivant a été préparé pour la version 1.x de pdf2zh et n'a pas encore été mis à jour pour la version 2.x. Par conséquent, les informations peuvent être **obsolètes**.
>
> Ce message d'avertissement sera supprimé une fois que le contenu de l'article sera aligné avec la nouvelle version.

* [Google Translate](https://cloud.google.com/translate/docs)
* [DeepL](https://developers.deepl.com/docs/api-reference/translate)
* [DeepLX](https://github.com/OwO-Network/DeepLX)
* [OpenAI](https://platform.openai.com/docs/api-reference/introduction)
* [Ollama](https://github.com/ollama/ollama/blob/main/docs/api.md)
* [Azure](https://learn.microsoft.com/en-us/azure/ai-services/translator/)
* [Zhipu](https://bigmodel.cn/)
* [DeepSeek](https://api-docs.deepseek.com/)

#### Traduire avec différents services

Nous avons fourni un tableau détaillé sur les [variables d'environnement](https://chatgpt.com/share/6734a83d-9d48-800e-8a46-f57ca6e8bcb4) requises pour chaque service de traduction. Assurez-vous de les configurer avant d'utiliser le service correspondant.

| **Traducteur**       | **Service**    | **Variables d'environnement**                                         | **Valeurs par défaut**                                   | **Notes**                                                                                                                                                                                                                  |
| -------------------- | -------------- | --------------------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Google (Par défaut)** | `google`       | Aucune                                                                  | N/A                                                      | Aucune                                                                                                                                                                                                                       |
| **Bing**             | `bing`         | None                                                                  | N/A                                                      | None                                                                                                                                                                                                                       |
| **DeepL**            | `deepl`        | `DEEPL_AUTH_KEY`                                                      | `[Your Key]`                                             | Voir [DeepL](https://support.deepl.com/hc/en-us/articles/360020695820-API-Key-for-DeepL-s-API)                                                                                                                              |
| **DeepLX**           | `deeplx`       | `DEEPLX_ENDPOINT`                                                     | `https://api.deepl.com/translate`                        | Voir [DeepLX](https://github.com/OwO-Network/DeepLX)                                                                                                                                                                        |
| **Ollama**           | `ollama`       | `OLLAMA_HOST`, `OLLAMA_MODEL`                                         | `http://127.0.0.1:11434`, `gemma2`                       | Voir [Ollama](https://github.com/ollama/ollama)                                                                                                                                                                             |
| **Xinference**       | `xinference`   | `XINFERENCE_HOST`, `XINFERENCE_MODEL`                                 | `http://127.0.0.1:9997`, `gemma-2-it`                    | Voir [Xinference](https://github.com/xorbitsai/inference)                                                                                                                                                                   |
| **OpenAI**           | `openai`       | `OPENAI_BASE_URL`, `OPENAI_API_KEY`, `OPENAI_MODEL`                   | `https://api.openai.com/v1`, `[Votre clé]`, `gpt-4o-mini` | Voir [OpenAI](https://platform.openai.com/docs/overview)                                                                                                                                                                    |
| **AzureOpenAI**      | `azure-openai` | `AZURE_OPENAI_BASE_URL`, `AZURE_OPENAI_API_KEY`, `AZURE_OPENAI_MODEL` | `[Your Endpoint]`, `[Your Key]`, `gpt-4o-mini`           | Voir [Azure OpenAI](https://learn.microsoft.com/zh-cn/azure/ai-services/openai/chatgpt-quickstart?tabs=command-line%2Cjavascript-keyless%2Ctypescript-keyless%2Cpython&pivots=programming-language-python)                  |
| **Zhipu**            | `zhipu`        | `ZHIPU_API_KEY`, `ZHIPU_MODEL`                                        | `[Your Key]`, `glm-4-flash`                              | Voir [Zhipu](https://open.bigmodel.cn/dev/api/thirdparty-frame/openai-sdk)                                                                                                                                                  |
| **ModelScope**       | `ModelScope`   | `MODELSCOPE_API_KEY`, `MODELSCOPE_MODEL`                              | `[Your Key]`, `Qwen/Qwen2.5-Coder-32B-Instruct`          | Voir [ModelScope](https://www.modelscope.cn/docs/model-service/API-Inference/intro)                                                                                                                                         |
| **Silicon**          | `silicon`      | `SILICON_API_KEY`, `SILICON_MODEL`                                    | `[Your Key]`, `Qwen/Qwen2.5-7B-Instruct`                 | Voir [SiliconCloud](https://docs.siliconflow.cn/quickstart)                                                                                                                                                                 |
| **Gemini**           | `gemini`       | `GEMINI_API_KEY`, `GEMINI_MODEL`                                      | `[Your Key]`, `gemini-1.5-flash`                         | Voir [Gemini](https://ai.google.dev/gemini-api/docs/openai)                                                                                                                                                                 |
| **Azure**            | `azure`        | `AZURE_ENDPOINT`, `AZURE_API_KEY`                                     | `https://api.translator.azure.cn`, `[Your Key]`          | Voir [Azure](https://docs.azure.cn/en-us/ai-services/translator/text-translation-overview)                                                                                                                                  |
| **Tencent**          | `tencent`      | `TENCENTCLOUD_SECRET_ID`, `TENCENTCLOUD_SECRET_KEY`                   | `[Your ID]`, `[Your Key]`                                | Voir [Tencent](https://www.tencentcloud.com/products/tmt?from_qcintl=122110104)                                                                                                                                             |
| **Dify**             | `dify`         | `DIFY_API_URL`, `DIFY_API_KEY`                                        | `[Your DIFY URL]`, `[Your Key]`                          | Voir [Dify](https://github.com/langgenius/dify),Trois variables, lang_out, lang_in et text, doivent être définies dans l'entrée du workflow de Dify.                                                                                  |
| **AnythingLLM**      | `anythingllm`  | `AnythingLLM_URL`, `AnythingLLM_APIKEY`                               | `[Your AnythingLLM URL]`, `[Your Key]`                   | Voir [anything-llm](https://github.com/Mintplex-Labs/anything-llm)                                                                                                                                                          |
| **Argos Translate**  | `argos`        |                                                                       |                                                          | Voir [argos-translate](https://github.com/argosopentech/argos-translate)                                                                                                                                                    |
| **Grok**             | `grok`         | `GORK_API_KEY`, `GORK_MODEL`                                          | `[Your GORK_API_KEY]`, `grok-2-1212`                     | Voir [Grok](https://docs.x.ai/docs/overview)                                                                                                                                                                                |
| **Groq**             | `groq`         | `GROQ_API_KEY`, `GROQ_MODEL`                                          | `[Your GROQ_API_KEY]`, `llama-3-3-70b-versatile`         | Voir [Groq](https://console.groq.com/docs/models)                                                                                                                                                                           |
| **DeepSeek**         | `deepseek`     | `DEEPSEEK_API_KEY`, `DEEPSEEK_MODEL`                                  | `[Your DEEPSEEK_API_KEY]`, `deepseek-chat`               | Voir [DeepSeek](https://www.deepseek.com/)                                                                                                                                                                                  |
| **OpenAI-Liked**     | `openailiked`  | `OPENAILIKED_BASE_URL`, `OPENAILIKED_API_KEY`, `OPENAILIKED_MODEL`    | `url`, `[Your Key]`, `model name`                        | None                                                                                                                                                                                                                       |
| **Ali Qwen Translation** | `qwen-mt`  | `ALI_MODEL`, `ALI_API_KEY`, `ALI_DOMAINS`                             | `qwen-mt-turbo`, `[Your Key]`, `scientific paper`        | Le chinois traditionnel n'est pas encore supporté, il sera traduit en chinois simplifié. Plus d'informations sur [Qwen MT](https://bailian.console.aliyun.com/?spm=5176.28197581.0.0.72e329a4HRxe99#/model-market/detail/qwen-mt-turbo) |

Pour les grands modèles de langage compatibles avec l'API OpenAI mais non listés dans le tableau ci-dessus, vous pouvez définir des variables d'environnement en utilisant la même méthode décrite pour OpenAI dans le tableau.

Utilisez `-s service` ou `-s service:model` pour spécifier le service :

```bash
pdf2zh_next example.pdf -s openai:gpt-4o-mini
```

Ou spécifiez le modèle avec des variables d'environnement :

```bash
set OPENAI_MODEL=gpt-4o-mini
pdf2zh_next example.pdf -s openai
```

Pour les utilisateurs de PowerShell :

```shell
$env:OPENAI_MODEL = gpt-4o-mini
pdf2zh_next example.pdf -s openai
```

<div align="right"> 
<h6><small>Une partie du contenu de cette page a été traduite par GPT et peut contenir des erreurs.</small></h6>