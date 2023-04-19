1.  Import necessary modules:


```import cv2 import numpy as np import os```

2.  Define a function to get the HSV values from the trackbar:


```def get_hsv_values(val):     pass```

This function is called whenever the trackbar value changes, but we don't need to do anything with it yet.

3.  Create a window to display the frame:


```cv2.namedWindow('frame')```

4.  Create trackbars for Hue, Saturation, and Value:


```cv2.createTrackbar('H min', 'frame', 0, 179, get_hsv_values) cv2.createTrackbar('H max', 'frame', 179, 179, get_hsv_values) cv2.createTrackbar('S min', 'frame', 0, 255, get_hsv_values) cv2.createTrackbar('S max', 'frame', 255, 255, get_hsv_values) cv2.createTrackbar('V min', 'frame', 0, 255, get_hsv_values) cv2.createTrackbar('V max', 'frame', 255, 255, get_hsv_values)```

The initial values for Hue are 0 and 179 because that covers the entire range. The initial values for Saturation and Value are 0 and 255 because those are the maximum values.

5.  Open the default camera (webcam):


```cap = cv2.VideoCapture(0)```

6.  Start an infinite loop:


```while True:```

7.  Capture a frame from the camera:


```ret, frame = cap.read()```

8.  Convert the frame to HSV (Hue, Saturation, Value) color space:


```hsv_frame = cv2.cvtColor(frame, cv2.COLOR_BGR2HSV)```

9.  Get the current HSV values from the trackbars:


```h_min = cv2.getTrackbarPos('H min', 'frame') h_max = cv2.getTrackbarPos('H max', 'frame') s_min = cv2.getTrackbarPos('S min', 'frame') s_max = cv2.getTrackbarPos('S max', 'frame') v_min = cv2.getTrackbarPos('V min', 'frame') v_max = cv2.getTrackbarPos('V max', 'frame')```

10.  Set the lower and upper HSV limits for the specified color range:


```lower_limit = np.array([h_min, s_min, v_min]) upper_limit = np.array([h_max, s_max, v_max])```

11.  Create a mask for the specified color range:


```mask = cv2.inRange(hsv_frame, lower_limit, upper_limit)```

12.  Apply the mask to the original frame to get the result:


```result = cv2.bitwise_and(frame, frame, mask=mask)```

13.  Show the original frame, the mask, and the result:


```cv2.imshow("original", frame) cv2.imshow("mask", mask) cv2.imshow('result', result)```

14.  Exit the loop if 'q' is pressed:


```if cv2.waitKey(1) & 0xFF == ord('q'):     break```

15.  Release the resources and close the window:


```cap.release() cv2.destroyAllWindows()```