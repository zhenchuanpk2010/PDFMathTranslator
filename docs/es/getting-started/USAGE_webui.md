[**Empezar**](./getting-started.md) > **Instalación** > **WebUI** _(actual)_

---

### Usar PDFMathTranslate a través de Webui

#### Cómo abrir la página de WebUI:

Existen varios métodos para abrir la interfaz de WebUI. Si estás usando **Windows**, por favor consulta [este artículo](./INSTALLATION_winexe.md);

1. Python instalado (versión 3.10 <= versión <= 3.12)

2. Instala nuestro paquete:

3. Comienza a usar en el navegador:

    ```bash
    pdf2zh_next --gui
    ```

4. Si tu navegador no se ha iniciado automáticamente, ve a

    ```bash
    http://localhost:7860/
    ```

    Arrastra el archivo `PDF` a la ventana y haz clic en `Translate`.

<!-- <img src="./images/gui.gif" width="500"/> -->
<img src='./../images/gui.gif' width="500"/>

### Variables de entorno

Puedes configurar los idiomas de origen y destino utilizando variables de entorno:

- `PDF2ZH_LANG_FROM`: Establece el idioma de origen. Por defecto es "English".
- `PDF2ZH_LANG_TO`: Establece el idioma de destino. Por defecto es "Simplified Chinese".

## Vista previa

<img src="./../images/before.png" width="500"/>
<img src="./../images/after.png" width="500"/>

## Mantenimiento

### TRANSLATION

GUI mantenido por [Rongxin](https://github.com/reycn)

<div align="right"> 
<h6><small>Parte del contenido de esta página ha sido traducido por GPT y puede contener errores.</small></h6>