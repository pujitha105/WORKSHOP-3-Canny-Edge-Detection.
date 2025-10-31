## Canny-edge-detection
Overview
This project demonstrates Canny edge detection on an image using normal (average) blur instead of Gaussian blur. The program reads an image, applies blur to reduce noise, calculates thresholds based on median intensity, and detects edges.

## Instructions to Run

## 1. Install Dependencies
Make sure you have Python 3 installed. Then install the required libraries:

OpenCV: For image processing

Matplotlib: For displaying images

NumPy: For numerical calculations

Use the following commands:

pip install opencv-python matplotlib numpy

## 2. Prepare the Image
Place your image (e.g., images.jpeg) in the project folder or specify the full path.

Make sure the filename matches exactly, including the extension.

## 3. Image Reading
Read the image from disk.

Check that the image loads successfully. If not, ensure the file path is correct.

## 4. Display Original Image
Convert the image to the correct color format for displaying with Matplotlib.

Show the original image before processing.

## 5. Apply Normal (Average) Blur
Use a 3x3 kernel to smooth the image and reduce noise.

This helps prevent detecting too many false edges.

## 6. Calculate Dynamic Thresholds
Compute the median intensity of the original image.

Set the low threshold as a fraction of the median.

Set the high threshold as another fraction of the median.

These thresholds control which edges are detected.

## 7. Apply Canny Edge Detection
Use the blurred image and the computed thresholds to detect edges.

The result is a black-and-white image where white lines represent detected edges.

## 8. Display Edge-Detected Image
Show the resulting image using Matplotlib with a grayscale colormap.

Compare it visually with the original image to see the detected edges.

9. Notes on Parameters
Kernel size (blur): Larger → smoother, fewer edges; Smaller → more edges, possibly noisy.

Thresholds: Lower → more sensitive, detects weak edges; Higher → detects only strong edges.

Image quality: High-resolution images may require larger kernel or adjusted thresholds.
