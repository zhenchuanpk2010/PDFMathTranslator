Certaines questions sont fréquemment posées, nous avons donc fourni une liste pour les utilisateurs qui rencontrent des problèmes similaires.

## Un GPU est-il nécessaire ?
- **Question**:  
- **Question**:
Le programme utilise l'intelligence artificielle pour reconnaître et extraire des documents, un GPU est-il nécessaire ?

- **Réponse** :
**Un GPU n'est pas nécessaire.** Mais si vous avez un GPU, le programme l'utilisera automatiquement pour une meilleure performance.

## Téléchargement interrompu ?
- **Question**:  
- **Question**:
J'ai rencontré l'erreur d'interruption suivante lors du téléchargement du modèle. Que dois-je faire ?

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **Réponse** :
Le réseau subit des interférences, veuillez utiliser une connexion réseau stable ou essayer de contourner l'intervention du réseau.

## Comment mettre à jour vers la dernière version ?
- **Question**:  
- **Question**:
Je souhaite utiliser certaines fonctionnalités de la dernière version, comment puis-je la mettre à jour ?

- **Réponse** :
`pip install -U pdf2zh`


## Les fichiers suivants n'existent pas : example.pdf
- **Problème** :
Lors de l'exécution du programme, les utilisateurs auront les sorties suivantes : `The following files do not exist: example.pdf` si le document n'a pas été trouvé.

- **Solution** :
  - Ouvrez la ligne de commande dans le répertoire où se trouve le fichier, ou
  - Entrez le chemin complet du fichier directement après pdf2zh, ou
  - Utilisez le mode interactif `pdf2zh -i` pour glisser-déposer les fichiers directement


## Erreur SSL et autres problèmes réseau
- **Problème** :
Lors du téléchargement des modèles de hugging face, les utilisateurs en Chine peuvent rencontrer des erreurs réseau. Par exemple, dans [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55), [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70).

- **Solution** :
  - [Contourner le GFW](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Utiliser le miroir Hugging Face](https://hf-mirror.com/).
  - [Utiliser la version portable](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [Utiliser Docker à la place](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [Mettre à jour les certificats](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), comme suggéré dans [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55).

## Localhost n'est pas accessible
Veuillez voir ci-dessous.

## Erreur lors du lancement de l'interface graphique avec 0.0.0.0
- **Problème** :
L'utilisation d'un logiciel proxy en mode global peut empêcher Gradio de démarrer correctement. Par exemple, dans [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77).

- **Solution** :
Utiliser le mode règle

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>Une partie du contenu de cette page a été traduite par GPT et peut contenir des erreurs.</small></h6>