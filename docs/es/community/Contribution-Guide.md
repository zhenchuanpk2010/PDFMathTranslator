# Contribuir al proyecto

> [!CAUTION]
>
> Los mantenedores actuales del proyecto están investigando la internacionalización automatizada de la documentación. Por lo tanto, ¡NO se aceptarán PRs relacionados con la internacionalización/traducción de la documentación!
>
> ¡Por favor, NO envíes PRs relacionados con la internacionalización/traducción de la documentación!

¡Gracias por tu interés en este proyecto! Antes de empezar a contribuir, por favor tómate un tiempo para leer las siguientes pautas para asegurar que tu contribución pueda ser aceptada sin problemas.

## Tipos de contribuciones no aceptadas

1. Internacionalización/traducción de documentación
2. Contribuciones relacionadas con la infraestructura central, como API HTTP, etc.
3. Problemas marcados explícitamente como "No se necesita ayuda" (incluyendo problemas en los repositorios [Byaidu/PDFMathTranslate](Byaidu/PDFMathTranslate) y [PDFMathTranslate/PDFMathTranslate-next](PDFMathTranslate/PDFMathTranslate-next)).
4. Otras contribuciones consideradas inapropiadas por los mantenedores.
5. Contribuir a la documentación, pero modificando la documentación en idiomas distintos al inglés.
6. PRs que requieran modificar archivos PDF.

Por favor NO envíes PRs relacionados con los tipos mencionados anteriormente.

> [!NOTE]
>
> Si deseas contribuir a la documentación, por favor **solo modifiques la versión en inglés de la documentación**. Las versiones en otros idiomas son traducidas por los propios colaboradores.

## Proceso de contribución

1. Haz un fork de este repositorio y clónalo localmente.
2. Crea una nueva rama: `git checkout -b feature/<feature-name>`.
3. Desarrolla y asegúrate de que tu código cumple con los requisitos.
4. Haz commit de tu código:
   ```bash
   git add .
   git commit -m "<semantic commit message>"
   ```
5. Haz push a tu repositorio: `git push origin feature/<feature-name>`.
6. Crea un PR en GitHub, proporciona una descripción detallada y solicita una revisión a [@awwaawwa](https://github.com/awwaawwa).
7. Asegúrate de que todas las verificaciones automáticas pasan.

> [!TIP]
>
> No es necesario esperar hasta que tu desarrollo esté completamente terminado para crear un PR. Crear uno temprano nos permite revisar tu implementación y proporcionar sugerencias.
>
> Si tienes alguna pregunta sobre el código fuente o temas relacionados, por favor contacta al mantenedor en aw@funstory.ai.
>
> Los archivos de recursos para la versión 2.0 se comparten con [BabelDOC](https://github.com/funstory-ai/BabelDOC). El código para descargar los recursos relacionados está en BabelDOC. Si deseas añadir nuevos archivos de recursos, por favor contacta al mantenedor de BabelDOC en aw@funstory.ai.

## Requisitos básicos

<h4 id="sop">1. Flujo de trabajo</h4>

- Por favor, haz un fork desde la rama `main` y desarrolla en tu rama bifurcada.
   - Al enviar un Pull Request (PR), proporciona una descripción detallada de tus cambios.
   - Si tu PR no pasa las verificaciones automáticas (indicado por `checks failed` y una cruz roja), revisa los `details` correspondientes y modifica tu envío para asegurar que el nuevo PR pase todas las verificaciones.


<h4 id="dev&test">2. Desarrollo y Pruebas</h4>

- Usa el comando `pip install -e .` para desarrollo y pruebas.


<h4 id="formato">3. Formateo de código</h4>

- Configurar la herramienta `pre-commit` y habilitar `black` y `flake8` para el formato del código.


<h4 id="requpdate">4. Actualizaciones de dependencias</h4>

- Si introduces nuevas dependencias, actualiza la lista de dependencias en el archivo `pyproject.toml` de manera oportuna.


<h4 id="docupdate">5. Actualizaciones de documentación</h4>

- Si añades nuevas opciones de línea de comandos, actualiza la lista de opciones de línea de comandos en todas las versiones de idioma del archivo `README.md` correspondientemente.


<h4 id="commitmsg">6. Mensajes de commit</h4>

- Usa [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), por ejemplo: `feat(translator): add openai`.


<h4 id="codestyle">7. Estilo de codificación</h4>

- Asegúrate de que el código enviado cumpla con los estándares básicos de estilo de codificación.
   - Utiliza snake_case o camelCase para el nombrado de variables.


<h4 id="doctypo">8. Formato de documentación</h4>

- Para el formato de `README.md`, sigue las [Directrices de redacción en chino](https://github.com/sparanoid/chinese-copywriting-guidelines).
   - Asegúrate de que tanto la documentación en inglés como en chino estén siempre actualizadas; las actualizaciones de documentación en otros idiomas son opcionales.

## Añadir un motor de traducción

1. Añade una nueva clase de configuración del traductor en el archivo `pdf2zh/config/translate_engine_model.py`.
2. Añade una instancia de la nueva clase de configuración del traductor al alias de tipo `TRANSLATION_ENGINE_SETTING_TYPE` en el mismo archivo.
3. Añade la nueva clase de implementación del traductor en la carpeta `pdf2zh/translator/translator_impl`.

> [!NOTE]
>
> Este proyecto no tiene la intención de soportar ningún motor de traducción con un RPS (solicitudes por segundo) inferior a 4. Por favor, no envíes soporte para dichos motores.

## Estructura del proyecto

- **config folder**: Sistema de configuración.
- **translator folder**: Implementaciones relacionadas con el traductor.
- **gui.py**: Proporciona la interfaz gráfica de usuario.
- **const.py**: Algunas constantes.
- **main.py**: Proporciona la herramienta de línea de comandos.
- **high_level.py**: Interfaces de alto nivel basadas en BabelDOC.
- **http_api.py**: Proporciona API HTTP (no iniciado).

## Contáctanos

Si tienes alguna pregunta, por favor envía tus comentarios a través de un Issue o únete a nuestro grupo de Telegram. ¡Gracias por tu contribución!

> [!TIP]
>
> [Immersive Translate](https://immersivetranslate.com) patrocina códigos de membresía Pro mensuales para los contribuyentes activos de este proyecto. Para más detalles, consulta: [BabelDOC/PDFMathTranslate Reglas de recompensa para contribuyentes](https://funstory-ai.github.io/BabelDOC/CONTRIBUTOR_REWARD/)

<div align="right"> 
<h6><small>Parte del contenido de esta página ha sido traducido por GPT y puede contener errores.</small></h6>