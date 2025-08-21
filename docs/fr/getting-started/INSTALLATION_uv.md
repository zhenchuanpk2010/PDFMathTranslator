[**Commencer**](./getting-started.md) > **Installation** > **uv** _(actuel)_

---

### Installer PDFMathTranslate via uv

#### Qu'est-ce que uv ? Comment l'installer ?

uv est un gestionnaire de paquets et de projets Python extrêmement rapide, écrit en Rust.
<br>
Pour installer uv sur votre ordinateur, veuillez consulter [cet article](https://docs.astral.sh/uv/getting-started/installation/).

---

#### Installation

1. Python installé (version 3.10 <= version <= 3.12) ;

2. Utilisez la commande suivante pour utiliser notre package :

    ```bash
    pip install uv
    uv tool install --python 3.12 pdf2zh-next
    ```

Après l'installation, vous pouvez commencer la traduction via la **ligne de commande** ou le **WebUI**.

!!! Warning

    Si vous voyez l'erreur `command not found: pdf2zh_next` lors de l'exécution, veuillez configurer les variables d'environnement comme suit et réessayer :

    === "macOS et Linux"

        Ajoutez ce qui suit à votre ~/.zshrc :

        ```console
        export PATH="$PATH:/Users/Username/.local/bin"
        ```

        Puis redémarrez votre terminal

    === "Windows"

        Entrez ce qui suit dans PowerShell :

        ```powershell
        $env:Path = "C:\Users\Username\.local\bin;$env:Path"
        ```

        Puis redémarrez votre terminal

> [!NOTE]
> Si vous rencontrez des problèmes lors de l'utilisation de WebUI, veuillez consulter [Utilisation --> WebUI](./USAGE_webui.md).

> [!NOTE]
> Si vous rencontrez des problèmes lors de l'utilisation de la ligne de commande, veuillez consulter [Utilisation --> Ligne de commande](./USAGE_commandline.md).

<div align="right"> 
<h6><small>Une partie du contenu de cette page a été traduite par GPT et peut contenir des erreurs.</small></h6>