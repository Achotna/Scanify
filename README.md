# Scanify

**Authors:** Antonina Savchenko & Elisa Salignon

>>> [A little video] (https://github.com/Achotna/Scanify/blob/main/Scanify/Scanify_video.mp4)

Scanify is a project developed for the **Trophées NSI competition**.

The application allows users to analyze receipts and better understand their expenses. It uses OCR to extract information from receipt images and then generates graphs to make spending easier to visualize and manage.

> **Language:** The application is currently available only in **French**.

## Features

- Upload a receipt as an image
- Extract information using OCR
- Analyze receipt data
- Generate graphs to visualize expenses
- Help users keep track of their spending

## Installation

### Requirements

Before running the project, make sure you have installed:

- **Python 3.11 or later**
- All Python libraries listed in `requirements.txt`
- **Tesseract OCR**  
  You can download it from: https://github.com/UB-Mannheim/tesseract/wiki
- An **API key** and the required configuration file to use it

For detailed installation instructions, follow:

`docs/installation.md`

## Running the Project

First, install the required Python packages:

```bash
pip install -r requirements.txt
```

Then make sure that Tesseract OCR is correctly installed and that its installation path is configured in `ocr.py`.

Follow the instructions in `docs/installation.md` to configure the API key and launch the application.

## Constraints and Limitations

### Operating System

The project has only been tested on **Windows**. Some features may not work correctly on macOS or Linux.

### Python Version

Python **3.11 or later** is recommended to avoid compatibility problems with some libraries.

### Dependencies

All libraries listed in `requirements.txt` must be installed before running the project.

### Tesseract OCR

The path to the Tesseract installation must be correctly configured in `ocr.py`.

### Image Quality

OCR performance can decrease if the uploaded image is:

- blurry,
- too large,
- poorly lit,
- or difficult to read.

### Supported Files

Receipts must be uploaded as images.

Currently supported formats include:

- `.jpg`
- `.jpeg`

### Receipt Complexity

For the best results, receipts should be similar to the examples available in the `test` folder.

The current version works best with receipts that:

- are relatively short,
- have clear product names,
- do not contain complex discounts or promotions,
- and have good image quality.

The application is not yet fully adapted to more complex receipts.

## Project Status

Scanify is still a developing project. Future improvements could include better support for complex receipts, additional image formats, improved OCR accuracy, and support for more languages.

## License

This project is licensed under the **GPL v3+ License**.

See `LICENCE.txt` for more information.
