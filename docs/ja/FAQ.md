よくある質問がいくつかあるため、同様の問題に遭遇したユーザー向けにリストを用意しました。

## GPUは必要ですか？

- **質問**:  
このプログラムは人工知能を使用して文書を認識・抽出しますが、GPUは必要ですか？

- **回答**:  
**GPUは必須ではありません。** ただし、GPUがある場合、プログラムは自動的にそれを使用してより高いパフォーマンスを発揮します。

## ダウンロードが中断されました？

- **質問**:  
モデルのダウンロード中に以下の中断エラーが発生しました。どうすればよいですか？

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **回答**:  
ネットワークが干渉を受けています。安定したネットワーク接続を使用するか、ネットワーク介入を回避するようにしてください。

## 最新バージョンへの更新方法は？

- **質問**:  
最新バージョンの機能の一部を使用したいのですが、どのように更新すればよいですか？

- **回答**:  
`pip install -U pdf2zh`

## 以下のファイルが存在しません: example.pdf

- **Issue**:  
プログラムを実行すると、ドキュメントが見つからない場合、ユーザーには次のような出力が表示されます: `The following files do not exist: example.pdf`

- **解決策**:
  - ファイルがあるディレクトリでコマンドラインを開く、または
  - pdf2zhの後にファイルのフルパスを直接入力する、または
  - インタラクティブモード `pdf2zh -i` を使用してファイルを直接ドラッグ＆ドロップする

## SSLエラーおよびその他のネットワーク問題

- **問題**:  
Hugging Faceのモデルをダウンロードする際、中国のユーザーはネットワークエラーに遭遇する可能性があります。例えば、[issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55)、[#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70)で報告されています。

- **解決策**:
  - [GFWをバイパスする](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Hugging Faceミラーを使用する](https://hf-mirror.com/).
  - [ポータブル版を使用する](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [代わりにDockerを使用する](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [証明書を更新する](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55)で提案されている通り。

## ローカルホストにアクセスできない

以下をご覧ください。

## GUIを0.0.0.0で起動する際のエラー

- **問題**:  
グローバルモードでプロキシソフトウェアを使用すると、Gradioが正常に起動しない場合があります。例として、[issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77)を参照してください。

- **解決策**:  
ルールモードを使用する

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)

<div align="right"> 
<h6><small>このページの一部のコンテンツはGPTによって翻訳されており、エラーが含まれている可能性があります。</small></h6>