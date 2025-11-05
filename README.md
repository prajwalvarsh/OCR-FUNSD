# OCR-FUNSD Document Analysis Project

This project focuses on Optical Character Recognition (OCR) and document understanding using the FUNSD (Form Understanding in Noisy Scanned Documents) dataset. The project demonstrates various techniques for document analysis, including text extraction, bounding box detection, and form field recognition.

## Project Structure

```
├── data/                  # Additional data files
├── dataset/              
│   ├── testing_data/     # FUNSD test dataset
│   │   ├── annotations/  # JSON annotations for test data
│   │   └── images/      # Test document images
│   └── training_data/    # FUNSD training dataset
│       ├── annotations/  # JSON annotations for training data
│       └── images/      # Training document images
└── notebooks/            # Jupyter notebooks for analysis
```

## Notebooks

1. `02_02_working with opencv.ipynb` - Introduction to image processing with OpenCV
2. `02_03_intro_to_pytes.ipynb` - Introduction to Python testing
3. `03_bounding_boxes_index_ocr.ipynb` - Bounding box detection and OCR implementation
4. `03_ocr_index.ipynb` - Main OCR implementation and analysis
5. `04_01_get_whole_text.ipynb` - Full text extraction from documents

## Requirements

- Python 3.13
- OpenCV
- NumPy
- Matplotlib
- Pillow (PIL)
- Jupyter Notebook

Key dependencies are managed in a virtual environment. See `OCR/` directory for the complete environment setup.

## Dataset

The FUNSD dataset consists of 199 fully annotated forms with more than 30,000 word-level annotations. The dataset includes:
- Scanned form images
- JSON annotations with word-level bounding boxes
- Semantic entity labels
- Relationships between fields

The dataset is split into training and testing sets, located in their respective directories.

## Getting Started

1. Clone this repository
2. Set up the Python virtual environment:
   ```powershell
   python -m venv OCR
   .\OCR\Scripts\activate
   ```
3. Install required packages:
   ```powershell
   pip install -r requirements.txt
   ```
4. Launch Jupyter Notebook:
   ```powershell
   jupyter notebook
   ```
5. Start with the introductory notebooks (02_*.ipynb) to understand the basics

## Features

- Document image preprocessing using OpenCV
- Text extraction and OCR processing
- Bounding box detection for form fields
- Form structure analysis
- Complete text extraction from documents


