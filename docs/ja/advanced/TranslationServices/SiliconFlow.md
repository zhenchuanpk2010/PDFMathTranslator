# SiliconFlow

## 無料翻訳サービス

[SiliconFlow](https://siliconflow.cn) はこのプロジェクトに無料翻訳サービスを提供しています。

現在、無料翻訳サービスでは `THUDM/GLM-4-9B-0414` モデルが使用されます。

### 使い方

#### コマンドライン

```bash
pdf2zh_next --siliconflowfree example.pdf 
```

#### webui

1. 「翻訳オプション」 - 「サービス」ドロップダウンリストから「SiliconFlowFree」を選択します。
2. ページ下部の「翻訳」ボタンをクリックして翻訳を開始します。
3. 翻訳が完了したら、ページ下部の「翻訳済み」セクションで翻訳された `PDF` ファイルを見つけることができます。


### プライバシーポリシー

ファイルの内容は、プロジェクトのメンテナー [@awwaawwa](https://github.com/awwaawwa) のサーバーに送信され、その後 SiliconFlow に転送されて翻訳されます。

このプロジェクトのメンテナーは、SiliconFlow から返されるエラー情報のみを収集し、関連サービスのデバッグに使用します。ファイルの内容は収集されません。

SiliconFlow プライバシーポリシー：[简体中文](https://docs.siliconflow.cn/cn/legals/privacy-policy)/[English](https://docs.siliconflow.cn/en/legals/privacy-policy)



## SiliconFlow の他のモデルを使用する

[SiliconFlow](https://siliconflow.cn) は翻訳用の他のモデルも提供しています。

### 使い方

1. [SiliconFlow](https://siliconflow.cn) でアカウントを登録してください

2. [SiliconFlow API Key](https://cloud.siliconflow.cn/me/account/ak) で API キーを作成します。その後、キーをクリックしてコピーしてください。

#### コマンドライン

```bash
pdf2zh_next --siliconflow --siliconflow-model "Pro/deepseek-ai/DeepSeek-V3" --siliconflow-api-key <your-api-key> example.pdf
```

#### webui

1. 「翻訳オプション」 - **「サービス」** ドロップダウンリスト： 「SiliconFlow」を選択
2. 「翻訳オプション」 - **「SiliconFlow API のベース URL」**：デフォルトのまま
3. 「翻訳オプション」 - **「使用する SiliconFlow モデル」**： 「Pro/deepseek-ai/DeepSeek-V3」または他のモデルを入力
4. 「翻訳オプション」 - **「SiliconFlow サービスの API キー」**：API キーを貼り付け
5. ページ下部の「翻訳」ボタンをクリックして翻訳を開始
6. 翻訳が完了したら、ページ下部の「翻訳済み」セクションで翻訳された `PDF` ファイルを確認できます。


## 謝辞

[SiliconFlow](https://siliconflow.cn) に、このプロジェクトのために無料翻訳サービスを提供していただき感謝します。

<div align="right"> 
<h6><small>このページの一部のコンテンツは GPT によって翻訳されており、エラーが含まれている可能性があります。</small></h6>