[**Opções avançadas**](./introduction.md) > **Documentação dos serviços de tradução** _(atual)_

---

### Visualizando os Serviços de Tradução Disponíveis via Linha de comando

Você pode confirmar os serviços de tradução disponíveis e seu uso imprimindo a mensagem de ajuda na linha de comando.

```bash
pdf2zh_next -h
```

No final da mensagem de ajuda, você pode visualizar informações detalhadas sobre os diferentes serviços de tradução.

---

> [!CAUTION]
> O conteúdo a seguir foi preparado para a versão 1.x do pdf2zh e ainda não foi atualizado para a versão 2.x. Portanto, as informações podem estar **desatualizadas**.
>
> Esta mensagem de aviso será removida assim que o conteúdo do artigo estiver alinhado com a nova versão.

* [Google Translate](https://cloud.google.com/translate/docs)
* [DeepL](https://developers.deepl.com/docs/api-reference/translate)
* [DeepLX](https://github.com/OwO-Network/DeepLX)
* [OpenAI](https://platform.openai.com/docs/api-reference/introduction)
* [Ollama](https://github.com/ollama/ollama/blob/main/docs/api.md)
* [Azure](https://learn.microsoft.com/en-us/azure/ai-services/translator/)
* [Zhipu](https://bigmodel.cn/)
* [DeepSeek](https://api-docs.deepseek.com/)

#### Traduzir com diferentes serviços

Fornecemos uma tabela detalhada sobre as [variáveis de ambiente](https://chatgpt.com/share/6734a83d-9d48-800e-8a46-f57ca6e8bcb4) necessárias para cada serviço de tradução. Certifique-se de configurá-las antes de usar o respectivo serviço.

| **Tradutor**         | **Serviço**    | **Variáveis de Ambiente**                                             | **Valores Padrão**                                       | **Observações**                                                                                                                                                                                                                  |
| -------------------- | -------------- | --------------------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Google (Padrão)**  | `google`       | None                                                                  | N/A                                                      | None                                                                                                                                                                                                                       |
| **Bing**             | `bing`         | None                                                                  | N/A                                                      | None                                                                                                                                                                                                                       |
| **DeepL**            | `deepl`        | `DEEPL_AUTH_KEY`                                                      | `[Sua Chave]`                                             | Veja [DeepL](https://support.deepl.com/hc/en-us/articles/360020695820-API-Key-for-DeepL-s-API)                                                                                                                              |
| **DeepLX**           | `deeplx`       | `DEEPLX_ENDPOINT`                                                     | `https://api.deepl.com/translate`                        | Veja [DeepLX](https://github.com/OwO-Network/DeepLX)                                                                                                                                                                        |
| **Ollama**           | `ollama`       | `OLLAMA_HOST`, `OLLAMA_MODEL`                                         | `http://127.0.0.1:11434`, `gemma2`                       | Veja [Ollama](https://github.com/ollama/ollama)                                                                                                                                                                             |
| **Xinference**       | `xinference`   | `XINFERENCE_HOST`, `XINFERENCE_MODEL`                                 | `http://127.0.0.1:9997`, `gemma-2-it`                    | Veja [Xinference](https://github.com/xorbitsai/inference)                                                                                                                                                                   |
| **OpenAI**           | `openai`       | `OPENAI_BASE_URL`, `OPENAI_API_KEY`, `OPENAI_MODEL`                   | `https://api.openai.com/v1`, `[Sua Chave]`, `gpt-4o-mini` | Veja [OpenAI](https://platform.openai.com/docs/overview)                                                                                                                                                                    |
| **AzureOpenAI**      | `azure-openai` | `AZURE_OPENAI_BASE_URL`, `AZURE_OPENAI_API_KEY`, `AZURE_OPENAI_MODEL` | `[Seu Endpoint]`, `[Sua Chave]`, `gpt-4o-mini`           | Veja [Azure OpenAI](https://learn.microsoft.com/zh-cn/azure/ai-services/openai/chatgpt-quickstart?tabs=command-line%2Cjavascript-keyless%2Ctypescript-keyless%2Cpython&pivots=programming-language-python)                  |
| **Zhipu**            | `zhipu`        | `ZHIPU_API_KEY`, `ZHIPU_MODEL`                                        | `[Your Key]`, `glm-4-flash`                              | Veja [Zhipu](https://open.bigmodel.cn/dev/api/thirdparty-frame/openai-sdk)                                                                                                                                                  |
| **ModelScope**       | `ModelScope`   | `MODELSCOPE_API_KEY`, `MODELSCOPE_MODEL`                              | `[Your Key]`, `Qwen/Qwen2.5-Coder-32B-Instruct`          | Veja [ModelScope](https://www.modelscope.cn/docs/model-service/API-Inference/intro)                                                                                                                                         |
| **Silicon**          | `silicon`      | `SILICON_API_KEY`, `SILICON_MODEL`                                    | `[Your Key]`, `Qwen/Qwen2.5-7B-Instruct`                 | Veja [SiliconCloud](https://docs.siliconflow.cn/quickstart)                                                                                                                                                                 |
| **Gemini**           | `gemini`       | `GEMINI_API_KEY`, `GEMINI_MODEL`                                      | `[Sua Chave]`, `gemini-1.5-flash`                         | Veja [Gemini](https://ai.google.dev/gemini-api/docs/openai)                                                                                                                                                                 |
| **Azure**            | `azure`        | `AZURE_ENDPOINT`, `AZURE_API_KEY`                                     | `https://api.translator.azure.cn`, `[Your Key]`          | Veja [Azure](https://docs.azure.cn/en-us/ai-services/translator/text-translation-overview)                                                                                                                                  |
| **Tencent**          | `tencent`      | `TENCENTCLOUD_SECRET_ID`, `TENCENTCLOUD_SECRET_KEY`                   | `[Seu ID]`, `[Sua Chave]`                                | Veja [Tencent](https://www.tencentcloud.com/products/tmt?from_qcintl=122110104)                                                                                                                                             |
| **Dify**             | `dify`         | `DIFY_API_URL`, `DIFY_API_KEY`                                        | `[Seu URL DIFY]`, `[Sua Chave]`                          | Veja [Dify](https://github.com/langgenius/dify),Três variáveis, lang_out, lang_in e text, precisam ser definidas na entrada do workflow do Dify.                                                                                  |
| **AnythingLLM**      | `anythingllm`  | `AnythingLLM_URL`, `AnythingLLM_APIKEY`                               | `[Your AnythingLLM URL]`, `[Your Key]`                   | Veja [anything-llm](https://github.com/Mintplex-Labs/anything-llm)                                                                                                                                                          |
| **Argos Translate**  | `argos`        |                                                                       |                                                          | Veja [argos-translate](https://github.com/argosopentech/argos-translate)                                                                                                                                                    |
| **Grok**             | `grok`         | `GORK_API_KEY`, `GORK_MODEL`                                          | `[Your GORK_API_KEY]`, `grok-2-1212`                     | Veja [Grok](https://docs.x.ai/docs/overview)                                                                                                                                                                                |
| **Groq**             | `groq`         | `GROQ_API_KEY`, `GROQ_MODEL`                                          | `[Your GROQ_API_KEY]`, `llama-3-3-70b-versatile`         | Veja [Groq](https://console.groq.com/docs/models)                                                                                                                                                                           |
| **DeepSeek**         | `deepseek`     | `DEEPSEEK_API_KEY`, `DEEPSEEK_MODEL`                                  | `[Seu DEEPSEEK_API_KEY]`, `deepseek-chat`               | Veja [DeepSeek](https://www.deepseek.com/)                                                                                                                                                                                  |
| **OpenAI-Liked**     | `openailiked`  | `OPENAILIKED_BASE_URL`, `OPENAILIKED_API_KEY`, `OPENAILIKED_MODEL`    | `url`, `[Your Key]`, `model name`                        | None                                                                                                                                                                                                                       |
| **Ali Qwen Translation** | `qwen-mt`  | `ALI_MODEL`, `ALI_API_KEY`, `ALI_DOMAINS`                             | `qwen-mt-turbo`, `[Your Key]`, `scientific paper`        | O Chinês Tradicional ainda não é suportado, será traduzido para Chinês Simplificado. Mais informações em [Qwen MT](https://bailian.console.aliyun.com/?spm=5176.28197581.0.0.72e329a4HRxe99#/model-market/detail/qwen-mt-turbo) |

Para modelos de linguagem grandes que são compatíveis com a API OpenAI, mas não estão listados na tabela acima, você pode definir variáveis de ambiente usando o mesmo método descrito para OpenAI na tabela.

Use `-s service` ou `-s service:model` para especificar o serviço:

```bash
pdf2zh_next example.pdf -s openai:gpt-4o-mini
```

Ou especifique o modelo com variáveis de ambiente:

```bash
set OPENAI_MODEL=gpt-4o-mini
pdf2zh_next example.pdf -s openai
```

Para usuários do PowerShell:

```shell
$env:OPENAI_MODEL = gpt-4o-mini
pdf2zh_next example.pdf -s openai
```

<div align="right"> 
<h6><small>Parte do conteúdo desta página foi traduzida pelo GPT e pode conter erros.</small></h6>