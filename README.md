# Optical Character Recognition (OCR) with Pytesseract
This repository contains code snippets demonstrating how to perform Optical Character Recognition (OCR) using Pytesseract, an OCR tool for Python. Pytesseract is a wrapper for Google's Tesseract-OCR Engine, which is widely used for extracting text from images.

## Requirements
Make sure you have the following dependencies installed:
pytesseract
PIL (Python Imaging Library)
OpenCV (cv2)

You can install these dependencies using pip:
pip install pytesseract pillow opencv-python matplotlib

### Page Segmentation Modes:
Pytesseract provides various page segmentation modes for different types of text in images. These modes determine how the OCR engine should interpret and process the image.
Here are the available segmentation modes:

0 Orientation and script detection (OSD) only.
1 Automatic page segmentation with OSD.
2 Automatic page segmentation, but no OSD, or OCR.
3 Fully automatic page segmentation, but no OSD. (Default)
4 Assume a single column of text of variable sizes.
5 Assume a single uniform block of vertically aligned text.
6 Assume a single uniform block of text.
7 Treat the image as a single text line.
8 Treat the image as a single word.
9 Treat the image as a single word in a circle.
10 Treat the image as a single character.
11 Sparse text. Find as much text as possible in no particular order.
12 Sparse text with OSD.
13 Raw line. Treat the image as a single text line bypassing hacks that are Tesseract-specific.

### OCR Engine Mode:
Pytesseract also supports different OCR Engine modes, which determine the underlying OCR engine to be used. Here are the available OCR Engine modes:
0 Legacy engine only.
1 Neural nets LSTM engine only.
2 Legacy + LSTM engines.
3 Default, based on what is available.

