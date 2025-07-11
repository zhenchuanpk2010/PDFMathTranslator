# プロジェクトへの貢献

> [!CAUTION]
>
> 現在のプロジェクトメンテナーは、ドキュメントの自動国際化を研究中です。そのため、ドキュメントの国際化/翻訳に関連する PR は受け付けられません！
>
> ドキュメントの国際化/翻訳に関連する PR を提出しないでください！

このプロジェクトに興味を持っていただきありがとうございます！貢献を始める前に、以下のガイドラインを読んで、あなたの貢献がスムーズに受け入れられるようにしてください。

## 受け付けない貢献の種類

1. ドキュメントの国際化/翻訳
2. HTTP API などのコアインフラストラクチャに関する貢献
3. 「No help needed」と明示的にマークされた Issue（[Byaidu/PDFMathTranslate](Byaidu/PDFMathTranslate)および[PDFMathTranslate/PDFMathTranslate-next](PDFMathTranslate/PDFMathTranslate-next)リポジトリの Issue を含む）。
4. メンテナーが不適切と判断したその他の貢献。
5. 貢献ドキュメント、ただし英語以外の言語でのドキュメント変更。
6. PDF ファイルの修正を必要とする PR。

上記の種類に関連する PR は提出しないでください。

> [!NOTE]
>
> ドキュメントに貢献したい場合は、**ドキュメントの英語版のみを修正してください**。他の言語バージョンは貢献者自身によって翻訳されています。

## 貢献プロセス

1. このリポジトリをフォークし、ローカルにクローンします。
2. 新しいブランチを作成：`git checkout -b feature/<feature-name>`.
3. 開発を行い、コードが要件を満たしていることを確認します。
4. コードをコミット：
   ```bash
   git add .
   git commit -m "<semantic commit message>"
   ```
5. 自分のリポジトリにプッシュ：`git push origin feature/<feature-name>`.
6. GitHub で PR を作成し、詳細な説明を提供して[@awwaawwa](https://github.com/awwaawwa)にレビューを依頼します。
7. すべての自動チェックが通過することを確認します。

> [!TIP]
>
> 開発が完全に完了するまで待つ必要はありません。早期に PR を作成することで、実装をレビューし、提案を行うことができます。
>
> ソースコードや関連事項について質問がある場合は、メンテナ aw@funstory.ai までお問い合わせください。
>
> バージョン 2.0 のリソースファイルは[BabelDOC](https://github.com/funstory-ai/BabelDOC)と共有されています。関連リソースのダウンロードコードは BabelDOC にあります。新しいリソースファイルを追加したい場合は、BabelDOC のメンテナ aw@funstory.ai までご連絡ください。

## 基本要件

<h4 id="sop">1. ワークフロー</h4>

- `main`ブランチからフォークし、フォークしたブランチで開発してください。
   - プルリクエスト（PR）を提出する際は、変更内容の詳細な説明を記載してください。
   - PR が自動チェックに合格しない場合（`checks failed`と赤い×マークで表示）、対応する`details`を確認し、修正を行って新しい PR がすべてのチェックに合格するようにしてください。


<h4 id="dev&test">2. 開発とテスト</h4>

- 開発とテストには `pip install -e .` コマンドを使用してください。


<h4 id="format">3. コードフォーマット</h4>

- `pre-commit`ツールを設定し、コードフォーマット用に`black`と`flake8`を有効にします。


<h4 id="requpdate">4. 依存関係の更新</h4>

- 新しい依存関係を導入する場合は、`pyproject.toml`ファイル内の依存関係リストを適宜更新してください。


<h4 id="docupdate">5. ドキュメント更新</h4>

- 新しいコマンドラインオプションを追加する場合、`README.md`ファイルのすべての言語バージョンにあるコマンドラインオプションのリストを適宜更新してください。


<h4 id="commitmsg">6. コミットメッセージ</h4>

- [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)を使用してください。例：`feat(translator): add openai`。


<h4 id="codestyle">7. コーディングスタイル</h4>

- 提出されたコードが基本的なコーディングスタイル標準に準拠していることを確認してください。
   - 変数名にはスネークケース（snake_case）またはキャメルケース（camelCase）を使用してください。


<h4 id="doctypo">8. ドキュメントフォーマット</h4>

- `README.md`のフォーマットについては、[中国語コピーライティングガイドライン](https://github.com/sparanoid/chinese-copywriting-guidelines)に従ってください。
   - 英語と中国語のドキュメントは常に最新の状態に保つようにし、その他の言語のドキュメント更新は任意とします。

## 翻訳エンジンの追加

1. `pdf2zh/config/translate_engine_model.py` ファイルに新しい翻訳エンジン設定クラスを追加します。
2. 同じファイル内の `TRANSLATION_ENGINE_SETTING_TYPE` 型エイリアスに新しい翻訳エンジン設定クラスのインスタンスを追加します。
3. `pdf2zh/translator/translator_impl` フォルダに新しい翻訳エンジン実装クラスを追加します。

> [!NOTE]
>
> このプロジェクトは、RPS（1 秒あたりのリクエスト数）が 4 未満の翻訳エンジンをサポートする意図はありません。そのようなエンジンのサポートを提出しないでください。

## プロジェクト構造

- **config folder**: 設定システム。
- **translator folder**: 翻訳関連の実装。
- **gui.py**: GUI インターフェースを提供。
- **const.py**: いくつかの定数。
- **main.py**: コマンドラインツールを提供。
- **high_level.py**: BabelDOC ベースの高レベルインターフェース。
- **http_api.py**: HTTP API を提供（未開始）。

## お問い合わせ

ご質問がある場合は、Issue を通じてフィードバックを提出するか、Telegram グループに参加してください。ご協力ありがとうございます！

> [!TIP]
>
> [没入型翻訳](https://immersivetranslate.com) は、このプロジェクトに積極的に貢献するコントリビューター向けに月額 Pro メンバーシップコードを提供しています。詳細はこちらをご覧ください：[BabelDOC/PDFMathTranslate コントリビューター報酬規則](https://funstory-ai.github.io/BabelDOC/CONTRIBUTOR_REWARD/)

<div align="right"> 
<h6><small>このページの一部のコンテンツは GPT によって翻訳されており、エラーが含まれている可能性があります。</small></h6>