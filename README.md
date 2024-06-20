## Air Canvas Project
### A Computer Vision Project Implemented with OpenCV
Ever wanted to draw your imagination by just waving your finger in the air? In this project, we will create an Air Canvas that allows you to draw anything by capturing the motion of a colored marker with a camera. Here, a colored object at the tip of your finger serves as the marker.

We will use computer vision techniques with OpenCV to build this project. Python is the preferred language due to its extensive libraries and easy-to-use syntax. However, with an understanding of the basics, it can be implemented in any OpenCV-supported language.

This project leverages color detection and tracking to achieve its objectives. The color marker is detected, and a mask is produced. The mask is then processed with morphological operations such as erosion and dilation. Erosion reduces impurities in the mask, and dilation restores the main mask's eroded parts.

## Algorithm
Frame Reading and Color Conversion: Start by reading the frames and converting them to HSV color space, which is easier for color detection.
Canvas Preparation: Prepare the canvas frame and add the respective ink buttons.
Trackbar Adjustment: Adjust the trackbar values to find the mask for the colored marker.
Mask Preprocessing: Preprocess the mask with morphological operations like erosion and dilation.
Contour Detection: Detect contours, find the center coordinates of the largest contour, and store these coordinates in an array for successive frames. These arrays will be used for drawing points on the canvas.
Drawing: Finally, draw the points stored in the array on the frames and canvas.
Requirements
Python 3
NumPy
OpenCV
With these steps and requirements, you can build your Air Canvas and bring your imagination to life by simply waving your finger in the air.
