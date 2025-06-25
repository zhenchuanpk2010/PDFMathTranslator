<div align="center">

<img src="./docs/images/banner.png" width="320px"  alt="banner"/>

<h2 id="titre">PDFMathTranslate</h2>

<p>

<!-- PyPI -->
  <a href="https://pypi.org/project/pdf2zh-next/">
    <img src="https://img.shields.io/pypi/v/pdf2zh-next"></a>
  <a href="https://pepy.tech/projects/pdf2zh-next">
    <img src="https://static.pepy.tech/badge/pdf2zh-next"></a>
  <a href="https://hub.docker.com/repository/docker/awwaawwa/pdfmathtranslate-next/tags">
    <img src="https://img.shields.io/docker/pulls/awwaawwa/pdfmathtranslate-next"></a>
  <a href="https://hellogithub.com/repository/8ec2cfd3ef744762bf531232fa32bc47" target="_blank"><img src="https://api.hellogithub.com/v1/widgets/recommend.svg?rid=8ec2cfd3ef744762bf531232fa32bc47&claim_uid=JQ0yfeBNjaTuqDU&theme=small" alt="À la une｜HelloGitHub" /></a>


<a href="https://t.me/+Z9_SgnxmsmA5NzBl">
    <img src="https://img.shields.io/badge/Telegram-2CA5E0?style=flat-squeare&logo=telegram&logoColor=white"></a>

<!-- License -->
  <a href="./LICENSE">
    <img src="https://img.shields.io/github/license/PDFMathTranslate/PDFMathTranslate-next"></a>
</p>

<a href="https://trendshift.io/repositories/12424" target="_blank"><img src="https://trendshift.io/api/badge/repositories/12424" alt="Byaidu%2FPDFMathTranslate | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>

</div>

Traduction de documents scientifiques PDF et comparaison bilingue.

