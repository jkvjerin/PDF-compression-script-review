# PDF-compression-script-review
PDF compression script review


# PDF Compressor (Ghostscript + Python)

This project provides a simple **PDF compressor** using Ghostscript, with progress bars, DPI control, visual previews, and batch mode.  
Works in **Google Colab** or locally in **Jupyter Notebook**.

---

## 🚀 Quick Start in Google Colab

Click the badge below to open the notebook in Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/your-username/your-repo/blob/main/compress_pdfs.ipynb)

---

## 📥 Local Installation

1. Clone the repo:
   ```bash
   git clone https://github.com/your-username/your-repo.git
   cd your-repo
   ```

2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Launch Jupyter:
   ```bash
   jupyter notebook compress_pdfs.ipynb
   ```

---

## 📌 Features

- ✅ Compress single PDF with Ghostscript  
- ✅ Preset qualities (`screen`, `ebook`, `printer`, `prepress`)  
- ✅ Custom DPI downsampling  
- ✅ Progress bar per page  
- ✅ Visual **before/after preview** of pages  
- ✅ Batch mode (compress all PDFs in a folder)  
- ✅ Auto-download in Colab  

---

## 🖼 Preview Example

Original vs Compressed (first page):

![Preview Example](example_preview.png)

Preview Example

Original vs Compressed (first page):


---

### 📌 Example `compress_pdfs.ipynb`

Structure:

- **Setup cell**
  ```python
  !apt-get install -y ghostscript poppler-utils
  !pip install PyPDF2 tqdm pdf2image
  ```

- **Import + Functions**
(copy the compress_pdf_with_progressbar, preview_pdf_quality, and compress_pdfs_in_folder code here)

- **Single file compression demo** 
 ```python
compress_pdf_with_progressbar("input.pdf", "output.pdf", dpi=150)
preview_pdf_quality("input.pdf", "output.pdf", page_num=0)
```

- **Batch compression demo**
 ```python
compress_pdfs_in_folder("my_pdfs", "compressed", dpi=150)
```
---
