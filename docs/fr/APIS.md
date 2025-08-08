> [!CAUTION]
>
> Ce document est obsolète, veuillez ne pas vous y référer.

<h2 id="toc">Table des matières</h2>
Le projet actuel prend en charge deux types d'APIs, toutes les méthodes nécessitent Redis ;

- [Appels fonctionnels en Python](#api-python)
- [Protocoles HTTP](#api-http)

---

<h2 id="api-python">Python</h2>

Comme `pdf2zh` est un module installé en Python, nous exposons deux méthodes pour que d'autres programmes puissent les appeler dans n'importe quel script Python.

Par exemple, si vous souhaitez traduire un document de l'anglais vers le chinois en utilisant Google Translate, vous pouvez utiliser le code suivant :

```python
from pdf2zh_next import translate, translate_stream

params = {
    'lang_in': 'en',
    'lang_out': 'zh',
    'service': 'google',
    'thread': 4,
}
```
Traduire avec des fichiers :
```python
(file_mono, file_dual) = translate(files=['example.pdf'], **params)[0]
```
Traduction avec flux :
```python
with open('example.pdf', 'rb') as f:
    (stream_mono, stream_dual) = translate_stream(stream=f.read(), **params)
```

[⬆️ Retour en haut](#toc)

---

<h2 id="api-http">HTTP</h2>

De manière plus flexible, vous pouvez communiquer avec le programme en utilisant les protocoles HTTP, si :

1. Installer et exécuter le backend

   ```bash
   pip install pdf2zh_next[backend]
   pdf2zh_next --flask
   pdf2zh_next --celery worker
   ```

2. Utiliser les protocoles HTTP comme suit :

   - Soumettre une tâche de traduction

     ```bash
     curl http://localhost:11008/v1/translate -F "file=@example.pdf" -F "data={\"lang_in\":\"en\",\"lang_out\":\"zh\",\"service\":\"google\",\"thread\":4}"
     {"id":"d9894125-2f4e-45ea-9d93-1a9068d2045a"}
     ```

   - Vérifier la progression

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"info":{"n":13,"total":506},"state":"PROGRESS"}
     ```

   - Vérifier la progression _(si terminé)_

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a
     {"state":"SUCCESS"}
     ```

   - Sauvegarder le fichier monolingue

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/mono --output example-mono.pdf
     ```

   - Sauvegarder le fichier bilingue

     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a/dual --output example-dual.pdf
     ```

   - Interrompre si en cours et supprimer la tâche
     ```bash
     curl http://localhost:11008/v1/translate/d9894125-2f4e-45ea-9d93-1a9068d2045a -X DELETE
     ```

[⬆️ Retour en haut](#toc)

---

<div align="right"> 
<h6><small>Une partie du contenu de cette page a été traduite par GPT et peut contenir des erreurs.</small></h6>