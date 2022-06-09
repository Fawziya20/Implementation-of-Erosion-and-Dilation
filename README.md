# Implementation-of-Erosion-and-Dilation
## Aim
To implement Erosion and Dilation using Python and OpenCV.
## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages.
### Step2:
Create the Text using cv2.putText.
### Step3:
Create the structuring element.
### Step4:
Erode and Dilate the image.
### Step5:
End Program.
## Program:
``` Python
# Developed By   : Fawziya
# Register Number: 212220230017

# Import the necessary packages
import cv2
import numpy as np
import matplotlib.pyplot as plt

# Create the Text using cv2.putText
img1 = np.zeros((100,500), dtype = 'uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img1,'Jayashree Rao',(5,70), font, 2,(255),5,cv2.LINE_AA)
plt.imshow(img1,'gray')

# Create the structuring element
cv2.erode(img1, kernel)
kernel = cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))

# Erode the image
image_erode1 = cv2.erode(img1,kernel)
plt.imshow(image_erode1, 'gray')

# Dilate the image
image_dilate1 = cv2.dilate(img1, kernel)
plt.imshow(image_dilate1, 'gray')
```
## Output:
### Display the input Image

![image](https://user-images.githubusercontent.com/74660507/172183066-c7903036-896a-411a-81c2-a3ea03be541b.png)

### Display the Eroded Image

![image](https://user-images.githubusercontent.com/74660507/172183180-79e4aa5d-d57e-4c10-81f2-01d8636502b9.png)


### Display the Dilated Image

![image](https://user-images.githubusercontent.com/74660507/172183238-c967cebe-fbe3-47a7-aeb5-ed2153157e66.png)


## Result
Thus the generated text image is eroded and dilated using python and OpenCV.
