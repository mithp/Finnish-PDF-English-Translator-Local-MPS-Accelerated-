# Finnish PDF → English Translator (Local, MPS‑Accelerated)

This repository provides a fully local, privacy‑preserving pipeline for translating **Finnish-language PDFs** into **English text files**, supporting:

- Native text extraction (for digital PDFs)
- OCR text extraction using Tesseract (for scanned PDFs)
- Sentence segmentation
- MarianMT translation (Helsinki-NLP/opus-mt-fi-en)
- Apple Silicon **MPS GPU acceleration**
- Complete offline execution (except first-time model download)

This is ideal for research, clinical documents, historical Finnish text, student papers, or any privacy-sensitive content.

---

## 🚀 Features

- **🔍 Automatic PDF type detection**  
  Detects if a PDF contains selectable text or requires OCR.

- **📖 OCR for scanned PDFs**  
  Uses `pytesseract` + `pdfplumber`.

- **💬 Sentence-based translation**  
  Translation quality improves when we translate sentence-by-sentence.

- **⚡ MPS GPU acceleration**  
  Dramatically faster translation on Apple Silicon:  
  (M1/M2/M3/M4 chips supported)

- **🧠 Local MarianMT model**  
  No cloud calls. No data leaves your device.

---

## 🛠️ Installation

### 1. Install system dependencies

#### macOS (recommended)

```bash
brew install tesseract
brew install tesseract-lang
brew install poppler
brew install libjpeg
