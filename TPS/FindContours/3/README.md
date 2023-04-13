# Contour detection in an image using OpenCV
==========================================

This is a Python script that detects and draws contours in an image using OpenCV library. The script performs the following operations:

1.  Load an image using ```cv2.imread()```
2.  Convert the image to grayscale using ```cv2.cvtColor()```
3.  Apply thresholding using ```cv2.threshold()```
4.  Find contours in the thresholded image using ```cv2.findContours()```
5.  Draw the contours on the original image using ```cv2.drawContours()```
6.  Display the image with the drawn contours using ```cv2.imshow()```

Prerequisites
-------------

*   Python 3.x
*   OpenCV library
*   An image file to perform contour detection on

Usage
-----

1.  Clone the repository or download the script file
2.  Install OpenCV library using ```pip install opencv-python``` if not already installed
3.  Place the image file in the same directory as the script file
4.  Run the script using ```python <script_file_name>.py```
5.  The script will display the original image with the drawn contours

Example
-------

An example image ```5.jpg``` is provided in the repository to test the script. The output of the script with the example image will show the contours detected in the image.