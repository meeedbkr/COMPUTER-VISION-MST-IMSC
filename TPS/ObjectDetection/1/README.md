Object Detection using OpenCV
=============================

This code uses OpenCV to detect objects in an image based on their color. It converts the image from the BGR color space to the HSV color space, creates a mask for the specified color range, and gets the bounding box of the detected object. If an object is detected, a green rectangle is drawn around it.

Getting Started
---------------

To run this code, you will need Python 3 and OpenCV installed on your machine. You can install OpenCV using pip:


```pip install opencv-python```

You will also need to provide an image file to be analyzed. Replace "examples/4.jpg" in the code with the path to your image file.

Running the Code
----------------

Once you have Python and OpenCV installed, you can run the code by running the following command in your terminal or command prompt:


```python object_detection.py```

Configurations
--------------

You can adjust the color range for object detection by modifying the ```lower_limit``` and ```upper_limit``` arrays. The values in these arrays correspond to the lower and upper limits of the HSV color space, respectively.

Constants
---------

To make it easier to adjust settings without modifying the main code, you can create a separate file for constants or configurations. Here's an example:


```import numpy as np  # Color range for object detection LOWER_LIMIT = np.array([75, 0, 99]) UPPER_LIMIT = np.array([179, 62, 255])```

With these changes, your code will be more organized and easier to use for other developers.