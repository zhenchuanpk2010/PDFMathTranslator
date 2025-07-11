# 为项目做贡献

> [!CAUTION]
>
> 当前项目维护者正在研究文档自动化国际化方案，因此任何与文档国际化/翻译相关的 PR 将不被接受！
>
> 请勿提交与文档国际化/翻译相关的 PR！

感谢您对本项目的关注！在开始贡献之前，请花些时间阅读以下指南，以确保您的贡献能够顺利被接受。

## 不接受的贡献类型

1. 文档国际化/翻译相关贡献
2. 与核心基础设施相关的贡献，例如 HTTP API 等
3. 明确标记为"无需帮助"的问题（包括[Byaidu/PDFMathTranslate](Byaidu/PDFMathTranslate)和[PDFMathTranslate/PDFMathTranslate-next](PDFMathTranslate/PDFMathTranslate-next)仓库中的问题）
4. 维护者认为不合适的其他贡献
5. 贡献文档，但修改非英语版本的文档
6. 需要修改 PDF 文件的 PR

请勿提交与上述类型相关的 PR。

> [!NOTE]
>
> 如果你想贡献文档，请**仅修改文档的英文版本**。其他语言版本由贡献者自行翻译。

## 贡献流程

1. 首先 Fork 这个仓库并克隆到本地。
2. 创建一个新分支：`git checkout -b feature/<feature-name>`。
3. 进行开发并确保代码符合要求。
4. 提交代码：
   ```bash
   git add .
   git commit -m "<semantic commit message>"
   ```
5. 推送到你的仓库：`git push origin feature/<feature-name>`。
6. 在 GitHub 上创建 PR，提供详细描述，并请求 [@awwaawwa](https://github.com/awwaawwa) 进行审核。
7. 确保所有自动化检查通过。

> [!TIP]
>
> 您无需等待开发完全完成即可创建 PR。提前创建 PR 可以让我们审查您的实现并提供建议。
>
> 如果对源代码或相关事项有任何疑问，请联系维护者：aw@funstory.ai。
>
> 2.0 版本的资源文件与[BabelDOC](https://github.com/funstory-ai/BabelDOC)共享。下载相关资源的代码位于 BabelDOC 中。如需添加新的资源文件，请联系 BabelDOC 维护者：aw@funstory.ai。

## 基本要求

<h4 id="sop">1. 工作流程</h4>

- 请从 `main` 分支进行 fork，并在你 fork 的分支上进行开发。
   - 提交 Pull Request (PR) 时，请提供详细的变更说明。
   - 如果你的 PR 未通过自动化检查（显示为 `checks failed` 和红色叉号），请查看对应的 `details` 并修改提交内容，确保新 PR 能通过所有检查。


<h4 id="dev&test">2. 开发与测试</h4>

- 使用命令行 `pip install -e .` 进行开发和测试。


<h4 id="format">3. 代码格式化</h4>

- 配置 `pre-commit` 工具并启用 `black` 和 `flake8` 进行代码格式化。


<h4 id="requpdate">4. 依赖项更新</h4>

- 如果引入了新的依赖项，请及时更新 `pyproject.toml` 文件中的依赖列表。


<h4 id="docupdate">5. 文档更新</h4>

- 如果添加了新的命令行选项，请相应地在所有语言版本的 `README.md` 文件中更新命令行选项列表。


<h4 id="commitmsg">6. 提交信息</h4>

- 使用[约定式提交](https://www.conventionalcommits.org/en/v1.0.0/)，例如：`feat(translator): add openai`。


<h4 id="codestyle">7. 代码风格</h4>

- 确保提交的代码符合基本的编码风格标准。
   - 变量命名请使用 snake_case 或 camelCase 格式。


<h4 id="doctypo">8. 文档格式</h4>

- 对于 `README.md` 的格式，请遵循[中文文案排版指北](https://github.com/sparanoid/chinese-copywriting-guidelines)。
   - 确保英文和中文文档始终保持最新；其他语言文档的更新是可选的。

## 添加翻译引擎

1. 在 `pdf2zh/config/translate_engine_model.py` 文件中添加一个新的翻译器配置类。
2. 在同一文件的 `TRANSLATION_ENGINE_SETTING_TYPE` 类型别名中添加新翻译器配置类的实例。
3. 在 `pdf2zh/translator/translator_impl` 文件夹中添加新翻译器的实现类。

> [!NOTE]
>
> 本项目无意支持任何 RPS（每秒请求数）低于 4 的翻译引擎。请不要提交对此类引擎的支持。

## 项目结构

- **config folder**: 配置系统。
- **translator folder**: 翻译器相关实现。
- **gui.py**: 提供图形用户界面。
- **const.py**: 一些常量。
- **main.py**: 提供命令行工具。
- **high_level.py**: 基于 BabelDOC 的高级接口。
- **http_api.py**: 提供 HTTP API（未启动）。

## 联系我们

如有任何疑问，请通过 Issue 提交反馈或加入我们的 Telegram 群组。感谢您的贡献！

> [!TIP]
>
> [沉浸式翻译](https://immersivetranslate.com) 为本项目的活跃贡献者提供月度 Pro 会员码。详情请参阅：[BabelDOC/PDFMathTranslate 贡献者奖励规则](https://funstory-ai.github.io/BabelDOC/CONTRIBUTOR_REWARD/)

<div align="right"> 
<h6><small>本页面的部分内容由 GPT 翻译，可能包含错误。</small></h6>