This project is a simple tool for interactively selecting a range of colors in an image using trackbars in the HSV color space. The code uses the OpenCV library to load the image, create the trackbars, and apply the selected range to the image.

To use this tool, run the code and load the image you want to select colors from. The trackbars will appear on the screen, allowing you to adjust the minimum and maximum values of the Hue, Saturation, and Value components of the HSV color space. The resulting mask and selected pixels will be displayed in real-time on the screen.

To exit the program, press the 'q' key.

Dependencies:

*   OpenCV
*   NumPy

To install OpenCV, run the following command:

Copy code

```pip install opencv-python```

To install NumPy, run the following command:

Copy code

```pip install numpy```