# Fabric-Defect-Detection using OpenCV and Tkinter
This Python script utilizes OpenCV, NumPy, and Tkinter to create a simple graphical user interface (GUI) for fabric defect detection. The fabric defect detection algorithm is applied to an input image, and the results are displayed using Tkinter.

## Table of contents 
<br>Requirements  
<br>Defect Detection Algorithm
<br>File Selection
<br>Result Display

## Requirements
Python 3.x
<br>OpenCV (cv2)
<br>NumPy (numpy)
<br>Tkinter (tkinter)
<br>Pillow (PIL, Image, ImageTk)

## Defect Detection Algorithm 
The defect detection algorithm consists of the following steps:

<br>1.Read and copy the input image.
<br>2.Convert the image to the HSV color space.
<br>3.Apply blurring and denoising to enhance the image.
<br>4.Threshold the image to create a binary mask.
<br>5.Perform erosion and dilation operations on the binary mask.
<br>6.If the dilated mask contains defects (non-zero pixels), identify and draw contours around defective regions.
<br>7.Display the input image and the image with highlighted defective regions.

## File Selection
The script utilizes Tkinter to create a simple GUI with a "Browse Image" button. Clicking this button opens a file dialog, allowing the user to select an image file (supported formats: jpg, jpeg, png, bmp, gif).

## Result Display
After selecting an image, the script creates a new Tkinter window displaying the following:
 ### Input Image: The original input image is displayed in the window.
 ### Defective Regions: If defects are detected, the script highlights these regions in the image and displays the result.
<br>Note: The script assumes that a fabric is defective if the dilated binary mask has more than one non-zero pixel. The contours of defective regions are drawn in green.

