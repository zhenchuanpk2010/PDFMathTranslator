Algumas perguntas são frequentemente feitas, por isso fornecemos uma lista para usuários que encontram problemas semelhantes.

## É necessária uma GPU?
- **Pergunta**:
Como o programa usa inteligência artificial para reconhecer e extrair documentos, é necessária uma GPU?

- **Resposta**:
**Não é necessária uma GPU.** Mas se você tiver uma GPU, o programa irá usá-la automaticamente para melhor desempenho.

## Download interrompido?
- **Pergunta**:
Encontrei o seguinte erro de interrupção ao baixar o modelo. O que devo fazer?

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **Resposta**:
A rede está sofrendo interferência, por favor use uma conexão de rede estável ou tente contornar a intervenção da rede.

## Como atualizar para a versão mais recente?
- **Pergunta**:
Quero usar alguns dos recursos da versão mais recente, como posso atualizá-la?

- **Resposta**:
`pip install -U pdf2zh`


## Os seguintes arquivos não existem: example.pdf
- **Problema**:
Ao executar o programa, os usuários terão as seguintes saídas: `Os seguintes arquivos não existem: example.pdf` se o documento não for encontrado.

- **Solução**:
  - Abra a linha de comando no diretório onde o arquivo está localizado, ou
  - Insira o caminho completo do arquivo diretamente após pdf2zh, ou
  - Use o modo interativo `pdf2zh -i` para arrastar e soltar arquivos diretamente


## Erro SSL e Outros Problemas de Rede

[!NOTE]
If you encounter SSL errors or other network issues when using **pdf2zh**, please try the following solutions:

1. **Check Your Internet Connection**: Ensure your device is connected to the internet and can access other websites normally.

2. **Update Your System's Root Certificates**:
   - On **Windows**, run `certmgr.msc` and update the certificates.
   - On **macOS**, use `Keychain Access` to update the certificates.
   - On **Linux**, run `sudo update-ca-certificates`.

3. **Disable SSL Verification (Not Recommended)**:
   - Add `--no-ssl-verify` to the command line when using **pdf2zh**.
   - Example: `pdf2zh --no-ssl-verify input.pdf`.

4. **Use a Proxy**:
   - If you are in a region with network restrictions, try using a proxy or VPN.

5. **Check the Server Status**:
   - Visit [PDFMathTranslate Status Page](https://status.pdf2zh.com) to see if there are any ongoing issues.

If the problem persists, please contact our [Community](#community) or check the [FAQ](#faq) for more help.
- **Problema**:
Ao baixar modelos do Hugging Face, usuários na China podem encontrar erros de rede. Por exemplo, nos [issues #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55), [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70).

- **Solução**:
  - [Bypass GFW](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Usar Espelho do Hugging Face](https://hf-mirror.com/).
  - [Usar versão Portátil](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [Usar Docker em vez disso](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [Atualizar Certificados](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), como sugerido em [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55).

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