> [!CAUTION]
>
> Este documento está desatualizado, por favor, não o consulte.

<h2 id="toc">Índice</h2>
O presente projeto suporta dois tipos de APIs, todos os métodos precisam do Redis;

- [Chamadas funcionais em Python](#api-python)
- [Protocolos HTTP](#api-http)

---

<h2 id="api-python">Python</h2>

Como `pdf2zh` é um módulo instalado em Python, expomos dois métodos para que outros programas possam chamar em qualquer script Python.

Por exemplo, se você deseja traduzir um documento do inglês para o chinês usando o Google Tradutor, você pode usar o seguinte código:

```python
from pdf2zh_next import translate, translate_stream

params = {
    'lang_in': 'en',
    'lang_out': 'zh',
    'service': 'google',
    'thread': 4,
}
```
Traduzir com arquivos:
```python
(file_mono, file_dual) = translate(files=['example.pdf'], **params)[0]
```
Traduzir com fluxo:
```python
with open('example.pdf', 'rb') as f:
    (stream_mono, stream_dual) = translate_stream(stream=f.read(), **params)
```

[⬆️ Voltar ao topo](#toc)

---

<h2 id="api-http">HTTP</h2>

De uma forma mais flexível, você pode se comunicar com o programa usando protocolos HTTP, se:

1. Instalar e executar o backend

   ```bash
   pip install pdf2zh_next[backend]
   pdf2zh_next --flask
   pdf2zh_next --celery worker
   ```

2. Usar os protocolos HTTP conforme a seguir:

   - Enviar tarefa de tradução

     ```bash
     curl http://localhost:11008/v1/translate -F "file=@example.pdf" -F "data={\"lang_in\":\"en\",\"lang_out\":\"zh\",\"service\":\"google\",\"thread\":4}"
     {"id":"d9894125-2f4e-45ea-9d93-1a9068d2045a"}
     ```

   - Verificar progresso

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"info":{"n":13,"total":506},"state":"PROGRESS"}
     ```

   - Verificar progresso _(se concluído)_

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"state":"SUCCESS"}
     ```

   - Salvar arquivo monolíngue

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/mono --output example-mono.pdf
     ```

   - Salvar arquivo bilíngue

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/dual --output example-dual.pdf
     ```

   - Interromper se estiver em execução e excluir a tarefa
     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a -X DELETE
     ```

[⬆️ Voltar ao topo](#toc)

---

<div align="right"> 
<h6><small>Parte do conteúdo desta página foi traduzida pelo GPT e pode conter erros.</small></h6>