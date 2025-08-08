[**Empezar**](./getting-started.md) > **Instalación** > **Windows EXE** _(actual)_

---

### Instalar PDFMathTranslate mediante archivo .exe

***Paso 1*** | Descarga `pdf2zh-<version>-with-assets-win64.zip` desde la [página de lanzamientos](https://github.com/PDFMathTranslate/PDFMathTranslate-next/releases).

> [!TIP]
> **¿Cuál es la diferencia entre `pdf2zh-<version>-with-assets-win64.zip` y `pdf2zh-<version>-win64.zip`?**
>
> - Si es la primera vez que descargas y usas PDFMathTranslate, se recomienda descargar `pdf2zh-<version>-with-assets-win64.zip`.
> - El archivo `pdf2zh-<version>-with-assets-win64.zip` incluye archivos de recursos (como fuentes y modelos) en comparación con `pdf2zh-<version>-win64.zip`.
> - La versión sin recursos también descargará dinámicamente los recursos al ejecutarse, pero la descarga puede fallar debido a problemas de red.

***Paso 2*** | Descomprime `pdf2zh-<version>-with-assets-win64.zip` y navega hasta la carpeta `pdf2zh`. La descompresión puede tomar un tiempo, por favor ten paciencia.

***Paso 3*** | Navega hasta la carpeta `pdf2zh`, luego haz doble clic en `pdf2zh.exe`.

> [!TIP]
> **No se puede ejecutar el archivo .exe**
>
> Si tienes problemas al ejecutar pdf2zh.exe, por favor instala `https://aka.ms/vs/17/release/vc_redist.x64.exe` e inténtalo de nuevo.

***Paso 4*** | Aparecerá una terminal después de hacer doble clic en el archivo exe. Después de aproximadamente medio minuto a un minuto, se abrirá una página web en tu navegador predeterminado. Si esto no ocurre, puedes intentar acceder manualmente a `http://localhost:7860/`.

> [!NOTE]
>
> Si encuentras algún problema al usar WebUI, por favor consulta [esta página web](./USAGE_webui.md).

***Paso 5*** | ¡Disfruta!

> [!TIP]
> **Puedes usar el archivo .exe mediante la línea de comandos**
>
> Usa el archivo .exe a través de la línea de comandos de la siguiente manera:
>
> - Abre tu terminal y navega hasta la carpeta que contiene el archivo .exe:
>
> ```bash
> cd /path/pdf2zh_next/build
> ```
>
> - Llama al archivo .exe:
>
> ```bash
> ./pdf2zh_next.exe "document.pdf"
> ```
>
> Puedes usar otros parámetros de línea de comandos como de costumbre:
>
> ```bash
> ./pdf2zh_next.exe "document.pdf" --lang-in en --lang-out ja
> ```
>
> Si necesitas más información sobre el uso de la línea de comandos, consulta este artículo.

<div align="right"> 
<h6><small>Parte del contenido de esta página ha sido traducido por GPT y puede contener errores.</small></h6>