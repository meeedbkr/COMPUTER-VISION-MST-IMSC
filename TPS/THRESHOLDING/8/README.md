# OpenCV Thresholding Techniques Demo
===================================

This Python script demonstrates how to apply different thresholding techniques to frames captured from the default camera using the OpenCV library.

## Requirements
------------

*   Python 3
*   OpenCV library

## Usage
-----

1.  Install the OpenCV library using ```pip install opencv-python``` or ```pip install opencv-python-headless```
2.  Run the script using ``python thresholding_demo.py```
3.  The script will open a window showing the frames captured from the default camera and the thresholded frames using different thresholding techniques. Press the ```Esc``` key to exit the script.

## Explanation
-----------

1.  Import the necessary libraries:


```python
import cv2
```

2.  Create a list of window names for displaying the thresholded frames:


```python
windowNames = ['Binary', 'Binary Inv', 'Zero', 'Zero Inv', 'Trunc']
```

3.  Create a `VideoCapture` object to read frames from the default camera:


```python
cap = cv2.VideoCapture(0)
```

4.  Check if the camera is opened successfully and read a frame from the camera:


```python
if cap.isOpened():
    ret, frame = cap.read()
else:     
    ret = False
```

5.  Loop until the user presses the `Esc` key or the camera fails to read a frame:


```python
while ret:     
    ret, frame = cap.read()
```

6.  Set the threshold value and the maximum pixel value:


```python
th = 127 max_val = 255
```

7.  Apply different thresholding techniques to the frame:


```
ret, o1 = cv2.threshold(frame, th, max_val, cv2.THRESH_BINARY) 
ret, o2 = cv2.threshold(frame, th, max_val, cv2.THRESH_BINARY_INV) 
ret, o3 = cv2.threshold(frame, th, max_val, cv2.THRESH_TOZERO) 
ret, o4 = cv2.threshold(frame, th, max_val, cv2.THRESH_TOZERO_INV) 
ret, o5 = cv2.threshold(frame, th, max_val, cv2.THRESH_TRUNC)
```

8.  Display the thresholded frames in different windows:


```python
cv2.imshow(windowNames[0], o1) 
cv2.imshow(windowNames[1], o2) 
cv2.imshow(windowNames[2], o3) 
cv2.imshow(windowNames[3], o4) 
cv2.imshow(windowNames[4], o5)
```

9.  Wait for a key press event for 1 millisecond, and check if the `Esc` key was pressed:

```python
if cv2.waitKey(1) == 27:
    break
```

10.  Close all the windows and release the camera:


```python
cv2.destroyAllWindows()
cap.release()
```