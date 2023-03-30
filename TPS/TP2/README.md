# Image Masking Example
This is an example of how to perform image masking using Python and OpenCV.
## Installation
To run this example, you will need to install the following packages:

1. numpy
1. opencv-python


You can install these packages using pip:
```
pip install numpy opencv-python

```
## Usage

1. Clone the repository to your local machine.

1. Navigate to the directory where the code is stored.
1. Update the __`url`__ variable in the code to point to the location of your input image.

1. Run the code using the following command:
```
python image_masking.py
```

1. The output image will be displayed on the screen.

## Code Description
This code performs image masking by creating a circular mask on the input image. The steps involved in this process are:


1. Read the input image using OpenCV's __`cv2.imread()`__ function.
1. Create a blank mask using numpy's __`np.zeros()`__ function, with the same dimensions as the input image.
1. Calculate the center of the image using the __`shape`__ attribute of the image array.
1. Draw a circle on the mask using the __`cv2.circle()`__ function.
1. Apply the mask to the input image using OpenCV's __`cv2.bitwise_and()`__ function.
1. Display the masked image on the screen using OpenCV's __`cv2.imshow()`__ function.

## Conclusion
Image masking is a useful technique for selecting specific areas of an image. This code provides a simple example of how to perform image masking using Python and OpenCV.