Some questions are frequently asked, so we have provided a list for users who encounter similar issues.

## Is a GPU required?
- **Question**:  
As the program uses artificial intelligence to recognize and extract documents, is GPU required?

- **Answer**:  
**GPU is not required.** But if you have a GPU, the program will automatically use it for higher performance.

## Downloading interrupted?
- **Question**:  
I encountered the following interrupt error while downloading the model. What should I do?

  ![image](https://github.com/user-attachments/assets/3c4eed44-3d9b-4e2f-a224-a58edca718c2)

- **Answer**:  
The network is receiving interference, please use a stable network link or try to bypass network intervention.

## How to update to the latest version?
- **Question**:  
I want to use some of the features of the latest version, how do I update it?

- **Answer**:  
`pip install -U pdf2zh`


## The following files do not exist: example.pdf
- **Issue**:  
When executing the program, users would have the following outputs: `The following files do not exist: example.pdf` if the document was not found.

- **Solution**:
  - Open the command line in the directory where the file is located, or
  - Enter the full path of the file directly after pdf2zh, or
  - Use the interactive mode `pdf2zh -i` to drag and drop files directly


## SSL Error and Other Network Issues
- **Issue**:  
When downloading hugging face models, users in China may get network error. For example, in [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55), [#70](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/70).

- **Solution**:
  - [Bypass GFW](https://github.com/clash-verge-rev/clash-verge-rev).
  - [Use Hugging Face Mirror](https://hf-mirror.com/).
  - [Use Portable version](https://github.com/PDFMathTranslate/PDFMathTranslate-next?tab=readme-ov-file#method-ii-portable).
  - [Use Docker instead](https://github.com/PDFMathTranslate/PDFMathTranslate-next#docker).
  - [Update Certificates](https://stackoverflow.com/questions/51925384/unable-to-get-local-issuer-certificate-when-using-requests), as suggested in [issue #55](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/55).

## Localhost is not accessible
Please see below.

## Error launching GUI using 0.0.0.0
- **Issue**:  
Using proxy software in global mode may prevent Gradio from starting properly. For example, in [issue #77](https://github.com/PDFMathTranslate/PDFMathTranslate-next/issues/77).

- **Solution**:  
Use rule mode

  ![image](https://github.com/user-attachments/assets/b1f2b16a-eb6a-4c03-995c-332ef1d82c96)