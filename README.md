# contour-detection-opencv
 Detecting character contours in an image using OpenCV, excluding background shapes like bounding boxes.
Contour Detection with OpenCV

This project demonstrates contour detection in an image using OpenCV, specifically designed to detect individual characters while excluding any non-character contours such as bounding boxes or frames.

Problem Statement

The given image contains a large number of characters enclosed within a rectangular box. The objective is to detect contours corresponding only to the characters and ignore the contour of the rectangular frame.

Solution Overview

This notebook performs the following steps:

Loads the input image using a relative path.

Converts the image to grayscale and applies thresholding to prepare for contour detection.

Uses OpenCV's contour detection functions to find all contours in the image.

Sorts the detected contours by area and removes the largest one (which corresponds to the bounding box).

Draws the remaining contours (characters) and displays or saves the output.

Key Features

Implemented using OpenCV

Filters out unwanted contour (bounding box)

Uses relative file paths for portability

Includes comments for key steps in the code

Project Structure

contour-detection-opencv/

ContourDetection.ipynb : Jupyter Notebook with the full implementation

fig1.jpg : Input image

result.png : Output image with character contours highlighted

requirements.txt : Required libraries

README.md : Project description and instructions

Requirements

Python 3.x

numpy

opencv-python

matplotlib (optional for plotting)
