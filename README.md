# Hindi-PDF-OCR-on-Google-Colab by Akella Niranjan
Every day we tend to scan many hard copies for various purposes. So, one such application confronted me where the scanned literature was in an Indian language - "Hindi" where the script was in a .pdf file format and when copied to a word document couldn't be recognize, hence displaying ASCII values.

So I developed an algorithm to convert scanned Hindi documents to text files for further use like notation editing, translating to other languages etc; using Googles Tesseract Engine. 

- Initially install all the necessary packages on to the Google Colab instance using the following commands
```
!pip install pytesseract
!sudo apt install tesseract-ocr
!apt-get update
!pip install pdf2image
!apt-get install poppler-utils
!sudo apt-get install tesseract-ocr-hin
```

- Then refer the algorithm in this <a href='Hindi_OCR.ipynb'>Jupyter Notebook</a>

## Further Usages

This algorithm can be used for a wider set of languages by installing the desired language model through the follwing command. 

- Change the language from 'hin' to desired language from the language list <a herf = 'https://tesseract-ocr.github.io/tessdoc/Data-Files-in-different-versions.html'> Here.</a>
```
#Exambple for English
!sudo apt-get install tesseract-ocr-eng
```
- Also change the "lang" parameter in the python code from 'hin' to desired language as follows,
```
#Example for English
pytesseract.image_to_string(x, lang = 'eng')
```