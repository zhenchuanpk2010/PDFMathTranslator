<div align="center">

<img src="./docs/images/banner.png" width="320px"  alt="banner"/>

<h2 id="title">PDFMathTranslate</h2>

<p>

<!-- PyPI -->
  <a href="https://pypi.org/project/pdf2zh-next/">
    <img src="https://img.shields.io/pypi/v/pdf2zh-next"></a>
  <a href="https://pepy.tech/projects/pdf2zh-next">
    <img src="https://static.pepy.tech/badge/pdf2zh-next"></a>
  <a href="https://hub.docker.com/repository/docker/awwaawwa/pdfmathtranslate-next/tags">
    <img src="https://img.shields.io/docker/pulls/awwaawwa/pdfmathtranslate-next"></a>
  <a href="https://hellogithub.com/repository/8ec2cfd3ef744762bf531232fa32bc47" target="_blank"><img src="https://api.hellogithub.com/v1/widgets/recommend.svg?rid=8ec2cfd3ef744762bf531232fa32bc47&claim_uid=JQ0yfeBNjaTuqDU&theme=small" alt="Рекомендуется｜HelloGitHub" /></a>


<a href="https://t.me/+Z9_SgnxmsmA5NzBl">
    <img src="https://img.shields.io/badge/Telegram-2CA5E0?style=flat-squeare&logo=telegram&logoColor=white"></a>

<!-- Лицензия -->
  <a href="./LICENSE">
    <img src="https://img.shields.io/github/license/PDFMathTranslate/PDFMathTranslate-next"></a>
</p>

<a href="https://trendshift.io/repositories/12424" target="_blank"><img src="https://trendshift.io/api/badge/repositories/12424" alt="Byaidu%2FPDFMathTranslate | Trendshift" style="width: 250px; height: 55px;" width="250" height="55"/></a>

</div>

Перевод научных статей в формате PDF с двуязычным сравнением.

