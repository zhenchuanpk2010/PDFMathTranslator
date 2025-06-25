[**開始**](./getting-started.md) > **インストール** > **Windows EXE** _(現在)_

---

### .exeファイル経由でPDFMathTranslateをインストール

***ステップ 1*** | [リリースページ](https://github.com/PDFMathTranslate/PDFMathTranslate-next/releases)から `pdf2zh-<version>-with-assets-win64.zip` をダウンロードします。

> [!TIP]
> **`pdf2zh-<version>-with-assets-win64.zip` と `pdf2zh-<version>-win64.zip` の違いは何ですか？**
>
> - PDFMathTranslateを初めてダウンロードして使用する場合は、`pdf2zh-<version>-with-assets-win64.zip` をダウンロードすることをお勧めします。
> - `pdf2zh-<version>-with-assets-win64.zip` には、`pdf2zh-<version>-win64.zip` と比較してリソースファイル（フォントやモデルなど）が含まれています。
> - アセットなしのバージョンも実行時にリソースを動的にダウンロードしますが、ネットワークの問題によりダウンロードが失敗する可能性があります。

***ステップ2*** | `pdf2zh-<version>-with-assets-win64.zip` を解凍し、`pdf2zh` フォルダに移動します。解凍には時間がかかる場合がありますので、しばらくお待ちください。

***ステップ3*** | `pdf2zh` フォルダに移動し、`pdf2zh.exe` をダブルクリックします。

> [!TIP]
> **.exeファイルが実行できない場合**
>
> pdf2zh.exeの実行に問題がある場合は、`https://aka.ms/vs/17/release/vc_redist.x64.exe`をインストールして再度お試しください。

***ステップ4*** | exeファイルをダブルクリックするとターミナルが表示されます。約30秒から1分後に、デフォルトのブラウザでウェブページが開きます。開かない場合は、手動で`http://localhost:7860/`にアクセスしてみてください。

> [!NOTE]
>
> WebUIの使用中に問題が発生した場合は、[このページ](./USAGE_webui.md)を参照してください。

***ステップ5*** | お楽しみください！

> [!TIP]
> **.exeファイルはコマンドラインから使用できます**
>
> .exeファイルは以下のようにコマンドラインから使用できます:
>
> - ターミナルを起動し、.exeファイルが含まれるフォルダに移動します:
>
> ```bash
> cd /path/pdf2zh_next/build
> ```
>
> - .exeファイルを呼び出します:
>
> ```bash
> ./pdf2zh_next.exe "document.pdf"
> ```
>
> 他のコマンドラインパラメータも通常通り使用できます:
>
> ```bash
> ./pdf2zh_next.exe "document.pdf" --lang-in en --lang-out ja
> ```
>
> コマンドラインの使い方についてさらに情報が必要な場合は、こちらの記事を参照してください。

<div align="right"> 
<h6><small>このページの一部のコンテンツはGPTによって翻訳されており、エラーが含まれている可能性があります。</small></h6>