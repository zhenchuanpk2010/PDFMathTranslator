[**Расширенные параметры**](./introduction.md) > **Расширенные параметры** _(current)_

---

<h3 id="toc">Содержание</h3>

- [Аргументы командной строки](#аргументы-командной-строки)
- [Частичный перевод](#частичный-перевод)
- [Указание исходного и целевого языков](#указание-исходного-и-целевого-языков)
- [Перевод с исключениями](#перевод-с-исключениями)
- [Пользовательский запрос](#пользовательский-запрос)
- [Пользовательская конфигурация](#пользовательская-конфигурация)
- [Пропустить очистку](#пропустить-очистку)
- [Кэш перевода](#кэш-перевода)
- [Развертывание в качестве публичного сервиса](#развертывание-в-качестве-публичного-сервиса)
- [Аутентификация и приветственная страница](#аутентификация-и-приветственная-страница)
- [Поддержка глоссария](#поддержка-глоссария)

---

#### Аргументы командной строки

Выполните команду перевода в командной строке, чтобы сгенерировать переведенный документ `example-mono.pdf` и двуязычный документ `example-dual.pdf` в текущей рабочей директории. По умолчанию используется сервис перевода Google. Дополнительные поддерживаемые сервисы перевода можно найти [ЗДЕСЬ](https://github.com/PDFMathTranslate/PDFMathTranslate-next/blob/main/docs/ADVANCED.md#services).

<img src="./../images/cmd_light.svg" width="580px"  alt="cmd"/>

В следующей таблице мы приводим все расширенные параметры для справки:

##### Аргументы

| Опция                          | Функция                                                                               | Пример                                                                                                              |
| ------------------------------- | -------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- |
| `files`                         | Локальный путь к PDF файлу                                                                    | `pdf2zh ~/local.pdf`                                                                                                 |
| `links`                         | Онлайн-файлы                                                                           | `pdf2zh http://arxiv.org/paper.pdf`                                                                                  |
| `--output`                      | Выходная директория для файлов                                                         | `pdf2zh example.pdf --output /outputpath`                                                                            |
| `--<Services>`                  | Использовать [**определенный сервис**](./Документация-служб-перевода.md) для перевода | `pdf2zh example.pdf --openai`<br>`pdf2zh example.pdf --deepseek`                                                     |
| `--help`, `-h`                  | Показать сообщение справки и выйти                                                     | `pdf2zh -h`                                                                                                          |
| `--config-file`                 | Путь к файлу конфигурации                                                         | `pdf2zh --config-file /path/to/config/config.toml`                                                                   |
| `--report-interval`             | Интервал отчета о прогрессе в секундах                                                    | `pdf2zh example.pdf --report-interval 5`                                                                             |
| `--debug`                       | Использовать уровень логирования для отладки                                                                | `pdf2zh example.pdf --debug`                                                                                         |
| `--gui`                         | Взаимодействие с GUI                                                                      | `pdf2zh --gui`                                                                                                       |
| `--warmup`                      | Только загрузить и проверить необходимые ресурсы, затем выйти                                     | `pdf2zh example.pdf --warmup`                                                                                        |
| `--generate-offline-assets`     | Создать пакет оффлайн-ресурсов в указанной директории                             | `pdf2zh example.pdf --generate-offline-assets /path`                                                                 |
| `--restore-offline-assets`      | Восстановить пакет оффлайн-ресурсов из указанной директории                            | `pdf2zh example.pdf --restore-offline-assets /path`                                                                  |
| `--version`                     | Показать версию и выйти                                                                 | `pdf2zh --version`                                                                                                   |
| `--pages`                       | Частичный перевод документа                                                           | `pdf2zh example.pdf --pages 1,2,1-,-3,3-5`                                                                           |
| `--lang-in`                     | Код исходного языка                                                            | `pdf2zh example.pdf --lang-in en`                                                                                    |
| `--lang-out`                    | Код целевого языка                                                            | `pdf2zh example.pdf --lang-out zh-CN`                                                                                |
| `--min-text-length`             | Минимальная длина текста для перевода                                                  | `pdf2zh example.pdf --min-text-length 5`                                                                             |
| `--rpc-doclayout`               | Адрес хоста RPC-сервиса для анализа структуры документа                                  |                                                                                                                      |
| `--qps`                         | Ограничение QPS для службы перевода                                                      | `pdf2zh example.pdf --qps 200`                                                                                       |
| `--ignore-cache`                | Игнорировать кэш перевода                                                               | `pdf2zh example.pdf --ignore-cache`                                                                                  |
| `--custom-system-prompt`        | Пользовательский системный запрос для перевода. Используется для `/no_think` в Qwen 3                   | `pdf2zh example.pdf --custom-system-prompt "/no_think You are a professional, authentic machine translation engine"` |
| `--pool-max-worker`             | Максимальное количество воркеров для пула перевода. Если не задано, будет использоваться qps в качестве количества воркеров | `pdf2zh example.pdf --pool-max-worker 100`                                                                |
| `--no-auto-extract-glossary`    | Отключить автоматическое извлечение глоссария                                          | `pdf2zh example.pdf --no-auto-extract-glossary`                                                                      |
| `--primary-font-family`         | Переопределение основного семейства шрифтов для переведенного текста. Варианты: 'serif' для шрифтов с засечками, 'sans-serif' для рубленых шрифтов, 'script' для курсивных/рукописных шрифтов. Если не указано, используется автоматический выбор шрифта на основе свойств исходного текста. | `pdf2zh example.pdf --primary-font-family serif` |
| `--no-dual`                     | Не выводить двуязычные PDF-файлы                                                      | `pdf2zh example.pdf --no-dual`                                                                                       |
| `--no-mono`                     | Не выводить одностраничные PDF-файлы                                                    | `pdf2zh example.pdf --no-mono`                                                                                       |
| `--formular-font-pattern`       | Шаблон шрифта для идентификации текста формул                                                  | `pdf2zh example.pdf --formular-font-pattern "(MS.*)"`                                                                |
| `--formular-char-pattern`       | Шаблон символов для идентификации текста формул                                             | `pdf2zh example.pdf --formular-char-pattern "(MS.*)"`                                                                |
| `--split-short-line`            | Принудительное разделение коротких строк на разные абзацы                                       | `pdf2zh example.pdf --split-short-line`                                                                              |
| `--short-line-split-factor`     | Коэффициент порога разделения для коротких строк                                       |                                                                                                                      |
| `--skip-clean`                  | Пропустить этап очистки PDF                                                                 | `pdf2zh example.pdf --skip-clean`                                                                                    |
| `--dual-translate-first`        | В режиме двойного PDF приоритетно размещать переведенную страницу      | `pdf2zh example.pdf --dual-translate-first`                                                                                            |
| `--disable-rich-text-translate` | Отключить перевод форматированного текста                                              | `pdf2zh example.pdf --disable-rich-text-translate`                                                                   |
| `--enhance-compatibility`       | Включить все опции повышения совместимости                                           | `pdf2zh example.pdf --enhance-compatibility`                                                                         |
| `--use-alternating-pages-dual`  | Использовать режим чередующихся страниц для двойного PDF                                                | `pdf2zh example.pdf --use-alternating-pages-dual`                                                                    |
| `--watermark-output-mode`       | Режим вывода водяных знаков для PDF-файлов                                             | `pdf2zh example.pdf --watermark-output-mode "NoWaterMark"`                                                           |
| `--max-pages-per-part`          | Максимальное количество страниц на часть для раздельного перевода                      | `pdf2zh example.pdf --max-pages-per-part 1`                                                                          |
| `--translate-table-text`        | Перевод текста таблицы (экспериментальная функция)                                                    | `pdf2zh example.pdf --translate-table-text`                                                                          |
| `--skip-scanned-detection`      | Пропустить обнаружение сканированных документов                                        | `pdf2zh example.pdf --skip-scanned-detection`                                                                        |
| `--ocr-workaround`              | Принудительно делает переведенный текст черным и добавляет белый фон                   | `pdf2zh example.pdf --ocr-workaround`                                                                                |
| `--auto-enable-ocr-workaround`  | Включить автоматическое обходное решение для OCR. Если документ определяется как сильно отсканированный, будет предпринята попытка включить обработку OCR и пропустить дальнейшее обнаружение сканирования. Подробности см. в документации. (по умолчанию: False) | `pdf2zh example.pdf --auto-enable-ocr-workaround True`                    |
| `--only-include-translated-page`| Включать в выходной PDF только переведенные страницы. Эффективно только при использовании --pages. | `pdf2zh example.pdf --pages 1-5 --only-include-translated-page`                                                       |
| `--glossaries`                  | Пользовательский глоссарий для перевода.                                              | `pdf2zh example.pdf --glossaries "glossary1.csv,glossary2.csv,glossary3.csv"`                                         |
| `--save-auto-extracted-glossary`| сохранить автоматически извлеченный глоссарий.                                                | `pdf2zh example.pdf --save-auto-extracted-glossary`                                                                   |


##### Аргументы GUI

| Опция                          | Функция                               | Пример                                         |
| ------------------------------- | -------------------------------------- | ----------------------------------------------- |
| `--share`                       | Включить режим общего доступа         | `pdf2zh --gui --share`                          |
| `--auth-file`                   | Путь к файлу аутентификации        | `pdf2zh --gui --auth-file /path`                |
| `--welcome-page`                | Путь к приветственному html-файлу      | `pdf2zh --gui --welcome-page /path`             |
| `--enabled-services`            | Включенные службы перевода           | `pdf2zh --gui --enabled-services "Bing,OpenAI"` |
| `--disable-gui-sensitive-input` | Отключить чувствительный ввод в GUI    | `pdf2zh --gui --disable-gui-sensitive-input`    |
| `--disable-config-auto-save`    | Отключить автоматическое сохранение конфигурации | `pdf2zh --gui --disable-config-auto-save`       |
| `--server-port`                 | Порт WebUI                             | `pdf2zh --gui --server-port 7860`               |

[⬆️ Наверх](#toc)

---

#### Частичный перевод

Используйте параметр `--pages` для перевода части документа.

- Если номера страниц идут подряд, можно записать это так:

```bash
pdf2zh_next example.pdf --pages 1-3
```

```bash
pdf2zh_next example.pdf --pages 25-
```

> [!TIP]
> `25-` включает все страницы после 25-й. Если ваш документ содержит 100 страниц, это эквивалентно `25-100`.
> 
> Аналогично, `-25` включает все страницы до 25-й, что эквивалентно `1-25`.

- Если страницы не идут подряд, можно использовать запятую `,` для их разделения.

Например, если вы хотите перевести первую и третью страницы, вы можете использовать следующую команду:

```bash
pdf2zh_next example.pdf --pages "1,3"
```

- Если страницы включают как последовательные, так и непоследовательные диапазоны, вы также можете соединить их запятой, например:

```bash
pdf2zh_next example.pdf --pages "1,3,10-20,25-"
```

Эта команда переведет первую страницу, третью страницу, страницы с 10 по 20 и все страницы с 25 до конца.


[⬆️ Наверх](#toc)

---

#### Указание исходного и целевого языков

См. [Коды языков Google](https://developers.google.com/admin-sdk/directory/v1/languages), [Коды языков DeepL](https://developers.deepl.com/docs/resources/supported-languages)

```bash
pdf2zh_next example.pdf --lang-in en -lang-out ja
```

[⬆️ Наверх](#toc)

---

#### Перевод с исключениями

Используйте регулярные выражения для указания шрифтов формул и символов, которые необходимо сохранить:

```bash
pdf2zh_next example.pdf --formular-font-pattern "(CM[^RT].*|MS.*|.*Ital)" --formular-char-pattern "(\(|\||\)|\+|=|\d|[\u0080-\ufaff])"
```

Сохранять шрифты `Latex`, `Mono`, `Code`, `Italic`, `Symbol` и `Math` по умолчанию:

```bash
pdf2zh_next example.pdf --formular-font-pattern "(CM[^R]|MS.M|XY|MT|BL|RM|EU|LA|RS|LINE|LCIRCLE|TeX-|rsfs|txsy|wasy|stmary|.*Mono|.*Code|.*Ital|.*Sym|.*Math)"
```

[⬆️ Наверх](#toc)

---

#### Пользовательский запрос

<!-- Note: System prompt is currently not supported. See [this change](https://github.com/PDFMathTranslate/PDFMathTranslate-next/pull/637). -->

Пользовательский системный запрос для перевода. В основном используется для добавления инструкции '/no_think' Qwen 3 в запрос.

```bash
pdf2zh_next example.pdf --custom-system-prompt "/no_think You are a professional and reliable machine translation engine responsible for translating the input text into zh_CN.When translating, strictly follow the instructions below to ensure translation quality and preserve all formatting, tags, and placeholders:"
```

[⬆️ Наверх](#toc)

---

#### Пользовательская конфигурация

Существует несколько способов изменения и импорта файла конфигурации.

> [!NOTE]
> **Иерархия файлов конфигурации**
>
> При изменении одного и того же параметра разными способами, программное обеспечение будет применять изменения в соответствии с указанным ниже порядком приоритетов.
>
> Изменения с более высоким приоритетом переопределяют изменения с более низким приоритетом.
>
> **cli/gui > env > пользовательский файл конфигурации > файл конфигурации по умолчанию**

- Изменение конфигурации через **Аргументы командной строки**

В большинстве случаев вы можете напрямую передать желаемые настройки через аргументы командной строки. Подробнее см. в разделе [Аргументы командной строки](#cmd).

Например, если вы хотите включить окно GUI, вы можете использовать следующую команду:

```bash
pdf2zh_next --gui
```

- Изменение конфигурации через **переменные окружения**

Вы можете заменить `--` в аргументах командной строки на `PDF2ZH_`, соединить параметры с помощью `=` и заменить `-` на `_` в качестве переменных окружения.

Например, если вы хотите включить окно GUI, вы можете использовать следующую команду:

```bash
PDF2ZH_GUI=TRUE pdf2zh_next
```

<img src="./../images/ev_light.svg" width="580px"  alt="env"/>

- Пользовательский **Файл конфигурации**

Вы можете указать файл конфигурации, используя следующий аргумент командной строки:

```bash
pdf2zh_next --config-file '/path/config.toml'
```

Если вы не уверены в формате файла конфигурации, обратитесь к стандартному файлу конфигурации, описанному ниже.

- **Конфигурация по умолчанию**

Файл конфигурации по умолчанию находится в `~/.config/pdf2zh`. 
Пожалуйста, не изменяйте файлы конфигурации в каталоге `default`. 
Настоятельно рекомендуется ознакомиться с содержимым этого файла конфигурации и использовать **Пользовательскую конфигурацию** для реализации собственного файла конфигурации.

> [!TIP]
> - По умолчанию pdf2zh 2.0 автоматически сохраняет текущую конфигурацию в файл `~/.config/pdf2zh/config.v3.toml` каждый раз, когда вы нажимаете кнопку перевода в GUI. Этот файл конфигурации будет загружен по умолчанию при следующем запуске.
> - Файлы конфигурации в директории `default` автоматически генерируются программой. Вы можете скопировать их для модификации, но пожалуйста, не изменяйте их напрямую.
> - Файлы конфигурации могут включать версионные номера, такие как "v2", "v3" и т.д. Это **версии файлов конфигурации**, а **не** версия самого pdf2zh.


[⬆️ Наверх](#toc)

---

#### Пропустить очистку

Когда этот параметр установлен в True, шаг очистки PDF будет пропущен, что может улучшить совместимость и избежать некоторых проблем с обработкой шрифтов.

Использование:

```bash
pdf2zh_next example.pdf --skip-clean
```

Или использование переменных окружения:

```bash
PDF2ZH_SKIP_CLEAN=TRUE pdf2zh_next example.pdf
```

> [!TIP]
> Когда включен параметр `--enhance-compatibility`, функция Пропустить очистку активируется автоматически.

---

#### Кэш перевода

PDFMathTranslate кэширует переведенные тексты для увеличения скорости и избежания ненужных вызовов API для одинакового содержимого. Вы можете использовать опцию `--ignore-cache`, чтобы игнорировать кэш перевода и принудительно выполнить повторный перевод.

```bash
pdf2zh_next example.pdf --ignore-cache
```

[⬆️ Наверх](#toc)

---

#### Развертывание в качестве публичного сервиса

При развертывании pdf2zh GUI в публичных сервисах следует изменить файл конфигурации, как описано ниже.

> [!TIP]
> - При публичном развертывании следует включить оба параметра `disable_gui_sensitive_input` и `disable_config_auto_save`.
> - Разделяйте различные доступные сервисы *английскими запятыми* <kbd>,</kbd> .

Используемая конфигурация выглядит следующим образом:

```toml title="config.toml"
[basic]
gui = true

[gui_settings]
enabled_services = "Bing,OpenAI"
disable_gui_sensitive_input = true
disable_config_auto_save = true
```

[⬆️ Наверх](#toc)

---

#### Аутентификация и приветственная страница

При использовании Аутентификация и приветственная страница для указания, какой пользователь должен использовать Web UI и настройки страницы входа:

пример auth.txt
Каждая строка содержит два элемента: имя пользователя и пароль, разделенные запятой.

```
admin,123456
user1,password1
user2,abc123
guest,guest123
test,test123
```

example welcome.html

```html
<!DOCTYPE html>
<html>
<head>
    <title>Simple HTML</title>
</head>
<body>
    <h1>Hello, World!</h1>
    <p>Welcome to my simple HTML page.</p>
</body>
</html>
```

> [!NOTE]
> приветственная страница будет работать, только если файл аутентификации не пуст.
> Если файл аутентификации пуст, аутентификация не будет выполняться. :)

Используемая конфигурация выглядит следующим образом:

```toml title="config.toml"
[basic]
gui = true

[gui_settings]
auth_file = "/path/to/auth/file"
welcome_page = "/path/to/welcome/html/file"
```

[⬆️ Наверх](#toc)

---

#### Поддержка глоссария

PDFMathTranslate поддерживает таблицу глоссария. Файл таблицы глоссария должен быть в формате `csv`.
В файле три столбца. Вот демонстрационный файл глоссария:

| source | target  | tgt_lng |
|--------|---------|---------|
| AutoML | 自动 ML  | zh-CN   |
| a,a    | a       | zh-CN   |
| "      | "       | zh-CN   |


Для пользователей командной строки:
Вы можете использовать несколько файлов для глоссария. Разные файлы должны быть разделены запятыми `,`.

```bash
pdf2zh_next example.pdf --glossaries "glossary1.csv,glossary2.csv,glossary3.csv"
```

Для пользователей WebUI:

Теперь вы можете загрузить собственный файл глоссария. После загрузки файла вы можете проверить его содержимое, нажав на его имя, и содержимое отобразится ниже.

[⬆️ Наверх](#toc)

<div align="right"> 
<h6><small>Часть содержимого этой страницы была переведена GPT и может содержать ошибки.</small></h6>