よくある質問をまとめました。同じ問題に遭遇したユーザーのためにリストを提供しています。

## GPU は必要ですか？
- **質問**:
プログラムは人工知能を使用して文書を認識および抽出しますが、GPU は必要ですか？

- **回答**:
**GPU は必要ありません。** ただし、GPU がある場合、プログラムは自動的にそれを使用してより高いパフォーマンスを発揮します。

## ダウンロードが中断されましたか？
- **質問**:
モデルのダウンロード中に以下の中断エラーが発生しました。どうすればよいですか？

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **回答**:
ネットワークが干渉を受けています。安定したネットワークリンクを使用するか、ネットワーク介入をバイパスしてみてください。

## 最新バージョンに更新する方法は？
- **質問**:
最新バージョンの機能の一部を使用したいのですが、更新方法は？

- **回答**:
`pip install -U pdf2zh`


## 以下のファイルが存在しません：example.pdf
- **Issue**:
プログラムを実行すると、ドキュメントが見つからない場合、ユーザーには次のような出力が表示されます：`以下のファイルが存在しません: example.pdf`

- **解決策**:
  - ファイルが存在するディレクトリでコマンドラインを開く、または
  - pdf2zh の後にファイルのフルパスを直接入力する、または
  - インタラクティブモード`pdf2zh -i`を使用してファイルを直接ドラッグ＆ドロップする


## SSL エラーとその他のネットワーク問題
- **Issue**:
Hugging Face のモデルをダウンロードする際、中国のユーザーはネットワークエラーに遭遇する可能性があります。例えば、[issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55)、[#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70)で報告されています。

- **解決策**:
  - [GFW をバイパスする](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Hugging Face Mirror を使用する](https://hf-mirror.com/).
  - [ポータブル版を使用する](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [代わりに Docker を使用する](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [証明書を更新する](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55)で提案されている通り。

## Localhost にアクセスできない
以下をご覧ください。

## GUI の起動エラー（0.0.0.0 使用時）
- **Issue**:
グローバルモードでプロキシソフトウェアを使用すると、Gradio が正常に起動しない場合があります。例として、[issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77)をご覧ください。

- **解決策**:
ルールモードを使用する

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>このページの一部のコンテンツは GPT によって翻訳されており、エラーが含まれている可能性があります。</small></h6>