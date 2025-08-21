[**Começar**](./getting-started.md) > **Instalação** > **Windows EXE** _(atual)_

---

### Instalar PDFMathTranslate via arquivo .exe

***Passo 1*** | Baixe `pdf2zh-<version>-with-assets-win64.zip` da [página de lançamentos](https://github.com/PDFMathTranslate/PDFMathTranslate-next/releases).

> [!TIP]
> **Qual é a diferença entre `pdf2zh-<version>-with-assets-win64.zip` e `pdf2zh-<version>-win64.zip`?**
>
> - Se você está baixando e usando o PDFMathTranslate pela primeira vez, é recomendado baixar `pdf2zh-<version>-with-assets-win64.zip`.
> - O `pdf2zh-<version>-with-assets-win64.zip` inclui arquivos de recursos (como fontes e modelos) em comparação com `pdf2zh-<version>-win64.zip`.
> - A versão sem recursos também irá baixar os recursos dinamicamente durante a execução, mas o download pode falhar devido a problemas de rede.

***Passo 2*** | Descompacte `pdf2zh-<version>-with-assets-win64.zip` e navegue até a pasta `pdf2zh`. Leva um tempo para descompactar, por favor, seja paciente.

***Passo 3*** | Navegue até a pasta `pdf2zh`, depois clique duas vezes em `pdf2zh.exe`.

> [!TIP]
> **Não consegue executar o arquivo .exe**
>
> Se você tiver algum problema ao executar o pdf2zh.exe, por favor instale `https://aka.ms/vs/17/release/vc_redist.x64.exe` e tente novamente.

***Passo 4*** | Um terminal será exibido após clicar duas vezes no arquivo .exe. Após cerca de meio minuto a um minuto, uma página da web será aberta no seu navegador padrão. Se isso não acontecer, você pode tentar acessar manualmente `http://localhost:7860/`.

> [!NOTE]
>
> Se você encontrar qualquer problema durante o uso do WebUI, consulte [esta página](./USAGE_webui.md).

***Passo 5*** | Aproveite!

> [!TIP]
> **Você pode usar o arquivo .exe via linha de comando**
>
> Use o arquivo .exe através da linha de comando da seguinte forma:
>
> - Inicie seu terminal e navegue até a pasta que contém o arquivo .exe:
>
> ```bash
> cd /path/pdf2zh_next/build
> ```
>
> - Chame o arquivo .exe:
>
> ```bash
> ./pdf2zh_next.exe "document.pdf"
> ```
>
> Você pode usar outros parâmetros de linha de comando normalmente:
>
> ```bash
> ./pdf2zh_next.exe "document.pdf" --lang-in en --lang-out ja
> ```
>
> Se precisar de mais informações sobre o uso da linha de comando, consulte este artigo.

<div align="right"> 
<h6><small>Parte do conteúdo desta página foi traduzida pelo GPT e pode conter erros.</small></h6>