Object Detection in Video Stream
--------------------------------

This Python script uses OpenCV library to detect a specific color object in a video stream and draw a bounding box around it. The detected object is based on the HSV color space, and the lower and upper limits of the color range can be adjusted according to the user's preferences.

### Dependencies

To run this script, you need to have the following dependencies installed on your machine:

*   Python 3.x
*   NumPy
*   OpenCV

### Installation

You can install the dependencies using the following commands in the terminal:

Copy code

```pip install numpy pip install opencv-python```

### Usage

To use this script, follow these steps:

1.  Clone the repository to your local machine.
2.  Open the script in a Python IDE or Jupyter Notebook.
3.  Change the path to your video file in the ```cap = cv2.VideoCapture()``` line.
4.  Adjust the lower and upper limits of the color range in the ```lower_limit``` and ```upper_limit``` variables respectively.
5.  Run the script.

The processed video with the bounding box around the detected object will be saved in the ```out.mp4``` file.

### Credits

This script was created by \[Meeedbkr\] and is based on the OpenCV library.