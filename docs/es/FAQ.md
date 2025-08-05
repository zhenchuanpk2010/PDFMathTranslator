Algunas preguntas se hacen con frecuencia, por lo que hemos proporcionado una lista para los usuarios que encuentren problemas similares.

## ¿Se requiere una GPU?
- **Pregunta**:
## ¿Se requiere una GPU?

- **Respuesta**:
**No se requiere una GPU.** Pero si tienes una GPU, el programa la usará automáticamente para un mayor rendimiento.

## ¿Descarga interrumpida?
- **Pregunta**:
Encontré el siguiente error de interrupción mientras descargaba el modelo. ¿Qué debo hacer?

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **Respuesta**:
La red está recibiendo interferencias, por favor utiliza un enlace de red estable o intenta evitar la intervención de la red.

## ¿Cómo actualizar a la última versión?
- **Pregunta**:
Quiero usar algunas de las funciones de la última versión, ¿cómo la actualizo?

- **Respuesta**:
`pip install -U pdf2zh`


## Los siguientes archivos no existen: example.pdf
- **Problema**:
Al ejecutar el programa, los usuarios tendrían las siguientes salidas: `The following files do not exist: example.pdf` si el documento no se encontró.

- **Solución**:
  - Abre la línea de comandos en el directorio donde se encuentra el archivo, o
  - Ingresa la ruta completa del archivo directamente después de pdf2zh, o
  - Usa el modo interactivo `pdf2zh -i` para arrastrar y soltar archivos directamente


## Error de SSL y otros problemas de red

Si estás utilizando **pdf2zh** y te encuentras con un error de SSL u otros problemas de red, aquí hay algunas soluciones comunes:

1. **Verifica tu conexión a Internet**:
   - Asegúrate de que tu conexión a Internet sea estable.
   - Intenta acceder a otros sitios web para confirmar que no hay problemas generales de red.

2. **Actualiza tu sistema operativo y software**:
   - Asegúrate de que tu sistema operativo y **pdf2zh** estén actualizados a la última versión.

3. **Configuración de proxy**:
   - Si estás detrás de un proxy, configura **pdf2zh** para que lo use. Consulta la [Documentación de servicios de traducción](#documentación-de-servicios-de-traducción) para más detalles.

4. **Desactiva temporalmente el firewall/antivirus**:
   - A veces, el firewall o el antivirus pueden bloquear la conexión. Intenta desactivarlos temporalmente para ver si resuelve el problema.

5. **Verifica la fecha y hora de tu sistema**:
   - Un error común de SSL ocurre cuando la fecha y hora de tu sistema son incorrectas. Asegúrate de que estén configuradas correctamente.

6. **Reinstala los certificados SSL**:
   - Si el problema persiste, reinstala los certificados SSL en tu sistema.

Si ninguno de estos pasos resuelve el problema, consulta la sección [Comunidad](#comunidad) para obtener ayuda adicional.
- **Problema**:
Al descargar modelos de Hugging Face, los usuarios en China pueden experimentar errores de red. Por ejemplo, en los [issues #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55) y [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70).

- **Solución**:
  - [Bypass GFW](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Usar espejo de Hugging Face](https://hf-mirror.com/).
  - [Usar versión portable](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [Usar Docker en su lugar](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [Actualizar certificados](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), como se sugiere en [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55).

# Localhost no es accesible

Si estás ejecutando `pdf2zh` en un servidor remoto (como un servidor en la nube), es posible que no puedas acceder a la interfaz web a través de `localhost` o `127.0.0.1`. Esto se debe a que la interfaz web solo está vinculada a la dirección IP local del servidor.

Para solucionar esto, puedes:

1. **Usar un túnel SSH** (recomendado para servidores remotos):
   ```bash
   ssh -L 8501:localhost:8501 tu_usuario@tu_servidor
   ```
   Luego, abre `http://localhost:8501` en tu navegador local.

2. **Cambiar el host de la interfaz web** (no recomendado para entornos de producción):
   ```bash
   pdf2zh --host 0.0.0.0
   ```
   Esto hará que la interfaz web sea accesible desde cualquier dirección IP, pero ten en cuenta los riesgos de seguridad.
Por favor, consulta a continuación.

## Error al iniciar la GUI usando 0.0.0.0
- **Problema**:
El uso de software de proxy en modo global puede impedir que Gradio se inicie correctamente. Por ejemplo, en el [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77).

- **Solución**:
Usar modo de regla

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>Parte del contenido de esta página ha sido traducido por GPT y puede contener errores.</small></h6>