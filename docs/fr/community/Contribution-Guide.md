# Contribuer au projet

> [!CAUTION]
>
> Les mainteneurs actuels du projet recherchent une internationalisation automatisée de la documentation. Par conséquent, toute PR liée à l'internationalisation/traduction de la documentation ne sera PAS acceptée !
>
> Veuillez ne PAS soumettre de PR liées à l'internationalisation/traduction de la documentation !

Merci pour votre intérêt pour ce projet ! Avant de commencer à contribuer, veuillez prendre le temps de lire les directives suivantes pour vous assurer que votre contribution puisse être acceptée sans problème.

## Types de contributions non acceptées

1. Documentation internationalisation/traduction  
2. Contributions liées à l'infrastructure principale, telles que l'API HTTP, etc.  
3. Problèmes explicitement marqués comme "No help needed" (y compris les problèmes dans les dépôts [Byaidu/PDFMathTranslate](Byaidu/PDFMathTranslate) et [PDFMathTranslate/PDFMathTranslate-next](PDFMathTranslate/PDFMathTranslate-next)).  
4. Autres contributions jugées inappropriées par les mainteneurs.  
5. Contribution à la documentation, mais modification de la documentation dans des langues autres que l'anglais.  
6. PRs nécessitant la modification de fichiers PDF.

Veuillez ne PAS soumettre de PR liées aux types mentionnés ci-dessus.

> [!NOTE]
>
> Si vous souhaitez contribuer à la documentation, veuillez **uniquement modifier la version anglaise de la documentation**. Les autres versions linguistiques sont traduites par les contributeurs eux-mêmes.

## Processus de contribution

1. Forkez ce dépôt et clonez-le localement.
2. Créez une nouvelle branche : `git checkout -b feature/<feature-name>`.
3. Développez et assurez-vous que votre code répond aux exigences.
4. Validez votre code :
   ```bash
   git add .
   git commit -m "<semantic commit message>"
   ```
5. Poussez vers votre dépôt : `git push origin feature/<feature-name>`.
6. Créez une PR sur GitHub, fournissez une description détaillée et demandez une revue à [@awwaawwa](https://github.com/awwaawwa).
7. Assurez-vous que toutes les vérifications automatisées passent.

> [!TIP]
>
> Vous n'avez pas besoin d'attendre que votre développement soit entièrement terminé pour créer une PR. En créer une tôt nous permet d'examiner votre implémentation et de fournir des suggestions.
>
> Si vous avez des questions sur le code source ou des sujets connexes, veuillez contacter le mainteneur à aw@funstory.ai.
>
> Les fichiers de ressources pour la version 2.0 sont partagés avec [BabelDOC](https://github.com/funstory-ai/BabelDOC). Le code pour télécharger les ressources associées se trouve dans BabelDOC. Si vous souhaitez ajouter de nouveaux fichiers de ressources, veuillez contacter le mainteneur de BabelDOC à aw@funstory.ai.

## Exigences de base

<h4 id="sop">1. Flux de travail</h4>

   - Veuillez forker à partir de la branche `main` et développer sur votre branche forké.  
   - Lors de la soumission d'une Pull Request (PR), fournissez une description détaillée de vos modifications.  
   - Si votre PR ne passe pas les vérifications automatisées (indiquées par `checks failed` et une croix rouge), veuillez consulter les `details` correspondants et modifier votre soumission pour vous assurer que la nouvelle PR passe toutes les vérifications.


<h4 id="dev&test">2. Développement et tests</h4>

   - Utilisez la commande `pip install -e .` pour le développement et les tests.


<h4 id="format">3. Formatage du code</h4>

   - Configurez l'outil `pre-commit` et activez `black` et `flake8` pour le formatage du code.


<h4 id="requpdate">4. Mises à jour des dépendances</h4>

   - Si vous introduisez de nouvelles dépendances, veuillez mettre à jour la liste des dépendances dans le fichier `pyproject.toml` en temps opportun.


<h4 id="docupdate">5. Mises à jour de la documentation</h4>

   - Si vous ajoutez de nouvelles options de ligne de commande, veuillez mettre à jour la liste des options de ligne de commande dans toutes les versions linguistiques du fichier `README.md` en conséquence.


<h4 id="commitmsg">6. Messages de commit</h4>

   - Utilisez [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), par exemple : `feat(translator): add openai`.


<h4 id="codestyle">7. Style de codage</h4>

   - Assurez-vous que le code soumis respecte les normes de base de style de codage.
   - Utilisez soit snake_case soit camelCase pour la dénomination des variables.


<h4 id="doctypo">8. Formatage de la documentation</h4>

   - Pour le formatage de `README.md`, veuillez suivre les [Chinese Copywriting Guidelines](https://github.com/sparanoid/chinese-copywriting-guidelines).
   - Assurez-vous que la documentation en anglais et en chinois est toujours à jour ; les mises à jour de la documentation dans d'autres langues sont facultatives.

## Ajout d'un moteur de traduction

1. Ajoutez une nouvelle classe de configuration de traducteur dans le fichier `pdf2zh/config/translate_engine_model.py`.
2. Ajoutez une instance de la nouvelle classe de configuration de traducteur à l'alias de type `TRANSLATION_ENGINE_SETTING_TYPE` dans le même fichier.
3. Ajoutez la nouvelle classe d'implémentation du traducteur dans le dossier `pdf2zh/translator/translator_impl`.

> [!NOTE]
>
> Ce projet n'a pas l'intention de prendre en charge les moteurs de traduction avec un RPS (requêtes par seconde) inférieur à 4. Veuillez ne pas soumettre de support pour ces moteurs.

## Structure du projet

- **config folder** : Système de configuration.
- **translator folder** : Implémentations liées au traducteur.
- **gui.py** : Fournit l'interface GUI.
- **const.py** : Quelques constantes.
- **main.py** : Fournit l'outil en ligne de commande.
- **high_level.py** : Interfaces de haut niveau basées sur BabelDOC.
- **http_api.py** : Fournit l'API HTTP (non démarrée).

## Nous contacter

Si vous avez des questions, veuillez soumettre vos commentaires via Issue ou rejoindre notre groupe Telegram. Merci pour votre contribution !

> [!TIP]
>
> [Immersive Translate](https://immersivetranslate.com) sponsorise des codes d'abonnement Pro mensuels pour les contributeurs actifs de ce projet. Pour plus de détails, veuillez consulter : [Règles de récompense des contributeurs BabelDOC/PDFMathTranslate](https://funstory-ai.github.io/BabelDOC/CONTRIBUTOR_REWARD/)

<div align="right"> 
<h6><small>Une partie du contenu de cette page a été traduite par GPT et peut contenir des erreurs.</small></h6>