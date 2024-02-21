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

0 Orientation and script detection (OSD) only. <br>
1 Automatic page segmentation with OSD. <br>
2 Automatic page segmentation, but no OSD, or OCR. <br>
3 Fully automatic page segmentation, but no OSD. (Default) <br>
4 Assume a single column of text of variable sizes. <br>
5 Assume a single uniform block of vertically aligned text. <br>
6 Assume a single uniform block of text. <br>
7 Treat the image as a single text line. <br>
8 Treat the image as a single word. <br>
9 Treat the image as a single word in a circle. <br>
10 Treat the image as a single character. <br>
11 Sparse text. Find as much text as possible in no particular order. <br>
12 Sparse text with OSD. <br>
13 Raw line. Treat the image as a single text line bypassing hacks that are Tesseract-specific. <br>

### OCR Engine Mode:
Pytesseract also supports different OCR Engine modes, which determine the underlying OCR engine to be used. Here are the available OCR Engine modes:
0 Legacy engine only. <br>
1 Neural nets LSTM engine only. <br>
2 Legacy + LSTM engines. <br>
3 Default, based on what is available. <br>

