<!-- CHUNK ID: chunk_53390D48  CHUNK TYPE: header START_LINE:1 -->
# Contributing to the Project

<!-- CHUNK ID: chunk_A71D833E  CHUNK TYPE: blockquote START_LINE:3 -->
> [!CAUTION]
>
> The current project maintainers are researching automated documentation internationalization. Therefore, any PRs related to documentation internationalization/translation will NOT be accepted!
>
> Please do NOT submit PRs related to documentation internationalization/translation!

<!-- CHUNK ID: chunk_D57757D9  CHUNK TYPE: paragraph START_LINE:9 -->
Thank you for your interest in this project! Before you start contributing, please take some time to read the following guidelines to ensure your contribution can be smoothly accepted.

<!-- CHUNK ID: chunk_FB836CBD  CHUNK TYPE: header START_LINE:11 -->
## Types of Contributions Not Accepted

<!-- CHUNK ID: chunk_F2331818  CHUNK TYPE: list START_LINE:13 -->
1. Documentation internationalization/translation
2. Contributions related to core infrastructure, such as HTTP API, etc.
3. Issues explicitly marked as "No help needed" (including issues in the [Byaidu/PDFMathTranslate](Byaidu/PDFMathTranslate) and the [PDFMathTranslate/PDFMathTranslate-next](PDFMathTranslate/PDFMathTranslate-next) repository).
4. Other contributions deemed inappropriate by the maintainers.
5. Contributing documentation, but changing the documentation in languages other than English.
6. PRs that require modifying PDF files.

<!-- CHUNK ID: chunk_7828B7C7  CHUNK TYPE: paragraph START_LINE:20 -->
Please do NOT submit PRs related to the above types.

<!-- CHUNK ID: chunk_56FADEC9  CHUNK TYPE: blockquote START_LINE:22 -->
> [!NOTE]
>
> If you want to contribute documentation, please **only modify the English version of the documentation**. Other language versions are translated by contributors themselves.

<!-- CHUNK ID: chunk_485712CB  CHUNK TYPE: header START_LINE:26 -->
## Contribution Process

<!-- CHUNK ID: chunk_4D698FBF  CHUNK TYPE: list START_LINE:28 -->
1. Fork this repository and clone it locally.
2. Create a new branch: `git checkout -b feature/<feature-name>`.
3. Develop and ensure your code meets the requirements.
4. Commit your code:
   ```bash
   git add .
   git commit -m "<semantic commit message>"
   ```
