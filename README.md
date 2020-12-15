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
