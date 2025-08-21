# SiliconFlow

## Servicio de traducción gratuito

[SiliconFlow](https://siliconflow.cn) proporciona un servicio de traducción gratuito para este proyecto.

Actualmente, el servicio de traducción gratuito utilizará el modelo `THUDM/GLM-4-9B-0414`.

### Uso

#### cli

```bash
pdf2zh_next --siliconflowfree example.pdf 
```

#### webui

1. Selecciona "SiliconFlowFree" de la lista desplegable "Opciones de traducción" - "Servicio".
2. Haz clic en el botón Traducir en la parte inferior de la página para comenzar la traducción.
3. Una vez completada la traducción, puedes encontrar el archivo PDF traducido en la sección "Traducido" en la parte inferior de la página.


### Política de privacidad

El contenido del archivo se enviará al servidor del mantenedor del proyecto [@awwaawwa](https://github.com/awwaawwa), y luego se reenviará a SiliconFlow para su traducción.

Los mantenedores de este proyecto solo recopilarán información de error devuelta por SiliconFlow para depurar los servicios relacionados. No se recopilará el contenido de su archivo.

Política de privacidad de SiliconFlow: [简体中文](https://docs.siliconflow.cn/cn/legals/privacy-policy)/[English](https://docs.siliconflow.cn/en/legals/privacy-policy)



## Usar otros modelos de SiliconFlow

[SiliconFlow](https://siliconflow.cn) también proporciona otros modelos para traducción.

### Uso

1. Registra una cuenta en [SiliconFlow](https://siliconflow.cn)

2. Crea una clave de API en [SiliconFlow API Key](https://cloud.siliconflow.cn/me/account/ak). Luego, haz clic en la clave para copiarla.

#### cli

```bash
pdf2zh_next --siliconflow --siliconflow-model "Pro/deepseek-ai/DeepSeek-V3" --siliconflow-api-key <your-api-key> example.pdf
```

#### webui

1. "Opciones de traducción" - Lista desplegable **"Servicio"**: Selecciona "SiliconFlow"  
2. "Opciones de traducción" - **"URL base para la API de SiliconFlow"**: Mantén el valor predeterminado  
3. "Opciones de traducción" - **"Modelo de SiliconFlow a utilizar"**: Ingresa "Pro/deepseek-ai/DeepSeek-V3" u otros modelos  
4. "Opciones de traducción" - **"Clave API para el servicio de SiliconFlow"**: Pega tu clave API  
5. Haz clic en el botón "Traducir" al final de la página para iniciar la traducción  
6. Una vez completada la traducción, podrás encontrar el archivo PDF traducido en la sección "Traducido" al final de la página.


## Agradecimientos

Gracias a [SiliconFlow](https://siliconflow.cn) por proporcionar el servicio de traducción gratuito para este proyecto.

<div align="right"> 
<h6><small>Parte del contenido de esta página ha sido traducido por GPT y puede contener errores.</small></h6>