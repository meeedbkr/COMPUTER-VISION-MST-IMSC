# Bitwise Operations
This script performs various bitwise operations on two images - a square and a circle - using OpenCV.

## Requirements
In order to run this script, you will need the following:
<ul>
<li>Python 3</li>
<li>NumPy</li>
<li>OpenCV</li>
</ul>
## Usage
<ol>
<li>Clone the repository or download the script file.</li>

<li>Open a terminal or command prompt window and navigate to the directory containing the script.</li>

<li>Run the script using the following command:
	'''
	python bitwise_operations.py
	'''
</li>
<li>
	The script will display the following images, each showing the result of a different bitwise operation:
	<ul>
		<li>A 300x300 black square with a white border</li>
		<li>A 300x300 black circle filled with white</li>
		<li>The result of the "AND" operation on the square and circle</li>
		<li>The result of the "OR" operation on the square and circle</li>
		<li>The result of the "XOR" operation on the square and circle</li>
		<li>The result of the "NOT" operation on the circle</li>
	</ul>
</li>
</ol>
## Notes
<ul>
<li>The script uses only one integer value for the `color` variable when drawing the square. This is because the rectangle function in OpenCV expects a single value for the color argument when drawing a solid shape.
</li>
<li>The script also includes an example of using truthy and falsy values in Python.
</li>
<li>The images will be displayed using OpenCV's `imshow` function, and will not be saved to disk. You can close each image window by pressing any key.


</li>
</ul>