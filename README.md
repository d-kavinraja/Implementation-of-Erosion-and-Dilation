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
# Import the necessary packages
# Developed : Kavinraja D
# Reg no : 212222240047
import cv2
import numpy as np
from matplotlib import pyplot as plt
# Load the image
img1=np.zeros((100,500),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX_SMALL

# Create the Text using cv2.putText

# Create the text using cv2.putText
cv2.putText(img1,'Kavinraja.D' ,(5,70),font,3.3,(255),5,cv2.LINE_AA)
plt.imshow(img1,cmap='gray')


# Create the structuring element

# Create the structuring element
kernel1=cv2.getStructuringElement(cv2.MORPH_CROSS,(7,7))


# Erode the image

# Erode the image
img_erode=cv2.erode(img1,kernel1)
plt.imshow(img_erode,cmap='gray')



# Dilate the image
# Dilate the image

img_dilate=cv2.dilate(img1,kernel1)
plt.imshow(img_dilate,cmap='gray')







```
## Output:

### Display the input Image

![output](./o1.png)
### Display the Eroded Image
![output](./o2.png)


### Display the Dilated Image

![output](./o3.png)

## Result
Thus the generated text image is eroded and dilated using python and OpenCV.