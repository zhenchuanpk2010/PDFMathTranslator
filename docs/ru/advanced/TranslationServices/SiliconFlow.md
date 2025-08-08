# SiliconFlow

## Бесплатный сервис перевода

[SiliconFlow](https://siliconflow.cn) предоставляет бесплатный сервис перевода для этого проекта.

В настоящее время бесплатный сервис перевода будет использовать модель `THUDM/GLM-4-9B-0414`.

### Использование

#### Командная строка

```bash
pdf2zh_next --siliconflowfree example.pdf 
```

#### webui

1. Выберите "SiliconFlowFree" из выпадающего списка "Translation Options" - "Service".
2. Нажмите кнопку "Translate" в нижней части страницы, чтобы начать перевод.
3. После завершения перевода вы можете найти переведённый файл PDF в разделе "Translated" в нижней части страницы.


### Политика конфиденциальности

Содержание файла будет отправлено на сервер сопровождающего проекта [@awwaawwa](https://github.com/awwaawwa), а затем перенаправлено в SiliconFlow для перевода.

Сопровождающие этого проекта будут собирать только информацию об ошибках, возвращаемую SiliconFlow, для отладки связанных сервисов. Содержание вашего файла не будет собираться.

Политика конфиденциальности SiliconFlow: [简体中文](https://docs.siliconflow.cn/cn/legals/privacy-policy)/[English](https://docs.siliconflow.cn/en/legals/privacy-policy)



## Использование других моделей от SiliconFlow

[SiliconFlow](https://siliconflow.cn) также предоставляет другие модели для перевода.

### Использование

1. Зарегистрируйте аккаунт на [SiliconFlow](https://siliconflow.cn)

2. Создайте API-ключ на странице [SiliconFlow API Key](https://cloud.siliconflow.cn/me/account/ak). Затем нажмите на ключ, чтобы скопировать его.

#### Командная строка

```bash
pdf2zh_next --siliconflow --siliconflow-model "Pro/deepseek-ai/DeepSeek-V3" --siliconflow-api-key <your-api-key> example.pdf
```

#### webui

1. "Параметры перевода" - выпадающий список **"Сервис"**: Выберите "SiliconFlow"  
2. "Параметры перевода" - **"Базовый URL для API SiliconFlow"**: Оставьте значение по умолчанию  
3. "Параметры перевода" - **"Модель SiliconFlow для использования"**: Введите "Pro/deepseek-ai/DeepSeek-V3" или другие модели  
4. "Параметры перевода" - **"API-ключ для сервиса SiliconFlow"**: Вставьте ваш API-ключ  
5. Нажмите кнопку "Перевести" в нижней части страницы, чтобы начать перевод  
6. После завершения перевода вы можете найти переведенный `PDF` файл в разделе "Translated" внизу страницы.


## Благодарности

Спасибо [SiliconFlow](https://siliconflow.cn) за предоставление бесплатного сервиса перевода для этого проекта.

<div align="right"> 
<h6><small>Часть содержимого этой страницы была переведена GPT и может содержать ошибки.</small></h6>