- 📊 Сохранение формул, графиков, оглавления и аннотаций _([предпросмотр](#предпросмотр))_.
- 🌐 Поддержка [множества языков](https://pdf2zh-next.com/supported_languages.html) и различных [служб перевода](https://pdf2zh-next.com/advanced/Документация-служб-перевода.html).
- 🤖 Предоставляет [инструмент командной строки](https://pdf2zh-next.com/Начало-работы/Использование-командной-строки.html), [интерактивный пользовательский интерфейс](https://pdf2zh-next.com/Начало-работы/Использование-веб-интерфейса.html) и [Docker](https://pdf2zh-next.com/Начало-работы/Установка-Docker.html)

Оставляйте отзывы в [GitHub Issues](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues) или [Telegram Group](https://t.me/+Z9_SgnxmsmA5NzBl).

Подробности о том, как внести вклад, можно найти в [Руководстве по участию](https://pdf2zh-next.com/сообщество/Руководство-по-участию.html).

<h2 id="обновления">Обновления</h2>

- [4 июня 2025] Проект переименован и перемещен в [PDFMathTranslate/PDFMathTranslate-next](https://github.com/PDFMathTranslate/PDFMathTranslate-next) (от [@awwaawwa](https://github.com/awwaawwa))
- [3 марта 2025] Экспериментальная поддержка нового бэкенда [BabelDOC](https://github.com/funstory-ai/BabelDOC) WebUI добавлена как экспериментальная опция (от [@awwaawwa](https://github.com/awwaawwa))
- [22 февраля 2025] Улучшенный CI для релизов и хорошо упакованный windows-amd64 exe (от [@awwaawwa](https://github.com/awwaawwa))
- [24 декабря 2024] Переводчик теперь поддерживает локальные модели на [Xinference](https://github.com/xorbitsai/inference) _(от [@imClumsyPanda](https://github.com/imClumsyPanda))_
- [19 декабря 2024] Теперь поддерживаются документы не в формате PDF/A с использованием `-cp` _(от [@reycn](https://github.com/reycn))_
- [13 декабря 2024] Дополнительная поддержка бэкенда от _(от [@YadominJinta](https://github.com/YadominJinta))_
- [10 декабря 2024] Переводчик теперь поддерживает модели OpenAI на Azure _(от [@yidasanqian](https://github.com/yidasanqian))_

<h2 id="предпросмотр">Предпросмотр</h2>

<div align="center">
<!-- <img src="./docs/images/preview.gif" width="80%"  alt="preview"/> -->


<img src="https://s.immersivetranslate.com/assets/r2-uploads/images/babeldoc-preview.png" width="80%"/>
</div>

<h2 id="demo">Онлайн-сервис 🌟</h2>

> [!NOTE]
>
> pdf2zh 2.0 в настоящее время не предоставляет онлайн-демонстрацию

Вы можете попробовать наше приложение, используя любую из следующих демонстрационных версий:

- [v1.x Бесплатный публичный сервис](https://pdf2zh.com/) онлайн без установки _(рекомендуется)_.
- [Immersive Translate - BabelDOC](https://app.immersivetranslate.com/babel-doc/) 1000 бесплатных страниц в месяц. _(рекомендуется)_

<!-- - [Демо на HuggingFace](https://huggingface.co/spaces/reycn/PDFMathTranslate-Docker)
- [Демо на ModelScope](https://www.modelscope.cn/studios/AI-ModelScope/PDFMathTranslate) без установки. -->

Обратите внимание, что вычислительные ресурсы демонстрационной версии ограничены, поэтому, пожалуйста, избегайте их злоупотребления.

<h2 id="install">Установка и Использование</h2>

### Установка

1. [**Windows EXE**](https://pdf2zh-next.com/getting-started/INSTALLATION_winexe.html) <small>Рекомендуется для Windows</small>
2. [**Docker**](https://pdf2zh-next.com/getting-started/INSTALLATION_docker.html) <small>Рекомендуется для Linux</small>
3. [**uv** (менеджер пакетов Python)](https://pdf2zh-next.com/getting-started/INSTALLATION_uv.html) <small>Рекомендуется для macOS</small>

---

### Использование

1. [Использование **WebUI**](https://pdf2zh-next.com/getting-started/USAGE_webui.html)  
2. [Использование **плагина Zotero**](https://github.com/guaguastandup/zotero-pdf2zh) (Сторонняя программа)  
3. [Использование **Командной строки**](https://pdf2zh-next.com/getting-started/USAGE_commandline.html)  

Для различных сценариев использования мы предоставляем разные методы работы с нашей программой. Подробнее см. на [этой странице](./getting-started/getting-started.md).  

<h2 id="usage">Расширенные параметры</h2>  

Подробные объяснения см. в нашей документации по [Расширенному использованию](https://pdf2zh-next.com/advanced/advanced.html) для полного списка доступных опций.  

<h2 id="downstream">Дополнительная разработка (API)</h2>

> [!NOTE]
>
> В настоящее время соответствующая документация не предоставлена. Она будет дополнена позже. Пожалуйста, ожидайте терпеливо.

<!-- Для последующих приложений, пожалуйста, обратитесь к нашей документации о [Детали API](./docs/APIS.md) для получения дополнительной информации о:

- [Python API](./docs/APIS.md#api-python), как использовать программу в других программах на Python
- [HTTP API](./docs/APIS.md#api-http), как взаимодействовать с сервером, на котором установлена программа -->

<h2 id="langcode">Код языка</h2>

Если вы не знаете, какой код использовать для перевода на нужный вам язык, ознакомьтесь с [этой документацией](https://pdf2zh-next.com/advanced/Language-Codes.html)

<!-- 
<h2 id="todo">TODO</h2>

- [ ] Разбор макета с помощью моделей на основе DocLayNet, [PaddleX](https://github.com/PaddlePaddle/PaddleX/blob/17cc27ac3842e7880ca4aad92358d3ef8555429a/paddlex/repo_apis/PaddleDetection_api/object_det/official_categories.py#L81), [PaperMage](https://github.com/allenai/papermage/blob/9cd4bb48cbedab45d0f7a455711438f1632abebe/README.md?plain=1#L102), [SAM2](https://github.com/facebookresearch/sam2)

- [ ] Исправить поворот страниц, оглавление, формат списков

- [ ] Исправить пиксельные формулы в старых статьях

- [ ] Асинхронная повторная попытка, кроме KeyboardInterrupt

- [ ] Алгоритм Кнута–Пласса для западных языков

- [ ] Поддержка файлов, не соответствующих PDF/A

- [ ] Плагины для [Zotero](https://github.com/zotero/zotero) и [Obsidian](https://github.com/obsidianmd/obsidian-releases) -->

<h2 id="благодарности">Благодарности</h2>

- [Immersive Translation](https://immersivetranslate.com) ежемесячно предоставляет коды для активации Pro-подписки активным участникам этого проекта. Подробности см. в: [CONTRIBUTOR_REWARD.md](https://github.com/funstory-ai/BabelDOC/blob/main/docs/CONTRIBUTOR_REWARD.md)

- Версия 1.x: [Byaidu/PDFMathTranslate](https://github.com/Byaidu/PDFMathTranslate)

- Новый бэкенд: [BabelDOC](https://github.com/funstory-ai/BabelDOC)

- Объединение документов: [PyMuPDF](https://github.com/pymupdf/PyMuPDF)

- Парсинг документов: [Pdfminer.six](https://github.com/pdfminer/pdfminer.six)

- Извлечение документов: [MinerU](https://github.com/opendatalab/MinerU)

- Просмотр документов: [Gradio PDF](https://github.com/freddyaboulton/gradio-pdf)

- Многопоточный перевод: [MathTranslate](https://github.com/SUSYUSTC/MathTranslate)

- Анализ макета: [DocLayout-YOLO](https://github.com/opendatalab/DocLayout-YOLO)

- Стандарт документов: [PDF Explained](https://zxyle.github.io/PDF-Explained/), [PDF Cheat Sheets](https://pdfa.org/resource/pdf-cheat-sheets/)

- Многоязычные шрифты: [Go Noto Universal](https://github.com/satbyy/go-noto-universal)

- [Asynchronize](https://github.com/multimeric/Asynchronize/tree/master?tab=readme-ov-file)

- [Расширенное логирование с многопроцессорностью](https://github.com/SebastianGrans/Rich-multiprocess-logging/tree/main)

<h2 id="conduct">Перед отправкой кода</h2>

Мы приветствуем активное участие участников, чтобы сделать pdf2zh лучше. Прежде чем отправить свой код, ознакомьтесь с нашим [Кодексом поведения](https://pdf2zh-next.com/community/CODE_OF_CONDUCT.html) и [Руководством по вкладу](https://pdf2zh-next.com/community/Contribution-Guide.html).

<h2 id="contrib">Участники</h2>

<a href="https://github.com/PDFMathTranslate/PDFMathTranslate-next/graphs/contributors">
  <img src="https://opencollective.com/PDFMathTranslate/contributors.svg?width=890&button=false" />
</a>

![Alt](https://repobeats.axiom.co/api/embed/45529651750579e099960950f757449a410477ad.svg "Repobeats analytics image")

<h2 id="star_hist">История звезд</h2>

<a href="https://star-history.com/#PDFMathTranslate/PDFMathTranslate-next&Date">
 <picture>
   <source media="(prefers-color-scheme: dark)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date&theme=dark" />
   <source media="(prefers-color-scheme: light)" srcset="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date" />
   <img alt="График истории звезд" src="https://api.star-history.com/svg?repos=PDFMathTranslate/PDFMathTranslate-next&type=Date"/>
 </picture>
</a>

<div align="right"> 
<h6><small>Часть содержимого этой страницы была переведена GPT и может содержать ошибки.</small></h6>