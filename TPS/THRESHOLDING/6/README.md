# Image Thresholding using Otsu's Method
--------------------------------------

This Python code demonstrates the use of Otsu's thresholding method to segment an image into foreground and background regions.

### Requirements

This code requires the following Python libraries to be installed:

*   OpenCV (cv2)

### Usage

1.  Install the required libraries.
2.  Place the input image in the directory where the code is located.
3.  Update the path to the input image in the ```cv2.imread()``` function.
4.  Run the script to obtain the thresholded image.
5.  Press any key to close the image windows.

### Description

The script reads a grayscale image from file using the OpenCV library. It then resizes the image to half its original size using bilinear interpolation. Otsu's thresholding method is applied to the image to separate the foreground from the background. The thresholded image is displayed in a separate window, along with the original image.

### References

*   Nobuyuki Otsu, "A threshold selection method from gray-level histograms," IEEE Transactions on Systems, Man, and Cybernetics, vol. 9, no. 1, pp. 62-66, Jan. 1979.
*   OpenCV documentation: [https://docs.opencv.org/](https://docs.opencv.org/)