# Liquid Level Detection Notebook

This notebook is designed for computer vision image analysis, focusing on edge detection, region masking, and contour detection. It utilizes various Python libraries and implements specific algorithms for image processing.

## Dependencies

- numpy
- skimage
- scipy
- cv2 (OpenCV)
- matplotlib
- urllib
- sklearn

## Notebook Structure

### Import Dependencies

Import necessary Python libraries for image processing and computer vision tasks.

### Function to Read Images from Web Addresses

Defines `url_to_image` function to convert images from web URLs to RGB format using OpenCV.

### Function to Mask Region of Interest

Includes `mask_img` function to apply a mask to a specified region of an image, useful for focusing on particular areas.

### Read in Test Image

Demonstrates how to read an image from a web URL for processing.

### Step 1: Convert the Image to Grayscale and Apply Gaussian Blur

Converts the image to grayscale and applies Gaussian blur to reduce noise, preparing it for edge detection.

### Step 2: Apply Canny Algorithm

Implements the Canny edge detection algorithm to highlight edges in the image.

### Step 3: Detect Contours

Finds and plots contours based on the edges detected in the previous step.

### Step 4: Set a Fill Level Threshold

Sets a threshold level to identify specific regions in the image (e.g., liquid level in a bottle).

### Step 5: Mask the Region of Interest

Masks specific regions in the image, focusing on areas of interest (e.g., individual bottles).

### Step 6: Apply Hough Transform to Find Lines

Uses the Hough Transform to find straight lines in the masked regions, useful for identifying linear features.

### Display the Image with the Status of Each Bottle

Adds status text to the image to indicate the analysis result of each region (e.g., pass/fail status based on fill level).

## Usage

This notebook is designed for users with a basic understanding of Python and computer vision concepts. It can be modified to suit different image analysis needs, particularly in areas like object detection, region of interest analysis, and feature extraction.
