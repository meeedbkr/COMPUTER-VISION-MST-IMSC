Adaptive Thresholding using Otsu's Method
-----------------------------------------

This Python code applies adaptive thresholding using Otsu's method to an input image of a Sudoku puzzle. The code uses OpenCV library to perform image processing tasks.

### Dependencies

This code requires the following dependencies to be installed:

*   OpenCV (cv2)

### Usage

1.  Install the required dependencies
2.  Replace the file path in line 4 with the path to your input image
3.  Run the Python script
4.  The original image and the thresholded image will be displayed in separate windows
5.  Press any key to close the windows

### Description

The code performs the following steps:

1.  Loads the input image in grayscale
2.  Resizes the image to half of its original size using bilinear interpolation
3.  Applies Gaussian blur with a kernel size of 5x5 to remove noise
4.  Applies Otsu's thresholding method to binarize the image
5.  Displays the original image and the thresholded image in separate windows

### References

*   OpenCV Documentation: [cv2.threshold()](https://docs.opencv.org/4.5.3/d7/d4d/tutorial_py_thresholding.html)
*   Wikipedia: [Otsu's method](https://en.wikipedia.org/wiki/Otsu%27s_method)