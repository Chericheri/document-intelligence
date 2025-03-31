# 📄 Smart Document Processing with OpenCV & Tesseract OCR

![Platforms](https://img.shields.io/badge/Platform-Windows%20|%20macOS%20|%20Linux-blue)
![Demo](https://img.shields.io/badge/Demo-Streamlit-important)
![License](https://img.shields.io/badge/License-MIT-success)

A cross-platform guide for extracting text from documents using **OpenCV** and **Tesseract OCR**. Complete with setup instructions for different operating systems.

---

##  Overview

This project demonstrates how to:
- Detect text regions in images using computer vision techniques.
- Extract machine-readable text using Tesseract OCR.
- Build an interactive document scanner with **Streamlit**.
- **No deep learning required** – lightweight and efficient!

---

##  Key Features

- **OCR Workflow**: Preprocessing → Text Localization → OCR → Postprocessing  
- **Tool Roles**:
  - `OpenCV`: Image thresholding, contour detection, and ROI extraction.  
  - `Tesseract`: Optical Character Recognition (OCR) engine.
- **Challenges Addressed**: Handling low contrast, multi-language text, and complex layouts.
- **Limitations**: Simpler but less accurate than deep learning approaches like LayoutParser.

---

##  Installation Guide

### 1. Clone the Repository
```bash
git clone https://github.com/Chericheri/document-intelligence.git
cd document-intelligence
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Install Tesseract OCR

| OS         | Command                                                                 | Additional Notes                          |
|------------|-------------------------------------------------------------------------|-------------------------------------------|
| **Windows**| [Download installer](https://github.com/UB-Mannheim/tesseract/wiki)     | Check "Add to PATH" during install        |
| **macOS**  | `brew install tesseract`                                                | Requires [Homebrew](https://brew.sh)      |
| **Linux**  | `sudo apt install tesseract-ocr libtesseract-dev`                       | For Debian/Ubuntu                         |

---

## 🖥️ Running the Project

**For Streamlit Web App:**
```bash
streamlit run ScanDoc.py
```

**For Jupyter Notebook:**
```bash
jupyter notebook
```

---

## 📌 Configuration

Ensure Tesseract OCR is correctly set up in your Python script:
```python
import pytesseract

# Windows
pytesseract.pytesseract.tesseract_cmd = r'C:\Program Files\Tesseract-OCR\tesseract.exe'

# macOS
pytesseract.pytesseract.tesseract_cmd = '/usr/local/bin/tesseract'

# Linux
pytesseract.pytesseract.tesseract_cmd = '/usr/bin/tesseract'
```

---

## 📜 License
MIT License - Free for academic and commercial use. Tesseract OCR is Apache 2.0 licensed.

---

## 🤝 Contributing
Contributions are welcome! Feel free to fork the repo and submit a pull request.

---

## 📧 Contact
For questions or suggestions, reach out via [GitHub Issues](https://github.com/Chericheri/document-intelligence/issues).

