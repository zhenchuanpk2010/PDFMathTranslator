[**高度な設定**](./introduction.md) > **翻訳サービスドキュメント** _(current)_

---

### コマンドラインで利用可能な翻訳サービスを表示する

コマンドラインでヘルプメッセージを表示することで、利用可能な翻訳サービスとその使い方を確認できます。

```bash
pdf2zh_next -h
```

ヘルプメッセージの最後で、さまざまな翻訳サービスの詳細情報を確認できます。

---

> [!CAUTION]
> 以下の内容は pdf2zh のバージョン 1.x 向けに準備されたもので、バージョン 2.x 向けにはまだ更新されていません。そのため、情報が**古くなっている**可能性があります。
>
> この警告メッセージは、記事の内容が新しいバージョンに合わせて更新された時点で削除されます。

* [Google Translate](https://cloud.google.com/translate/docs)
* [DeepL](https://developers.deepl.com/docs/api-reference/translate)
* [DeepLX](https://github.com/OwO-Network/DeepLX)
* [OpenAI](https://platform.openai.com/docs/api-reference/introduction)
* [Ollama](https://github.com/ollama/ollama/blob/main/docs/api.md)
* [Azure](https://learn.microsoft.com/en-us/azure/ai-services/translator/)
* [Zhipu](https://bigmodel.cn/)
* [DeepSeek](https://api-docs.deepseek.com/)

#### 異なるサービスで翻訳する

各翻訳サービスに必要な[環境変数](https://chatgpt.com/share/6734a83d-9d48-800e-8a46-f57ca6e8bcb4)について詳細な表を提供しています。それぞれのサービスを使用する前に設定してください。

| **Translator**       | **Service**    | **Environment Variables**                                             | **Default Values**                                       | **Notes**                                                                                                                                                                                                                  |
| -------------------- | -------------- | --------------------------------------------------------------------- | -------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Google (デフォルト)** | `google`       | None                                                                  | N/A                                                      | None                                                                                                                                                                                                                       |
| **Bing**             | `bing`         | None                                                                  | N/A                                                      | None                                                                                                                                                                                                                       |
| **DeepL**            | `deepl`        | `DEEPL_AUTH_KEY`                                                      | `[Your Key]`                                             | [DeepL](https://support.deepl.com/hc/en-us/articles/360020695820-API-Key-for-DeepL-s-API)を参照                                                                                                                              |
| **DeepLX**           | `deeplx`       | `DEEPLX_ENDPOINT`                                                     | `https://api.deepl.com/translate`                        | [DeepLX](https://github.com/OwO-Network/DeepLX) を参照                                                                                                                                                                        |
| **Ollama**           | `ollama`       | `OLLAMA_HOST`, `OLLAMA_MODEL`                                         | `http://127.0.0.1:11434`, `gemma2`                       | [Ollama](https://github.com/ollama/ollama) を参照                                                                                                                                                                             |
| **Xinference**       | `xinference`   | `XINFERENCE_HOST`, `XINFERENCE_MODEL`                                 | `http://127.0.0.1:9997`, `gemma-2-it`                    | [Xinference](https://github.com/xorbitsai/inference) を参照                                                                                                                                                                   |
| **OpenAI**           | `openai`       | `OPENAI_BASE_URL`, `OPENAI_API_KEY`, `OPENAI_MODEL`                   | `https://api.openai.com/v1`, `[Your Key]`, `gpt-4o-mini` | [OpenAI](https://platform.openai.com/docs/overview)を参照                                                                                                                                                                    |
| **AzureOpenAI**      | `azure-openai` | `AZURE_OPENAI_BASE_URL`, `AZURE_OPENAI_API_KEY`, `AZURE_OPENAI_MODEL` | `[Your Endpoint]`, `[Your Key]`, `gpt-4o-mini`           | [Azure OpenAI](https://learn.microsoft.com/zh-cn/azure/ai-services/openai/chatgpt-quickstart?tabs=command-line%2Cjavascript-keyless%2Ctypescript-keyless%2Cpython&pivots=programming-language-python) を参照                  |
| **Zhipu**            | `zhipu`        | `ZHIPU_API_KEY`, `ZHIPU_MODEL`                                        | `[Your Key]`, `glm-4-flash`                              | [Zhipu](https://open.bigmodel.cn/dev/api/thirdparty-frame/openai-sdk)を参照                                                                                                                                                  |
| **ModelScope**       | `ModelScope`   | `MODELSCOPE_API_KEY`, `MODELSCOPE_MODEL`                              | `[Your Key]`, `Qwen/Qwen2.5-Coder-32B-Instruct`          | [ModelScope](https://www.modelscope.cn/docs/model-service/API-Inference/intro)を参照                                                                                                                                         |
| **Silicon**          | `silicon`      | `SILICON_API_KEY`, `SILICON_MODEL`                                    | `[Your Key]`, `Qwen/Qwen2.5-7B-Instruct`                 | [SiliconCloud](https://docs.siliconflow.cn/quickstart)を参照                                                                                                                                                                 |
| **Gemini**           | `gemini`       | `GEMINI_API_KEY`, `GEMINI_MODEL`                                      | `[Your Key]`, `gemini-1.5-flash`                         | [Gemini](https://ai.google.dev/gemini-api/docs/openai)を参照                                                                                                                                                                 |
| **Azure**            | `azure`        | `AZURE_ENDPOINT`, `AZURE_API_KEY`                                     | `https://api.translator.azure.cn`, `[Your Key]`          | [Azure](https://docs.azure.cn/en-us/ai-services/translator/text-translation-overview) を参照                                                                                                                                  |
| **Tencent**          | `tencent`      | `TENCENTCLOUD_SECRET_ID`, `TENCENTCLOUD_SECRET_KEY`                   | `[Your ID]`, `[Your Key]`                                | [Tencent](https://www.tencentcloud.com/products/tmt?from_qcintl=122110104)を参照                                                                                                                                             |
| **Dify**             | `dify`         | `DIFY_API_URL`, `DIFY_API_KEY`                                        | `[Your DIFY URL]`, `[Your Key]`                          | [Dify](https://github.com/langgenius/dify)を参照。Dify のワークフロー入力では、lang_out、lang_in、text の 3 つの変数を定義する必要があります。                                                                                  |
| **AnythingLLM**      | `anythingllm`  | `AnythingLLM_URL`, `AnythingLLM_APIKEY`                               | `[Your AnythingLLM URL]`, `[Your Key]`                   | 詳細は [anything-llm](https://github.com/Mintplex-Labs/anything-llm) を参照                                                                                                                                                          |
| **Argos Translate**  | `argos`        |                                                                       |                                                          | [argos-translate](https://github.com/argosopentech/argos-translate) を参照                                                                                                                                                    |
| **Grok**             | `grok`         | `GORK_API_KEY`, `GORK_MODEL`                                          | `[Your GORK_API_KEY]`, `grok-2-1212`                     | [Grok](https://docs.x.ai/docs/overview) を参照                                                                                                                                                                                |
| **Groq**             | `groq`         | `GROQ_API_KEY`, `GROQ_MODEL`                                          | `[Your GROQ_API_KEY]`, `llama-3-3-70b-versatile`         | [Groq](https://console.groq.com/docs/models)を参照                                                                                                                                                                           |
| **DeepSeek**         | `deepseek`     | `DEEPSEEK_API_KEY`, `DEEPSEEK_MODEL`                                  | `[Your DEEPSEEK_API_KEY]`, `deepseek-chat`               | [DeepSeek](https://www.deepseek.com/)を参照                                                                                                                                                                                  |
| **OpenAI-Liked**     | `openailiked`  | `OPENAILIKED_BASE_URL`, `OPENAILIKED_API_KEY`, `OPENAILIKED_MODEL`    | `url`, `[Your Key]`, `model name`                        | None                                                                                                                                                                                                                       |
| **Ali Qwen Translation** | `qwen-mt`  | `ALI_MODEL`, `ALI_API_KEY`, `ALI_DOMAINS`                             | `qwen-mt-turbo`, `[Your Key]`, `scientific paper`        | 繁体中国語はまだサポートされていません、簡体中国語に翻訳されます。詳細は[Qwen MT](https://bailian.console.aliyun.com/?spm=5176.28197581.0.0.72e329a4HRxe99#/model-market/detail/qwen-mt-turbo)をご覧ください |

上記の表に記載されていないが OpenAI API と互換性のある大規模言語モデルの場合、表で OpenAI に対して説明されているのと同じ方法で環境変数を設定できます。

サービスを指定するには `-s service` または `-s service:model` を使用します：

```bash
pdf2zh_next example.pdf -s openai:gpt-4o-mini
```

または環境変数でモデルを指定します：

```bash
set OPENAI_MODEL=gpt-4o-mini
pdf2zh_next example.pdf -s openai
```

PowerShell ユーザーの場合：

```shell
$env:OPENAI_MODEL = gpt-4o-mini
pdf2zh_next example.pdf -s openai
```

<div align="right"> 
<h6><small>このページの一部のコンテンツは GPT によって翻訳されており、エラーが含まれている可能性があります。</small></h6>