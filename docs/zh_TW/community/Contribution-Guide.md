# 為專案貢獻

> [!CAUTION]
>
> 當前專案維護者正在研究自動化文檔國際化。因此，任何與文檔國際化/翻譯相關的 PR 將不被接受！
>
> 請勿提交與文檔國際化/翻譯相關的 PR！

感謝您對本專案的關注！在開始貢獻之前，請花些時間閱讀以下指南，以確保您的貢獻能夠順利被接受。

## 不接受的貢獻類型

1. 文件國際化/翻譯
2. 與核心基礎設施相關的貢獻，例如 HTTP API 等。
3. 明確標記為「無需幫助」的議題（包括 [Byaidu/PDFMathTranslate](Byaidu/PDFMathTranslate) 和 [PDFMathTranslate/PDFMathTranslate-next](PDFMathTranslate/PDFMathTranslate-next) 存儲庫中的議題）。
4. 其他被維護者認為不適當的貢獻。
5. 貢獻文件，但修改非英文的其他語言文件。
6. 需要修改 PDF 檔案的 PRs。

請勿提交與上述類型相關的 PR。

> [!NOTE]
>
> 若您想貢獻文檔，請**僅修改英文版本文檔**。其他語言版本由貢獻者自行翻譯。

## 貢獻流程

1. 複製此儲存庫並在本地克隆。
2. 創建一個新分支：`git checkout -b feature/<feature-name>`。
3. 開發並確保你的代碼符合要求。
4. 提交你的代碼：
   ```bash
   git add .
   git commit -m "<semantic commit message>"
   ```
5. 推送至你的儲存庫：`git push origin feature/<feature-name>`。
6. 在 GitHub 上創建一個 PR，提供詳細描述，並請求 [@awwaawwa](https://github.com/awwaawwa) 進行審查。
7. 確保所有自動化檢查通過。

> [!TIP]
>
> 您不需要等到開發完全完成才創建 PR。提前創建 PR 可以讓我們審查您的實現並提供建議。
>
> 如果您對源代碼或相關事宜有任何疑問，請聯繫維護者 aw@funstory.ai。
>
> 2.0 版本的資源文件與 [BabelDOC](https://github.com/funstory-ai/BabelDOC) 共享。下載相關資源的代碼位於 BabelDOC 中。如果您想新增資源文件，請聯繫 BabelDOC 維護者 aw@funstory.ai。

## 基本要求

<h4 id="sop">1. 工作流程</h4>

   - 請從 `main` 分支進行 fork，並在您 fork 的分支上進行開發。
   - 提交 Pull Request (PR) 時，請提供詳細的變更說明。
   - 如果您的 PR 未通過自動化檢查（顯示為 `checks failed` 和紅色叉號），請查看對應的 `details` 並修改您的提交，以確保新的 PR 通過所有檢查。


<h4 id="開發與測試">2. 開發與測試</h4>

   - 使用命令 `pip install -e .` 進行開發和測試。


<h4 id="格式">3. 代碼格式化</h4>

   - 配置 `pre-commit` 工具並啟用 `black` 和 `flake8` 進行代碼格式化。


<h4 id="requpdate">4. 依賴項更新</h4>

   - 如果您引入了新的依賴項，請及時更新 `pyproject.toml` 文件中的依賴列表。


<h4 id="docupdate">5. 文件更新</h4>

   - 如果您新增了命令行選項，請相應地更新所有語言版本的 `README.md` 文件中的命令行選項列表。


<h4 id="commitmsg">6. 提交訊息</h4>

   - 使用 [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)，例如：`feat(translator): add openai`。


<h4 id="codestyle">7. 程式碼風格</h4>

   - 確保您提交的代碼符合基本的編碼風格標準。
   - 變量命名請使用 snake_case 或 camelCase。


<h4 id="doctypo">8. 文件格式</h4>

   - 對於 `README.md` 的格式，請遵循 [中文文案排版指南](https://github.com/sparanoid/chinese-copywriting-guidelines)。
   - 確保英文和中文文檔始終保持最新；其他語言文檔的更新是可選的。

## 新增翻譯引擎

1. 在 `pdf2zh/config/translate_engine_model.py` 檔案中新增一個翻譯器配置類別。
2. 在相同檔案中，將新的翻譯器配置類別實例添加到 `TRANSLATION_ENGINE_SETTING_TYPE` 類型別名中。
3. 在 `pdf2zh/translator/translator_impl` 資料夾中新增翻譯器實作類別。

> [!NOTE]
>
> 本專案無意支援任何 RPS (每秒請求數) 低於 4 的翻譯引擎。請勿提交對此類引擎的支援。

## 專案結構

- **config 資料夾**：配置系統。
- **translator 資料夾**：與翻譯器相關的實現。
- **gui.py**：提供 GUI 介面。
- **const.py**：一些常數。
- **main.py**：提供命令行工具。
- **high_level.py**：基於 BabelDOC 的高階介面。
- **http_api.py**：提供 HTTP API（尚未啟動）。

## 聯絡我們

如果您有任何疑問，請透過 Issue 提交反饋或加入我們的 Telegram 群組。感謝您的貢獻！

> [!TIP]
>
> [Immersive Translate](https://immersivetranslate.com) 為本專案的活躍貢獻者提供每月 Pro 會員碼贊助。詳情請參閱：[BabelDOC/PDFMathTranslate 貢獻者獎勵規則](https://funstory-ai.github.io/BabelDOC/CONTRIBUTOR_REWARD/)

<div align="right"> 
<h6><small>Some content on this page has been translated by GPT and may contain errors.</small></h6>