- 📊 Préserve les formules, graphiques, tables des matières et annotations _([aperçu](#aperçu))_.
- 🌐 Prend en charge [plusieurs langues](https://pdf2zh-next.com/supported_languages.html) et divers [services de traduction](https://pdf2zh-next.com/advanced/Documentation-des-services-de-traduction.html).
- 🤖 Fournit un [outil en ligne de commande](https://pdf2zh-next.com/commencer/UTILISATION_ligne-de-commande.html), une [interface utilisateur interactive](https://pdf2zh-next.com/commencer/UTILISATION_webui.html) et [Docker](https://pdf2zh-next.com/commencer/INSTALLATION_docker.html)

N'hésitez pas à fournir des retours dans les [GitHub Issues](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues) ou le [Groupe Telegram](https://t.me/+Z9_SgnxmsmA5NzBl).

Pour plus de détails sur comment contribuer, veuillez consulter le [Guide de contribution](https://pdf2zh-next.com/communauté/Guide-de-contribution.html).

<h2 id="mises-à-jour">Mises à jour</h2>

- [4 juin 2025] Le projet est renommé et déplacé vers [PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next) (par [@awwaawwa](https://github.com/awwaawwa))
- [3 mars 2025] Support expérimental pour le nouveau backend [BabelDOC](https://github.com/funstory-ai/BabelDOC) WebUI ajouté comme option expérimentale (par [@awwaawwa](https://github.com/awwaawwa))
- [22 fév. 2025] Meilleure CI de release et exe Windows-amd64 bien packagé (par [@awwaawwa](https://github.com/awwaawwa))
- [24 déc. 2024] Le traducteur prend désormais en charge les modèles locaux sur [Xinference](https://github.com/xorbitsai/inference) _(par [@imClumsyPanda](https://github.com/imClumsyPanda))_
- [19 déc. 2024] Les documents non-PDF/A sont désormais pris en charge en utilisant `-cp` _(par [@reycn](https://github.com/reycn))_
- [13 déc. 2024] Support supplémentaire pour le backend par _(par [@YadominJinta](https://github.com/YadominJinta))_
- [10 déc. 2024] Le traducteur prend désormais en charge les modèles OpenAI sur Azure _(par [@yidasanqian](https://github.com/yidasanqian))_

<h2 id="aperçu">Aperçu</h2>

<div align="center">
<!-- <img src="./docs/images/preview.gif" width="80%"  alt="preview"/> -->

<img src="https://s.immersivetranslate.com/assets/r2-uploads/images/babeldoc-preview.png" width="80%"/>
</div>

<h2 id="demo">Service en ligne 🌟</h2>

> [!NOTE]
>
> pdf2zh 2.0 ne propose actuellement pas de démonstration en ligne

Vous pouvez essayer notre application en utilisant l'une des démonstrations suivantes :

- [v1.x Service public gratuit](https://pdf2zh.com/) en ligne sans installation _(recommandé)_.
- [Immersive Translate - BabelDOC](https://app.immersivetranslate.com/babel-doc/) 1000 pages gratuites par mois. _(recommandé)_

<!-- - [Démo hébergée sur HuggingFace](https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker)
- [Démo hébergée sur ModelScope](https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate) sans installation. -->

Notez que les ressources de calcul de la démo sont limitées, veuillez donc éviter de les abuser.

<h2 id="install">Installation et Utilisation</h2>

### Installation

1. [**Windows EXE**](https://pdf2zh-next.com/commencer/INSTALLATION_winexe.html) <small>Recommandé pour Windows</small>
2. [**Docker**](https://pdf2zh-next.com/commencer/INSTALLATION_docker.html) <small>Recommandé pour Linux</small>
3. [**uv** (un gestionnaire de paquets Python)](https://pdf2zh-next.com/commencer/INSTALLATION_uv.html) <small>Recommandé pour macOS</small>

---

### Utilisation

1. [Utilisation de **WebUI**](https://pdf2zh-next.com/getting-started/USAGE_webui.html)
2. [Utilisation du **Plugin Zotero**](https://github.com/guaguastandup/zotero-pdf2zh) (Programme tiers)
3. [Utilisation de la **Ligne de commande**](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)

Pour différents cas d'utilisation, nous proposons des méthodes distinctes pour utiliser notre programme. Consultez [cette page](./getting-started/getting-started.md) pour plus d'informations.

<h2 id="usage">Options avancées</h2>

Pour des explications détaillées, veuillez vous référer à notre document sur [l'Utilisation avancée](https://pdf2zh-next.com/advanced/advanced.html) pour une liste complète de chaque option.

<h2 id="downstream">Développement secondaire (APIs)</h2>

> [!NOTE]
>
> Actuellement, aucune documentation pertinente n'est fournie. Elle sera complétée ultérieurement. Veuillez patienter.

<!-- Pour les applications en aval, veuillez consulter notre document sur les [Détails de l'API](./docs/APIS.md) pour plus d'informations concernant :

- [API Python](./docs/APIS.md#api-python), comment utiliser le programme dans d'autres programmes Python
- [API HTTP](./docs/APIS.md#api-http), comment communiquer avec un serveur sur lequel le programme est installé -->

<h2 id="langcode">Code de langue</h2>

Si vous ne savez pas quel code utiliser pour traduire dans la langue dont vous avez besoin, consultez [cette documentation](https://pdf2zh-next.com/advanced/Language-Codes.html)

<!-- 
<h2 id="todo">TODOs</h2>

- [ ] Analyser la mise en page avec des modèles basés sur DocLayNet, [PaddleX](https://github.com/PaddlePaddle/PaddleX/blob/17cc27ac3842e7880ca4aad92358d3ef8555429a/paddlex/repo_apis/PaddleDetection_api/object_det/official_categories.py#L81), [PaperMage](https://github.com/allenai/papermage/blob/9cd4bb48cbedab45d0f7a455711438f1632abebe/README.md?plain=1#L102), [SAM2](https://github.com/facebookresearch/sam2)

- [ ] Corriger la rotation des pages, la table des matières, le format des listes

- [ ] Corriger les formules en pixels dans les anciens articles

- [ ] Réessai asynchrone sauf KeyboardInterrupt

- [ ] Algorithme de Knuth–Plass pour les langues occidentales

- [ ] Prendre en charge les fichiers non-PDF/A

- [ ] Plugins pour [Zotero](https://github.com/zotero/zotero) et [Obsidian](https://github.com/obsidianmd/obsidian-releases) -->

<h2 id="acknowledgement">Remerciements</h2>

- [Immersive Translation](https://immersivetranslate.com) sponsorise des codes de rédemption mensuels pour l'abonnement Pro destinés aux contributeurs actifs de ce projet. Pour plus de détails, consultez : [CONTRIBUTOR_REWARD.md](https://github.com/funstory-ai/BabelDOC/blob/main/docs/CONTRIBUTOR_REWARD.md)

- Version 1.x : [Byaidu/PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate)

- Nouveau backend : [BabelDOC](https://github.com/funstory-ai/BabelDOC)

- Fusion de documents : [PyMuPDF](https://github.com/pymupdf/PyMuPDF)

- Analyse de documents : [Pdfminer.six](https://github.com/pdfminer/pdfminer.six)

- Extraction de documents : [MinerU](https://github.com/opendatalab/MinerU)

- Prévisualisation de documents : [Gradio PDF](https://github.com/freddyaboulton/gradio-pdf)

- Traduction multithread : [MathTranslate](https://github.com/SUSYUSTC/MathTranslate)

- Analyse de mise en page : [DocLayout-YOLO](https://github.com/opendatalab/DocLayout-YOLO)

- Standard de document : [PDF Explained](https://zxyle.github.io/PDF-Explained/), [PDF Cheat Sheets](https://pdfa.org/resource/pdf-cheat-sheets/)

- Police multilingue : [Go Noto Universal](https://github.com/satbyy/go-noto-universal)

- [Asynchronize](https://github.com/multimeric/Asynchronize/tree/master?tab=readme-ov-file)

- [Journalisation enrichie avec multiprocessing](https://github.com/SebastianGrans/Rich-multiprocess-logging/tree/main)

<h2 id="conduct">Avant de soumettre votre code</h2>

Nous encourageons la participation active des contributeurs pour améliorer pdf2zh. Avant de soumettre votre code, veuillez consulter notre [Code de conduite](https://pdf2zh-next.com/community/CODE_OF_CONDUCT.html) et notre [Guide de contribution](https://pdf2zh-next.com/community/Contribution-Guide.html).

<h2 id="contrib">Contributeurs</h2>

<a href="https://github.com/PDFMathTranslate/PDFMathTranslate-next/graphs/contributors">
  <img src="https://opencollective.com/PDFMathTranslate/contributors.svg?width=890&button=false" />
</a>

![Alt](https://repobeats.axiom.co/api/embed/45529651750579e099960950f757449a410477ad.svg "Image d'analyse Repobeats")

<h2 id="star_hist">Historique des étoiles</h2>

<a href="https://star-history.com/#PDFMathTranslate/PDFMathTranslate-next&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date" />
   <img alt="Graphique de l'historique des étoiles" src="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date"/>
 </picture>
</a>

<div align="right"> 
<h6><small>Une partie du contenu de cette page a été traduite par GPT et peut contenir des erreurs.</small></h6>