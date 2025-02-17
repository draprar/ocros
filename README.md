# OCRos - OCR Application

OCRos is a Python-based GUI application that provides an easy-to-use Optical Character Recognition (OCR) tool to upload, crop, and extract text from images. The application is built using `tkinter` and utilizes Tesseract OCR for text extraction.

![Project Demo](OCRos.gif)

## Features
- **Image Upload**: Upload and display images for text extraction.
- **Image Cropping**: Select and crop a specific area of the image using a mouse.
- **Text Extraction**: Extract text from the cropped image and display it in a text box for easy copying.

## Technologies Used
- **Python 3.x**
- **Tkinter**: For the graphical user interface.
- **Pillow**: For image processing.
- **pytesseract**: A Python wrapper for Tesseract OCR.

## Installation

### 1. Clone the repository:

```bash
git clone https://github.com/draprar/ocr-app_ocros.git
cd ocr-app_ocros
```

### 2. Install dependencies:

```bash
pip install -r requirements.txt
```
### 3. Set Up Tesseract OCR:

#### On Linux (Ubuntu-based):

```bash
sudo apt-get update
sudo apt-get install tesseract-ocr
```

#### On macOS (using Homebrew):

```bash
brew install tesseract
```

#### On Windows:
Download and install Tesseract from the official GitHub page: 
[Tesseract OCR](https://github.com/tesseract-ocr/tesseract). Add the Tesseract executable to your system's PATH.

### 4. Configure Tesseract Path

The OCRos app will automatically detect the Tesseract executable based on your platform:
- **Linux**: `/usr/bin/tesseract`
- **macOS**: `/usr/local/bin/tesseract`
- **Windows**: `C:\Program Files\Tesseract-OCR\tesseract.exe`

If necessary, update the `ocros_logic.py` file to set the correct Tesseract path for your system.

### 5. Run the App

```bash
python main.py
```

The OCRos GUI will open, and you can upload an image, crop it, and extract text using Tesseract OCR.

## How to Use

1. **Upload Image**: Click the "Załaduj obraz" button to upload an image.
2. **Crop Image**: Use the mouse to select the area of the image you want to crop.
3. **Extract Text**: After cropping, click the "Wydobądź tekst" button to extract text using Tesseract OCR. The text will be displayed in the text box.

## Contributing

If you’d like to contribute to the project, feel free to submit a pull request. Make sure to adhere to the existing code style and include detailed explanations of your changes.

## License

This project is licensed under the MIT License.