# Printed Text Scanner (PyTesseract + PyQt5)

A GUI-based printed text scanner for the "AI Without ML" assignment. Built with PyQt5, OpenCV and PyTesseract.

## Features
- Load images from disk
- Live camera preview and capture
- Select ROI (drag on the preview)
- Preprocessing options (grayscale, binarize, adaptive thresh, denoising)
- Run OCR with configurable Tesseract OEM/PSM
- Overlay boxes showing detected words on the image
- Save extracted text to `.txt`

## Requirements
- Python 3.8+
- pip packages:

- **Tesseract-OCR** (system dependency)
- Windows: install from Tesseract releases and add to PATH
- Ubuntu/Debian: `sudo apt install tesseract-ocr`
- macOS (Homebrew): `brew install tesseract`

If Tesseract is not in PATH, open `printed_text_scanner.py` and set:
```py
pytesseract.pytesseract.tesseract_cmd = r"C:\Program Files\Tesseract-OCR\tesseract.exe"

DONE WITH 💗 by IRADUKUNDA Joyeuse