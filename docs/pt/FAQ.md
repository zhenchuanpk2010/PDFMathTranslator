Algumas perguntas são frequentemente feitas, por isso fornecemos uma lista para usuários que encontram problemas semelhantes.

## É necessária uma GPU?
- **Pergunta**:
Como o programa usa inteligência artificial para reconhecer e extrair documentos, é necessária uma GPU?

- **Resposta**:
**Não é necessária uma GPU.** Mas se você tiver uma GPU, o programa usará automaticamente para obter um desempenho maior.

## Download interrompido?
- **Pergunta**:
Encontrei o seguinte erro de interrupção ao baixar o modelo. O que devo fazer?

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **Resposta**:
A rede está recebendo interferência, por favor use uma conexão de rede estável ou tente contornar a intervenção da rede.

## Como atualizar para a versão mais recente?
- **Pergunta**:
Quero usar alguns dos recursos da versão mais recente, como faço para atualizá-la?

- **Resposta**:
`pip install -U pdf2zh`


## Os seguintes arquivos não existem: example.pdf
- **Problema**:
Ao executar o programa, os usuários teriam as seguintes saídas: `The following files do not exist: example.pdf` se o documento não fosse encontrado.

- **Solução**:
  - Abra a linha de comando no diretório onde o arquivo está localizado, ou
  - Insira o caminho completo do arquivo diretamente após pdf2zh, ou
  - Use o modo interativo `pdf2zh -i` para arrastar e soltar arquivos diretamente


## Erro SSL e Outros Problemas de Rede

### 1. SSL Error

If you encounter an SSL error when using `pdf2zh`, it is likely due to an outdated SSL certificate or an issue with your network configuration. Here are some steps to resolve this:

1. **Update Your System**: Ensure your operating system and Python environment are up to date.
2. **Check the Certificate**: Verify the SSL certificate of the server you are trying to connect to.
3. **Use a VPN**: Sometimes, network restrictions can cause SSL errors. Try using a VPN to bypass these restrictions.

### 2. Other Network Issues

If you are experiencing other network-related issues, consider the following:

1. **Check Your Internet Connection**: Ensure you have a stable internet connection.
2. **Firewall Settings**: Check if your firewall is blocking `pdf2zh`.
3. **Proxy Configuration**: If you are behind a proxy, ensure it is correctly configured.

For more detailed troubleshooting, refer to the [Documentation of Translation Services](#documentation-of-translation-services).
- **Problema**:
Ao baixar modelos do Hugging Face, usuários na China podem enfrentar erros de rede. Por exemplo, nos [issues #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55), [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70).

- **Solução**:
  - [Bypass GFW](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Usar espelho do Hugging Face](https://hf-mirror.com/).
  - [Usar versão portátil](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [Usar Docker em vez disso](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [Atualizar certificados](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), conforme sugerido em [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55).

## O localhost não está acessível
Por favor, veja abaixo.

## Erro ao iniciar a GUI usando 0.0.0.0
- **Problema**:
O uso de software de proxy no modo global pode impedir que o Gradio seja iniciado corretamente. Por exemplo, no [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77).

- **Solução**:
Usar modo de regra

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>Parte do conteúdo desta página foi traduzida pelo GPT e pode conter erros.</small></h6>