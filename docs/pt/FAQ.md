Algumas perguntas são frequentemente feitas, então fornecemos uma lista para usuários que encontram problemas semelhantes.

## É necessária uma GPU?
- **Pergunta**:
Como o programa usa inteligência artificial para reconhecer e extrair documentos, é necessária uma GPU?


- **Resposta**:  
```
**Não é necessária uma GPU.** Mas se você tiver uma GPU, o programa usará automaticamente para maior desempenho.

## Download interrompida?
- **Pergunta**:
Encontrei o seguinte erro de interrupção ao baixar o modelo. O que devo fazer?

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)


- **Resposta**:  
```
A rede está recebendo interferência, por favor use uma conexão de rede estável ou tente contornar a intervenção da rede.

## Como atualizar para a versão mais recente?
- **Pergunta**:
Eu quero usar alguns dos recursos da versão mais recente, como atualizo para ela?


- **Resposta**:  
```
`pip install -U pdf2zh`


## Os seguintes arquivos não existem: example.pdf
- **Problema**:
Ao executar o programa, os usuários terão as seguintes saídas: `Os seguintes arquivos não existem: example.pdf` se o documento não for encontrado.

- **Solução**:
  - Abra a linha de comando no diretório onde o arquivo está localizado, ou
  - Insira o caminho completo do arquivo diretamente após pdf2zh, ou
  - Use o modo interativo `pdf2zh -i` para arrastar e soltar arquivos diretamente


## Erro SSL e Outros Problemas de Rede
- **Problema**:
Ao baixar modelos do hugging face, usuários na China podem encontrar erros de rede. Por exemplo, nos [problemas #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55), [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70).

- **Solução**:
  - [Bypass GFW](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Usar o Espelho do Hugging Face](https://hf-mirror.com/).
  - [Usar a versão Portátil](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [Usar Docker em vez disso](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [Atualizar Certificados](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), como sugerido em [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55).

## Localhost não está acessível
Por favor, veja abaixo.

## Erro ao iniciar a GUI usando 0.0.0.0
- **Problema**:
O uso de software de proxy no modo global pode impedir que o Gradio inicie corretamente. Por exemplo, no [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77).

- **Solução**:
Usar modo de regra

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>Parte do conteúdo desta página foi traduzida pelo GPT e pode conter erros.</small></h6>