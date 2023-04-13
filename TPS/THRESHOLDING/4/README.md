# Adaptive Thresholding with OpenCV
=================================

This script demonstrates how to apply adaptive thresholding to an image using OpenCV in Python. Adaptive thresholding is a technique used in image processing to binarize an image by choosing the threshold value based on the local pixel neighborhood.

## Getting Started
---------------

### Prerequisites

*   Python 3.x
*   OpenCV

### Installing

1.  Clone the repository:
    
    
2.  Install OpenCV:
    
    
    ```pip install opencv-python```
    

### Usage

1.  Place the image you want to process in the ```input``` folder.
    
2.  In the script, change the path to your image:
    
     ```img = cv2.imread('input/sudoku.png', cv2.IMREAD_GRAYSCALE)```
    
3.  Run the script:
    
    ```python adaptive_thresholding.py```
    
4.  The processed image will be displayed in a window titled "Adaptive Thresholding".
    

Acknowledgments
---------------

*   This script is based on the following OpenCV documentation: [https://docs.opencv.org/master/d7/d4d/tutorial\_py\_thresholding.html](https://docs.opencv.org/master/d7/d4d/tutorial_py_thresholding.html)

License
-------

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.