5. Push to your repository: `git push origin feature/<feature-name>`.
6. Create a PR on GitHub, provide a detailed description, and request a review from [@awwaawwa](https://github.com/awwaawwa).
7. Ensure all automated checks pass.

<!-- CHUNK ID: chunk_89A6F55A  CHUNK TYPE: blockquote START_LINE:40 -->
> [!TIP]
>
> You do not need to wait until your development is fully complete to create a PR. Creating one early allows us to review your implementation and provide suggestions.
>
> If you have any questions about the source code or related matters, please contact the maintainer at aw@funstory.ai.
>
> Resource files for version 2.0 are shared with [BabelDOC](https://github.com/funstory-ai/BabelDOC). The code for downloading related resources is in BabelDOC. If you want to add new resource files, please contact the BabelDOC maintainer at aw@funstory.ai.

<!-- CHUNK ID: chunk_E7638696  CHUNK TYPE: header START_LINE:48 -->
## Basic Requirements

<!-- CHUNK ID: chunk_4D251FB3  CHUNK TYPE: paragraph START_LINE:50 -->
<h4 id="sop">1. Workflow</h4>

<!-- CHUNK ID: chunk_8FDDA473  CHUNK TYPE: list START_LINE:52 -->
   - Please fork from the `main` branch and develop on your forked branch.
   - When submitting a Pull Request (PR), provide a detailed description of your changes.
   - If your PR does not pass automated checks (indicated by `checks failed` and a red cross), please review the corresponding `details` and modify your submission to ensure the new PR passes all checks.


<!-- CHUNK ID: chunk_19D447DF  CHUNK TYPE: paragraph START_LINE:57 -->
<h4 id="dev&test">2. Development and Testing</h4>

<!-- CHUNK ID: chunk_65AB8932  CHUNK TYPE: list START_LINE:59 -->
   - Use the command `pip install -e .` for development and testing.


<!-- CHUNK ID: chunk_B4865580  CHUNK TYPE: paragraph START_LINE:62 -->
<h4 id="format">3. Code Formatting</h4>

<!-- CHUNK ID: chunk_E8324FFA  CHUNK TYPE: list START_LINE:64 -->
   - Configure the `pre-commit` tool and enable `black` and `flake8` for code formatting.


<!-- CHUNK ID: chunk_7A584B10  CHUNK TYPE: paragraph START_LINE:67 -->
<h4 id="requpdate">4. Dependency Updates</h4>

<!-- CHUNK ID: chunk_BE2E8298  CHUNK TYPE: list START_LINE:69 -->
   - If you introduce new dependencies, please update the dependency list in the `pyproject.toml` file in a timely manner.


<!-- CHUNK ID: chunk_1615D8D8  CHUNK TYPE: paragraph START_LINE:72 -->
<h4 id="docupdate">5. Documentation Updates</h4>

<!-- CHUNK ID: chunk_725E4B8A  CHUNK TYPE: list START_LINE:74 -->
   - If you add new command-line options, please update the list of command-line options in all language versions of the `README.md` file accordingly.


<!-- CHUNK ID: chunk_09178615  CHUNK TYPE: paragraph START_LINE:77 -->
<h4 id="commitmsg">6. Commit Messages</h4>

<!-- CHUNK ID: chunk_8007BC97  CHUNK TYPE: list START_LINE:79 -->
   - Use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/), for example: `feat(translator): add openai`.


<!-- CHUNK ID: chunk_F5439516  CHUNK TYPE: paragraph START_LINE:82 -->
<h4 id="codestyle">7. Coding Style</h4>

<!-- CHUNK ID: chunk_22ECCE1D  CHUNK TYPE: list START_LINE:84 -->
   - Ensure your submitted code adheres to basic coding style standards.
   - Use either snake_case or camelCase for variable naming.


<!-- CHUNK ID: chunk_2F60B8EB  CHUNK TYPE: paragraph START_LINE:88 -->
<h4 id="doctypo">8. Documentation Formatting</h4>

<!-- CHUNK ID: chunk_320F91BE  CHUNK TYPE: list START_LINE:90 -->
   - For `README.md` formatting, please follow the [Chinese Copywriting Guidelines](https://github.com/sparanoid/chinese-copywriting-guidelines).
   - Ensure that both English and Chinese documentation are always up to date; other language documentation updates are optional.

<!-- CHUNK ID: chunk_126AF33C  CHUNK TYPE: header START_LINE:93 -->
## Adding a Translation Engine

<!-- CHUNK ID: chunk_38A36DFF  CHUNK TYPE: list START_LINE:95 -->
1. Add a new translator configuration class in the `pdf2zh/config/translate_engine_model.py` file.
2. Add an instance of the new translator configuration class to the `TRANSLATION_ENGINE_SETTING_TYPE` type alias in the same file.
3. Add the new translator implementation class in the `pdf2zh/translator/translator_impl` folder.

<!-- CHUNK ID: chunk_5B4684E1  CHUNK TYPE: blockquote START_LINE:99 -->
> [!NOTE]
>
> This project does not intend to support any translation engines with an RPS (requests per second) lower than 4. Please do not submit support for such engines.

<!-- CHUNK ID: chunk_7ED6230D  CHUNK TYPE: header START_LINE:103 -->
## Project Structure

<!-- CHUNK ID: chunk_9004E6A3  CHUNK TYPE: list START_LINE:105 -->
- **config folder**: Configuration system.
- **translator folder**: Translator-related implementations.
- **gui.py**: Provides the GUI interface.
- **const.py**: Some constants.
- **main.py**: Provides the command-line tool.
- **high_level.py**: High-level interfaces based on BabelDOC.
- **http_api.py**: Provides HTTP API (not started).

<!-- CHUNK ID: chunk_0C087ADF  CHUNK TYPE: header START_LINE:113 -->
## Contact Us

<!-- CHUNK ID: chunk_2FB8F835  CHUNK TYPE: paragraph START_LINE:115 -->
If you have any questions, please submit feedback via Issue or join our Telegram Group. Thank you for your contribution!

<!-- CHUNK ID: chunk_C2A414AC  CHUNK TYPE: blockquote START_LINE:117 -->
> [!TIP]
>
> [Immersive Translate](https://immersivetranslate.com) sponsors monthly Pro membership codes for active contributors to this project. For details, please see: [BabelDOC/PDFMathTranslate Contributor Reward Rules](https://funstory-ai.github.io/BabelDOC/CONTRIBUTOR_REWARD/)