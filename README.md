# Writer_Identification_Kannada

 * Writer Identification: Designed a system for identifying the authors of Kannada manuscripts and handwritten texts. This project employs the VGG16 CNN architecture to analyze handwriting features and accurately classify the writer based on their unique writing style, achieving 100% accuracy.
 * ![Screenshot 2024-10-02 232320](https://github.com/user-attachments/assets/8f5a36cb-6f22-4ace-8638-1734a56c415d)
  * The Writer Identification system can be used in forensic analysis to identify authors in criminal investigations, assist researchers in analyzing historical manuscripts, and aid educational institutions in providing personalized feedback on handwriting.
  * The Writer Identification system can be used in:
  * Forensic analysis to identify authors in criminal investigations.
  * Assisting researchers in analyzing historical manuscripts.
  * Aiding educational institutions in providing personalized feedback on handwriting.
  * ![Screenshot (317)](https://github.com/user-attachments/assets/42c4b162-0153-4f1f-b44c-4ccb5415e9db)
  * ![Screenshot 2024-10-02 232357](https://github.com/user-attachments/assets/8cf81d11-086d-4689-acfc-7360b39b3a1a)

    # Kannada OCR and Writer Identification Project
---

## Team Members
- **Suhas S**
- **Sai Darshan**
- **Guhan KS**
--- 

## Overview

This project was developed as part of the "Kannada Hackathon," focusing on enhancing technology for the Kannada language. The primary objective is to improve text extraction from images and PDF files using advanced Optical Character Recognition (OCR) techniques, as well as implement innovative solutions such as writer identification and keyword search for Kannada texts.

### Key Features:
- **Image to Text Extraction**: Developed an advanced OCR system capable of extracting text from Kannada images, leveraging machine learning techniques to enhance accuracy and efficiency.
- **Writer Identification**: Designed a system to identify the authors of Kannada manuscripts and handwritten texts using VGG16 CNN architecture.
- **Keyword Search**: Implemented a keyword search functionality for Kannada text files, allowing custom searches within large volumes of text.

---

## Project Flow

1. **Input Handling**:
   - Extract images from PDFs using `PyMuPDF`.
   - Load and preprocess images (invert colors, sharpen, apply binary thresholding).

2. **Image Preprocessing**:
   - Enhance image quality for OCR by applying sharpening filters and thresholding.
   - Crop images based on detected rows and columns of text.
   - Remove duplicate cropped images using Structural Similarity Index (SSIM).

3. **OCR Process**:
   - Choose between three OCR engines: Tesseract, EasyOCR, and PaddleOCR.
   - Extract Kannada and English text from preprocessed images.

4. **Text Output**:
   - Save extracted text to organized directories in `.txt` files.
   - Option to append or overwrite OCR results based on user requirements.

---

## Hackathon Initiatives

### Image to Text Extraction
We developed a powerful OCR system that extracts Kannada text from images using machine learning models like Convolutional Neural Networks (CNNs). The system enhances both accuracy and efficiency, helping streamline the process of converting images into text files.

### Writer Identification
In addition to OCR, we designed a writer identification system for Kannada manuscripts and handwritten documents. This project utilizes the VGG16 CNN architecture to analyze handwriting features and classify authors based on their unique writing style.

- **Applications**:  
  - Forensic analysis: Identifying authors in criminal investigations.  
  - Historical research: Analyzing historical Kannada manuscripts.  
  - Education: Providing personalized feedback on handwriting.

### Keyword Search
We implemented a keyword search functionality for Kannada text files. Users can easily conduct custom searches, making it faster and easier to find specific information within large volumes of text.

---

## Installation

To run this project, install the required Python packages mentioned below: 

### Required Packages:
- `opencv-python`
- `PyMuPDF`
- `pytesseract`
- `easyocr`
- `paddleocr`
- `scikit-image`
- `numpy`

---


Available OCR models:
- `tesseract`
- `easyocr`
- `paddleocr`

---

## Directory Structure

```
project_root/
│
├── output/
│   ├── pdf_images/        # Extracted images from PDF
│   ├── preprocessed_images/  # Preprocessed images for OCR
│   ├── cropped_images/    # Cropped images based on rows and columns
│   └── ocr_texts/         # Extracted text saved as .txt files
│
├── main.py                # Main script for running the OCR process
└── requirements.txt       # Python packages to install
```

---

## Future Improvements
- **Improved OCR Accuracy**: Further refining image preprocessing techniques for better accuracy in low-quality documents.
- **GUI Interface**: Developing a user-friendly interface to make the process more accessible.
- **Optimised Preprocessing Flow** : This will good to process and analyse the text even in more obsure conditions
