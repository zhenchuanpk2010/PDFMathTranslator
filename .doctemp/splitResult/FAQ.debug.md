<!-- CHUNK ID: chunk_BBFC419C  CHUNK TYPE: paragraph START_LINE:1 -->
Some questions are frequently asked, so we have provided a list for users who encounter similar issues.

<!-- CHUNK ID: chunk_2B5D23E7  CHUNK TYPE: header START_LINE:3 -->
## Is a GPU required?
<!-- CHUNK ID: chunk_A85F81AE  CHUNK TYPE: list START_LINE:4 -->
- **Question**:  
<!-- CHUNK ID: chunk_8E573398  CHUNK TYPE: paragraph START_LINE:5 -->
As the program uses artificial intelligence to recognize and extract documents, is GPU required?

<!-- CHUNK ID: chunk_FE846FC9  CHUNK TYPE: list START_LINE:7 -->
- **Answer**:  
<!-- CHUNK ID: chunk_63C892F6  CHUNK TYPE: paragraph START_LINE:8 -->
**GPU is not required.** But if you have a GPU, the program will automatically use it for higher performance.

<!-- CHUNK ID: chunk_610DD2DC  CHUNK TYPE: header START_LINE:10 -->
## Downloading interrupted?
<!-- CHUNK ID: chunk_A85F81AE  CHUNK TYPE: list START_LINE:11 -->
- **Question**:  
<!-- CHUNK ID: chunk_53B66922  CHUNK TYPE: paragraph START_LINE:12 -->
I encountered the following interrupt error while downloading the model. What should I do?

<!-- CHUNK ID: chunk_663B9855  CHUNK TYPE: image START_LINE:14 -->
  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

<!-- CHUNK ID: chunk_FE846FC9  CHUNK TYPE: list START_LINE:16 -->
- **Answer**:  
<!-- CHUNK ID: chunk_2A133C40  CHUNK TYPE: paragraph START_LINE:17 -->
The network is receiving interference, please use a stable network link or try to bypass network intervention.

<!-- CHUNK ID: chunk_ABB33668  CHUNK TYPE: header START_LINE:19 -->
## How to update to the latest version?
<!-- CHUNK ID: chunk_A85F81AE  CHUNK TYPE: list START_LINE:20 -->
- **Question**:  
<!-- CHUNK ID: chunk_981A22AF  CHUNK TYPE: paragraph START_LINE:21 -->
I want to use some of the features of the latest version, how do I update it?

<!-- CHUNK ID: chunk_FE846FC9  CHUNK TYPE: list START_LINE:23 -->
- **Answer**:  
<!-- CHUNK ID: chunk_E6E8A1D1  CHUNK TYPE: paragraph START_LINE:24 -->
`pip install -U pdf2zh`


<!-- CHUNK ID: chunk_9FB0E3EA  CHUNK TYPE: header START_LINE:27 -->
## The following files do not exist: example.pdf
<!-- CHUNK ID: chunk_22B1E6C4  CHUNK TYPE: list START_LINE:28 -->
- **Issue**:  
<!-- CHUNK ID: chunk_FAB807CC  CHUNK TYPE: paragraph START_LINE:29 -->
When executing the program, users would have the following outputs: `The following files do not exist: example.pdf` if the document was not found.

<!-- CHUNK ID: chunk_E7371FD6  CHUNK TYPE: list START_LINE:31 -->
- **Solution**:
  - Open the command line in the directory where the file is located, or
  - Enter the full path of the file directly after pdf2zh, or
  - Use the interactive mode `pdf2zh -i` to drag and drop files directly


<!-- CHUNK ID: chunk_F523458B  CHUNK TYPE: header START_LINE:37 -->
## SSL Error and Other Network Issues
<!-- CHUNK ID: chunk_22B1E6C4  CHUNK TYPE: list START_LINE:38 -->
- **Issue**:  
<!-- CHUNK ID: chunk_DF99BBC1  CHUNK TYPE: paragraph START_LINE:39 -->
When downloading hugging face models, users in China may get network error. For example, in [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55), [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70).

<!-- CHUNK ID: chunk_AC4D20E5  CHUNK TYPE: list START_LINE:41 -->
- **Solution**:
  - [Bypass GFW](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Use Hugging Face Mirror](https://hf-mirror.com/).
  - [Use Portable version](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [Use Docker instead](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [Update Certificates](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), as suggested in [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55).

<!-- CHUNK ID: chunk_8AA448AC  CHUNK TYPE: header START_LINE:48 -->
## Localhost is not accessible
<!-- CHUNK ID: chunk_4E814B7B  CHUNK TYPE: paragraph START_LINE:49 -->
Please see below.

<!-- CHUNK ID: chunk_EA897629  CHUNK TYPE: header START_LINE:51 -->
## Error launching GUI using 0.0.0.0
<!-- CHUNK ID: chunk_22B1E6C4  CHUNK TYPE: list START_LINE:52 -->
- **Issue**:  
<!-- CHUNK ID: chunk_D65A22CE  CHUNK TYPE: paragraph START_LINE:53 -->
Using proxy software in global mode may prevent Gradio from starting properly. For example, in [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77).

<!-- CHUNK ID: chunk_587F7FBA  CHUNK TYPE: list START_LINE:55 -->
- **Solution**:  
<!-- CHUNK ID: chunk_E7C819A4  CHUNK TYPE: paragraph START_LINE:56 -->
Use rule mode

<!-- CHUNK ID: chunk_E6DC933A  CHUNK TYPE: image START_LINE:58 -->
  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)