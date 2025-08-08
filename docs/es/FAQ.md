Algunas preguntas se hacen con frecuencia, por lo que hemos proporcionado una lista para los usuarios que encuentren problemas similares.

## ¿Se requiere una GPU?
- **Pregunta**:
¿El programa utiliza inteligencia artificial para reconocer y extraer documentos, se requiere una GPU?

- **Respuesta**:
**No se requiere una GPU.** Pero si tienes una GPU, el programa la usará automáticamente para un mayor rendimiento.

## ¿Descarga interrumpida?
- **Pregunta**:
Encontré el siguiente error de interrupción mientras descargaba el modelo. ¿Qué debo hacer?

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **Respuesta**:
La red está recibiendo interferencias, por favor usa un enlace de red estable o intenta evitar la intervención de la red.

## ¿Cómo actualizar a la última versión?
- **Pregunta**:
Quiero usar algunas de las funciones de la última versión, ¿cómo la actualizo?

- **Respuesta**:
`pip install -U pdf2zh`


## Los siguientes archivos no existen: example.pdf
- **Problema**:
Al ejecutar el programa, los usuarios tendrían las siguientes salidas: `Los siguientes archivos no existen: example.pdf` si el documento no se encontró.

- **Solución**:
  - Abre la línea de comandos en el directorio donde se encuentra el archivo, o
  - Ingresa la ruta completa del archivo directamente después de pdf2zh, o
  - Usa el modo interactivo `pdf2zh -i` para arrastrar y soltar archivos directamente


## Error SSL y otros problemas de red
- **Problema**:
Al descargar modelos de hugging face, los usuarios en China pueden experimentar errores de red. Por ejemplo, en [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55), [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70).

- **Solución**:
  - [Bypass GFW](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Usar espejo de Hugging Face](https://hf-mirror.com/).
  - [Usar versión portable](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [Usar Docker en su lugar](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [Actualizar certificados](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), como se sugiere en [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55).

## Localhost no es accesible
Por favor, vea a continuación.

## Error al iniciar la GUI usando 0.0.0.0
- **Problema**:
El uso de software de proxy en modo global puede impedir que Gradio se inicie correctamente. Por ejemplo, en [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77).

- **Solución**:
Modo de uso de reglas

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>Parte del contenido de esta página ha sido traducido por GPT y puede contener errores.</small></h6>