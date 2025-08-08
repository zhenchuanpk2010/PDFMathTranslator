# SiliconFlow

## Serviço de Tradução Gratuito

[SiliconFlow](https://siliconflow.cn) fornece um serviço de tradução gratuito para este projeto.

Atualmente, o serviço de tradução gratuito utilizará o modelo `THUDM/GLM-4-9B-0414`.

### Uso

#### Linha de comando

```bash
pdf2zh_next --siliconflowfree example.pdf 
```

#### webui

1. Selecione "SiliconFlowFree" na lista suspensa "Translation Options" - "Service".
2. Clique no botão "Translate" na parte inferior da página para iniciar a tradução.
3. Após a conclusão da tradução, você pode encontrar o arquivo PDF traduzido na seção "Translated" na parte inferior da página.


### Política de Privacidade

O conteúdo do arquivo será enviado para o servidor do mantenedor do projeto [@awwaawwa](https://github.com/awwaawwa) e, em seguida, encaminhado para o SiliconFlow para tradução.

Os mantenedores deste projeto coletarão apenas informações de erro retornadas pelo SiliconFlow para depuração dos serviços relacionados. O conteúdo do seu arquivo não será coletado.

Política de Privacidade do SiliconFlow: [简体中文](https://docs.siliconflow.cn/cn/legals/privacy-policy)/[English](https://docs.siliconflow.cn/en/legals/privacy-policy)



## Usar outros modelos do SiliconFlow

[SiliconFlow](https://siliconflow.cn) também fornece outros modelos para tradução.

### Uso

1. Registre uma conta no [SiliconFlow](https://siliconflow.cn)

2. Crie uma chave de API no [SiliconFlow API Key](https://cloud.siliconflow.cn/me/account/ak). Em seguida, clique na chave para copiá-la.

#### Linha de comando

```bash
pdf2zh_next --siliconflow --siliconflow-model "Pro/deepseek-ai/DeepSeek-V3" --siliconflow-api-key <your-api-key> example.pdf
```

#### webui

1. "Opções de Tradução" - Lista suspensa **"Serviço"**: Selecione "SiliconFlow"  
2. "Opções de Tradução" - **"URL base para a API do SiliconFlow"**: Mantenha o padrão  
3. "Opções de Tradução" - **"Modelo do SiliconFlow a ser usado"**: Insira "Pro/deepseek-ai/DeepSeek-V3" ou outros modelos  
4. "Opções de Tradução" - **"Chave de API para o serviço SiliconFlow"**: Cole sua chave de API  
5. Clique no botão "Traduzir" na parte inferior da página para iniciar a tradução  
6. Após a conclusão da tradução, você pode encontrar o arquivo PDF traduzido na seção "Traduzido" na parte inferior da página.


## Agradecimentos

Obrigado ao [SiliconFlow](https://siliconflow.cn) por fornecer o serviço de tradução gratuito para este projeto.

<div align="right"> 
<h6><small>Parte do conteúdo desta página foi traduzida pelo GPT e pode conter erros.</small></h6>