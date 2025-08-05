Algumas perguntas são frequentemente feitas, por isso fornecemos uma lista para usuários que enfrentam problemas semelhantes.

## É necessária uma GPU?
- **Pergunta**:
O programa usa inteligência artificial para reconhecer e extrair documentos, é necessária uma GPU?

- **Resposta**:
**Não é necessária uma GPU.** Mas se você tiver uma GPU, o programa usará automaticamente para melhor desempenho.

## Download interrompido?
- **Pergunta**:
Encontrei o seguinte erro de interrupção ao baixar o modelo. O que devo fazer?

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **Resposta**:
A rede está recebendo interferência, por favor, use um link de rede estável ou tente contornar a intervenção da rede.

## Como atualizar para a versão mais recente?
- **Pergunta**:
Quero usar alguns dos recursos da versão mais recente, como atualizo?

- **Resposta**:
`pip install -U pdf2zh`


## Os seguintes arquivos não existem: example.pdf
- **Problema**:
Ao executar o programa, os usuários terão as seguintes saídas: `The following files do not exist: example.pdf` se o documento não for encontrado.

- **Solução**:
  - Abra a linha de comando no diretório onde o arquivo está localizado, ou
  - Insira o caminho completo do arquivo diretamente após pdf2zh, ou
  - Use o modo interativo `pdf2zh -i` para arrastar e soltar arquivos diretamente


## Erro SSL e Outros Problemas de Rede
- **Problema**:
Ao baixar modelos do Hugging Face, usuários na China podem enfrentar erros de rede. Por exemplo, nos [issues #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55), [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70).

- **Solução**:
  - [Contornar o GFW](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Usar o Espelho do Hugging Face](https://hf-mirror.com/).
  - [Usar a versão Portátil](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [Usar Docker em vez disso](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [Atualizar Certificados](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), conforme sugerido no [problema #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55).

If you cannot access the localhost address (e.g., `http://127.0.0.1:5000`), please check the following:

1. **Check if the service is running**  
   Run `pdf2zh --version` in the terminal to confirm that the service is installed and running. If not, please refer to the [Installation](#installation) guide.

2. **Check the port**  
   The default port is `5000`. If it's occupied, the service will automatically switch to another port. You can check the actual port in the terminal logs.

3. **Check the firewall**  
   Ensure that your firewall or security software is not blocking the port. You may need to add an exception for `pdf2zh`.

4. **Try another browser**  
   Some browsers or extensions may block localhost access. Try accessing it in incognito mode or another browser.

5. **Check the network configuration**  
   If you are using a proxy or VPN, disable them temporarily to see if the issue persists.

If the problem persists, please refer to the [FAQ](#faq) or seek help in the [Community](#community).

---

## Localhost não está acessível

Se você não consegue acessar o endereço localhost (por exemplo, `http://127.0.0.1:5000`), verifique o seguinte:

1. **Verifique se o serviço está em execução**  
   Execute `pdf2zh --version` no terminal para confirmar que o serviço está instalado e em execução. Caso não esteja, consulte o guia de [Instalação](#instalação).

2. **Verifique a porta**  
   A porta padrão é `5000`. Se estiver ocupada, o serviço mudará automaticamente para outra porta. Você pode verificar a porta real nos logs do terminal.

3. **Verifique o firewall**  
   Certifique-se de que seu firewall ou software de segurança não está bloqueando a porta. Talvez seja necessário adicionar uma exceção para `pdf2zh`.

4. **Tente outro navegador**  
   Alguns navegadores ou extensões podem bloquear o acesso ao localhost. Tente acessar no modo anônimo ou em outro navegador.

5. **Verifique a configuração de rede**  
   Se você estiver usando um proxy ou VPN, desative-os temporariamente para ver se o problema persiste.

Se o problema persistir, consulte as [Perguntas frequentes](#perguntas-frequentes) ou busque ajuda na [Comunidade](#comunidade).
Por favor, veja abaixo.

## Erro ao iniciar a GUI usando 0.0.0.0
- **Problema**:
O uso de software de proxy no modo global pode impedir que o Gradio seja iniciado corretamente. Por exemplo, no [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77).

- **Solução**:
Usar modo de regra

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>Parte do conteúdo desta página foi traduzida pelo GPT e pode conter erros.</small></h6>