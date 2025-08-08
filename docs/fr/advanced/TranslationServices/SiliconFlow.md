# SiliconFlow

## Service de traduction gratuit

[SiliconFlow](https://siliconflow.cn) fournit un service de traduction gratuit pour ce projet.

Actuellement, le service de traduction gratuit utilisera le modèle `THUDM/GLM-4-9B-0414`.

### Utilisation

#### Ligne de commande

```bash
pdf2zh_next --siliconflowfree example.pdf 
```

#### webui

1. Sélectionnez "SiliconFlowFree" dans la liste déroulante "Options de traduction" - "Service".
2. Cliquez sur le bouton Traduire en bas de la page pour démarrer la traduction.
3. Une fois la traduction terminée, vous pouvez trouver le fichier PDF traduit dans la section "Traduit" en bas de la page.


### Politique de confidentialité

Le contenu du fichier sera envoyé au serveur du mainteneur du projet [@awwaawwa](https://github.com/awwaawwa), puis transmis à SiliconFlow pour traduction.

Les mainteneurs de ce projet ne collecteront que les informations d'erreur renvoyées par SiliconFlow pour le débogage des services associés. Votre contenu de fichier ne sera pas collecté.

Politique de confidentialité de SiliconFlow : [简体中文](https://docs.siliconflow.cn/cn/legals/privacy-policy)/[English](https://docs.siliconflow.cn/en/legals/privacy-policy)



## Utiliser d'autres modèles de SiliconFlow

[SiliconFlow](https://siliconflow.cn) propose également d'autres modèles pour la traduction.

### Utilisation

1. Créez un compte sur [SiliconFlow](https://siliconflow.cn)

2. Générez une clé API sur [SiliconFlow API Key](https://cloud.siliconflow.cn/me/account/ak). Ensuite, cliquez sur la clé pour la copier.

#### Ligne de commande

```bash
pdf2zh_next --siliconflow --siliconflow-model "Pro/deepseek-ai/DeepSeek-V3" --siliconflow-api-key <your-api-key> example.pdf
```

#### webui

1. "Options de traduction" - Liste déroulante **"Service"** : Sélectionnez "SiliconFlow"
2. "Options de traduction" - **"URL de base pour l'API SiliconFlow"** : Gardez la valeur par défaut
3. "Options de traduction" - **"Modèle SiliconFlow à utiliser"** : Entrez "Pro/deepseek-ai/DeepSeek-V3" ou d'autres modèles
4. "Options de traduction" - **"Clé API pour le service SiliconFlow"** : Collez votre clé API
5. Cliquez sur le bouton Traduire en bas de la page pour démarrer la traduction
6. Une fois la traduction terminée, vous pouvez trouver le fichier PDF traduit dans la section "Traduits" en bas de la page.


## Remerciements

Merci à [SiliconFlow](https://siliconflow.cn) pour avoir fourni un service de traduction gratuit pour ce projet.

<div align="right"> 
<h6><small>Une partie du contenu de cette page a été traduite par GPT et peut contenir des erreurs.</small></h6>