[**Commencer**](./getting-started.md) > **Installation** > **Windows EXE** _(current)_

---

### Installer PDFMathTranslate via fichier .exe

***Étape 1*** | Téléchargez `pdf2zh-<version>-with-assets-win64.zip` depuis la [page des versions](https://github.com/PDFMathTranslate/PDFMathTranslate-next/releases).

> [!TIP]
> **Quelle est la différence entre `pdf2zh-<version>-with-assets-win64.zip` et `pdf2zh-<version>-win64.zip` ?**
>
> - Si vous téléchargez et utilisez PDFMathTranslate pour la première fois, il est recommandé de télécharger `pdf2zh-<version>-with-assets-win64.zip`.
> - Le fichier `pdf2zh-<version>-with-assets-win64.zip` inclut les fichiers de ressources (tels que les polices et les modèles) contrairement à `pdf2zh-<version>-win64.zip`.
> - La version sans ressources téléchargera également les ressources dynamiquement lors de l'exécution, mais le téléchargement peut échouer en raison de problèmes de réseau.

***Étape 2*** | Décompressez `pdf2zh-<version>-with-assets-win64.zip` et accédez au dossier `pdf2zh`. La décompression prend un certain temps, soyez patient.

***Étape 3*** | Accédez au dossier `pdf2zh`, puis double-cliquez sur `pdf2zh.exe`.

> [!TIP]
> **Impossible d'exécuter le fichier .exe**
>
> Si vous rencontrez des problèmes pour exécuter pdf2zh.exe, veuillez installer `https://aka.ms/vs/17/release/vc_redist.x64.exe` et réessayer.

***Étape 4*** | Un terminal s'ouvrira après avoir double-cliqué sur le fichier exe. Après environ une demi-minute à une minute, une page web s'ouvrira dans votre navigateur par défaut. Si cela ne se produit pas, vous pouvez essayer d'accéder manuellement à `http://localhost:7860/`.

> [!NOTE]
>
> Si vous rencontrez des problèmes lors de l'utilisation de WebUI, veuillez consulter [cette page web](./USAGE_webui.md).

***Étape 5*** | Profitez-en !

> [!TIP]
> **Vous pouvez utiliser le fichier .exe via la ligne de commande**
>
> Utilisez le fichier .exe via la ligne de commande comme suit :
>
> - Lancez votre terminal et naviguez vers le dossier contenant le fichier .exe :
>
> ```bash
> cd /path/pdf2zh_next/build
> ```
>
> - Appelez le fichier .exe :
>
> ```bash
> ./pdf2zh_next.exe "document.pdf"
> ```
>
> Vous pouvez utiliser d'autres paramètres de ligne de commande comme d'habitude :
>
> ```bash
> ./pdf2zh_next.exe "document.pdf" --lang-in en --lang-out ja
> ```
>
> Si vous avez besoin de plus d'informations sur l'utilisation de la ligne de commande, veuillez vous référer à cet article.

<div align="right"> 
<h6><small>Une partie du contenu de cette page a été traduite par GPT et peut contenir des erreurs.</small></h6>