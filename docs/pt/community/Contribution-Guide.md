# Contribuindo para o projeto

> [!CAUTION]
>
> Os mantenedores atuais do projeto estão pesquisando a internacionalização automatizada de documentação. Portanto, qualquer PR relacionado à internacionalização/tradução de documentação NÃO será aceito!
>
> Por favor, NÃO envie PRs relacionados à internacionalização/tradução de documentação!

Obrigado pelo seu interesse neste projeto! Antes de começar a contribuir, reserve um tempo para ler as seguintes diretrizes para garantir que sua contribuição possa ser aceita sem problemas.

## Tipos de Contribuições Não Aceitas

1. Documentação de internacionalização/tradução  
2. Contribuições relacionadas à infraestrutura principal, como API HTTP, etc.  
3. Problemas explicitamente marcados como "No help needed" (incluindo problemas nos repositórios [Byaidu/PDFMathTranslate](Byaidu/PDFMathTranslate) e [PDFMathTranslate/PDFMathTranslate-next](PDFMathTranslate/PDFMathTranslate-next)).  
4. Outras contribuições consideradas inadequadas pelos mantenedores.  
5. Contribuição com documentação, mas alterando a documentação em idiomas diferentes do inglês.  
6. PRs que exigem modificação de arquivos PDF.

Por favor, NÃO envie PRs relacionados aos tipos mencionados acima.

> [!NOTE]
>
> Se você deseja contribuir com a documentação, por favor **modifique apenas a versão em inglês da documentação**. As outras versões em outros idiomas são traduzidas pelos próprios contribuidores.

## Processo de Contribuição

1. Faça um fork deste repositório e clone-o localmente.
2. Crie uma nova branch: `git checkout -b feature/<feature-name>`.
3. Desenvolva e certifique-se de que seu código atenda aos requisitos.
4. Faça commit do seu código:
   ```bash
   git add .
   git commit -m "<semantic commit message>"
   ```
5. Envie para o seu repositório: `git push origin feature/<feature-name>`.
6. Crie um PR no GitHub, forneça uma descrição detalhada e solicite uma revisão de [@awwaawwa](https://github.com/awwaawwa).
7. Certifique-se de que todas as verificações automatizadas sejam aprovadas.

> [!TIP]
>
> Você não precisa esperar até que seu desenvolvimento esteja totalmente completo para criar um PR. Criar um PR antecipadamente nos permite revisar sua implementação e fornecer sugestões.
>
> Se você tiver alguma dúvida sobre o código-fonte ou assuntos relacionados, entre em contato com o mantenedor em aw@funstory.ai.
>
> Os arquivos de recursos para a versão 2.0 são compartilhados com [BabelDOC](https://github.com/funstory-ai/BabelDOC). O código para baixar os recursos relacionados está no BabelDOC. Se você deseja adicionar novos arquivos de recursos, entre em contato com o mantenedor do BabelDOC em aw@funstory.ai.

## Requisitos básicos

<h4 id="sop">1. Fluxo de trabalho</h4>

   - Por favor, faça um fork a partir do branch `main` e desenvolva no seu branch bifurcado.
   - Ao enviar um Pull Request (PR), forneça uma descrição detalhada das suas alterações.
   - Se o seu PR não passar nas verificações automatizadas (indicado por `checks failed` e um cruz vermelho), revise os `details` correspondentes e modifique sua submissão para garantir que o novo PR passe em todas as verificações.


<h4 id="dev&test">2. Desenvolvimento e Teste</h4>

   - Use o comando `pip install -e .` para desenvolvimento e teste.


<h4 id="format">3. Formatação de Código</h4>

   - Configure a ferramenta `pre-commit` e ative `black` e `flake8` para formatação de código.


<h4 id="requpdate">4. Atualizações de Dependências</h4>

   - Se você introduzir novas dependências, atualize a lista de dependências no arquivo `pyproject.toml` em tempo hábil.


<h4 id="docupdate">5. Atualizações da Documentação</h4>

   - Se você adicionar novas opções de linha de comando, atualize a lista de opções de linha de comando em todas as versões de idioma do arquivo `README.md` de acordo.


<h4 id="commitmsg">6. Mensagens de Commit</h4>

   - Use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), por exemplo: `feat(translator): add openai`.


<h4 id="codestyle">7. Estilo de Codificação</h4>

   - Certifique-se de que o código enviado adere aos padrões básicos de estilo de codificação.
   - Use snake_case ou camelCase para nomeação de variáveis.


<h4 id="doctypo">8. Formatação de Documentação</h4>

   - Para a formatação de `README.md`, siga as [Diretrizes de Redação em Chinês](https://github.com/sparanoid/chinese-copywriting-guidelines).
   - Certifique-se de que a documentação em inglês e chinês esteja sempre atualizada; as atualizações de documentação em outros idiomas são opcionais.

## Adicionando um mecanismo de tradução

1. Adicione uma nova classe de configuração de tradutor no arquivo `pdf2zh/config/translate_engine_model.py`.
2. Adicione uma instância da nova classe de configuração de tradutor ao alias de tipo `TRANSLATION_ENGINE_SETTING_TYPE` no mesmo arquivo.
3. Adicione a nova classe de implementação de tradutor na pasta `pdf2zh/translator/translator_impl`.

> [!NOTE]
>
> Este projeto não pretende suportar nenhum mecanismo de tradução com um RPS (solicitações por segundo) inferior a 4. Por favor, não envie suporte para esses mecanismos.

## Estrutura do Projeto

- **config folder**: Sistema de configuração.
- **translator folder**: Implementações relacionadas ao tradutor.
- **gui.py**: Fornece a interface GUI.
- **const.py**: Algumas constantes.
- **main.py**: Fornece a ferramenta de linha de comando.
- **high_level.py**: Interfaces de alto nível baseadas no BabelDOC.
- **http_api.py**: Fornece API HTTP (não iniciada).

## Entre em contato conosco

Se você tiver alguma dúvida, envie feedback via Issue ou entre em nosso Grupo no Telegram. Obrigado pela sua contribuição!

> [!TIP]
>
> [Immersive Translate](https://immersivetranslate.com) patrocina códigos de assinatura Pro mensais para contribuidores ativos deste projeto. Para mais detalhes, consulte: [Regras de Recompensa para Contribuidores do BabelDOC/PDFMathTranslate](https://funstory-ai.github.io/BabelDOC/CONTRIBUTOR_REWARD/)

<div align="right"> 
<h6><small>Parte do conteúdo desta página foi traduzida pelo GPT e pode conter erros.</small></h6>