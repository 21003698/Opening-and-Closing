# Opening-and-Closing

## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:

### Step1:
Import the necessary packages.

### Step2:
Create the Text using cv2.putText.

### Step3:
Use Opening operation.

### Step4:
Use Opening operation.

### Step5:
Use Closing Operation. 
 
## Program:

``` Python
### Developed By: Manoj Guna Sundar Tella.
### Register No: 212221240026.
# Import the necessary packages
import numpy as np
import cv2
import matplotlib.pyplot as plt
# Create the Text using cv2.putText
img1=np.zeros((100,500),dtype='uint8')
font=cv2.FONT_HERSHEY_COMPLEX_SMALL
im=cv2.putText(img1,'Sandeep',(5,70),font,2,(255),5,cv2.LINE_AA)
# Create the structuring element
Kernel=cv2.getStructuringElement(cv2.MORPH_CROSS,(11,11))
# Use Opening operation
image1=cv2.morphologyEx(im,cv2.MORPH_OPEN,Kernel)
plt.imshow(image1)
# Use Closing Operation
image1=cv2.morphologyEx(im,cv2.MORPH_CLOSE,Kernel)
plt.imshow(image1)









```
## Output:

### Display the input Image
<img width="376" alt="sandoo" src="https://user-images.githubusercontent.com/93427522/175764575-3a1d4186-8a94-4023-ab21-554fe4cffc37.png">




### Display the result of Opening
<img width="376" alt="sandoo1" src="https://user-images.githubusercontent.com/93427522/175764586-0a9530eb-d027-42d0-9791-010f5c5efece.png">


### Display the result of Closing
<img width="376" alt="sandoo2" src="https://user-images.githubusercontent.com/93427522/175764591-18eaadd0-51ce-4f07-b7df-a86c6c3f3265.png">


## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
