# OCRos - OCR Application

OCRos is a simple Optical Character Recognition (OCR) tool built using Python and Tkinter. It allows users to upload images, crop them, and extract text using Tesseract OCR. 

![Project Demo](OCRos.gif)

## Features
- Upload and display images.
- Crop images using a mouse interaction.
- Extract text from the cropped image using Tesseract OCR.
- Text is displayed in a text box for easy copy-pasting.

## Requirements
Make sure you have the following installed:
- Python 3.x
- Tesseract OCR (make sure the Tesseract executable is accessible in your PATH)
- Tkinter (comes pre-installed with Python on most systems)
- Pillow library for image handling
- pytesseract Python wrapper for Tesseract OCR

## Installation

### Step 1: Install Python Dependencies

You can install the required Python libraries by running the following command in your terminal:

```bash
pip install -r requirements.txt
```

Where `requirements.txt` includes the following packages:
- Pillow
- pytesseract
- tkinter (if not pre-installed)

### Step 2: Install Tesseract

#### On Linux (Ubuntu-based):
Install Tesseract OCR via:

```bash
sudo apt-get update
sudo apt-get install tesseract-ocr
```

#### On macOS:
Install using Homebrew:

```bash
brew install tesseract
```

#### On Windows:
Download and install Tesseract from the official GitHub page: 
[https://github.com/tesseract-ocr/tesseract](https://github.com/tesseract-ocr/tesseract)

Make sure the Tesseract executable is added to your system's PATH.

### Step 3: Configure Tesseract Path

The OCRos app will automatically detect the Tesseract executable based on your platform:
- **Linux**: `/usr/bin/tesseract`
- **macOS**: `/usr/local/bin/tesseract`
- **Windows**: `C:\Program Files\Tesseract-OCR\tesseract.exe`

If necessary, update the `ocros_logic.py` file to set the correct Tesseract path for your system.

### Step 4: Run the App

Once everything is set up, you can run the OCRos app by executing the following command:

```bash
python main.py
```

The OCRos GUI will open, and you can upload an image, crop it, and extract text using Tesseract OCR.

## Usage

1. **Upload Image**: Click the "Załaduj obraz" button to upload an image.
2. **Crop Image**: Use the mouse to select the area of the image you want to crop.
3. **Extract Text**: After cropping, click the "Wydobądź tekst" button to extract text using Tesseract OCR. The text will be displayed in the text box.

## License

This project is licensed under the MIT License.