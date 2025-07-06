[**Começar**](./comecar.md) > **Instalação** > **WebUI** _(atual)_

---

### Usar PDFMathTranslate via Webui

#### Como abrir a página WebUI:

Existem vários métodos para abrir a interface WebUI. Se você estiver usando **Windows**, consulte [este artigo](./INSTALLATION_winexe.md);

1. Python instalado (3.10 <= versão <= 3.13)

2. Instale nosso pacote:

3. Comece a usar no navegador:

    ```bash
    pdf2zh_next --gui
    ```

4. Se o seu navegador não foi iniciado automaticamente, acesse

    ```bash
    http://localhost:7860/
    ```

    Solte o arquivo PDF na janela e clique em `Translate`.

<!-- <img src="./images/gui.gif" width="500"/> -->
<img src='./../images/gui.gif' width="500"/>

### Variáveis de Ambiente

Você pode definir os idiomas de origem e destino usando variáveis de ambiente:

- `PDF2ZH_LANG_FROM`: Define o idioma de origem. O padrão é "English".
- `PDF2ZH_LANG_TO`: Define o idioma de destino. O padrão é "Simplified Chinese".

## Pré-visualização

<img src="./../images/before.png" width="500"/>
<img src="./../images/after.png" width="500"/>

## Manutenção

GUI mantida por [Rongxin](https://github.com/reycn)

<div align="right"> 
<h6><small>Parte do conteúdo desta página foi traduzida pelo GPT e pode conter erros.</small></h6>