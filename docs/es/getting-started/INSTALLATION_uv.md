[**Empezar**](./getting-started.md) > **Instalación** > **uv** _(actual)_

---

### Instalar PDFMathTranslate mediante uv

#### ¿Qué es uv? ¿Cómo instalarlo?

uv es un gestor de paquetes y proyectos de Python extremadamente rápido, escrito en Rust.
<br>
Para instalar uv en tu computadora, consulta [este artículo](https://docs.astral.sh/uv/getting-started/installation/).

---

#### Instalación

1. Python instalado (versión 3.10 <= versión <= 3.12);

2. Utilice el siguiente comando para usar nuestro paquete:

    ```bash
    pip install uv
    uv tool install --python 3.12 pdf2zh-next
    ```

Después de la instalación, puedes comenzar la traducción mediante la **línea de comandos** o **WebUI**.

!!! Warning

    Si ves el error `command not found: pdf2zh_next` al ejecutar, por favor configura las variables de entorno de la siguiente manera e inténtalo de nuevo:

    === "macOS y Linux"

        Añade lo siguiente a tu ~/.zshrc:

        ```console
        export PATH="$PATH:/Users/Username/.local/bin"
        ```

        Luego reinicia tu terminal

    === "Windows"

        Ingresa lo siguiente en PowerShell:

        ```powershell
        $env:Path = "C:\Users\Username\.local\bin;$env:Path"
        ```

        Luego reinicia tu terminal

> [!NOTE]
> Si encuentras algún problema al usar WebUI, consulta [Uso --> WebUI](./USAGE_webui.md).

> [!NOTE]
> Si encuentras algún problema al usar la línea de comandos, consulta [Uso --> Línea de comandos](./USAGE_commandline.md).

<div align="right"> 
<h6><small>Parte del contenido de esta página ha sido traducido por GPT y puede contener errores.</small></h6>