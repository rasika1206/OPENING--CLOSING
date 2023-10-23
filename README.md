# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step 1 :
Import the necessary packages.

## Step 2 :
Create the Text using cv2.putText

### Step 3 :
Create the structuring element.

### Step 4 :
Use Opening operation.

### Step 5 :
Use Closing Operation.

## Program:
## DEVELOPED BY : RASIKA
## REGISTER NO : 212222230117
## Import the necessary packages :
```
import cv2
import numpy as np
import matplotlib.pyplot as plt
```
## Create the Text using cv2.putText :
```
img=np.zeros((100,400),dtype='uint8')
font=cv2.FONT_ITALIC
cv2.putText(img,'RASIKA',(5,70),font,2,(255),5,cv2.LINE_AA)
plt.axis('off')
plt.imshow(img)
plt.show()
```
## Create the structuring element :
```
kernel=cv2.getStructuringElement(cv2.MORPH_RECT,(9,9))
```
## Use Opening operation :
```
image_open=cv2.morphologyEx(img,cv2.MORPH_OPEN,kernel)
plt.axis('off')
plt.imshow(image_open)
plt.show()
```
## Use Closing Operation :
```
image_close=cv2.morphologyEx(img,cv2.MORPH_CLOSE,kernel)
plt.axis('off')
plt.imshow(image_close)
plt.show()
```
## Output :
## Display the input Image :
![Screenshot from 2023-10-14 16-03-27](https://github.com/rasika1206/OPENING--CLOSING/assets/124434806/13a12a29-3a43-4afc-86fb-e4dbbbff954d)


## Display the result of Opening :
![Screenshot from 2023-10-14 16-03-31](https://github.com/rasika1206/OPENING--CLOSING/assets/124434806/f111ce51-fccb-4041-a5d6-3cf1a2aa5cf4)


## Display the result of Closing :
![Screenshot from 2023-10-14 16-03-37](https://github.com/rasika1206/OPENING--CLOSING/assets/124434806/35336ef8-21f2-4209-a84d-328e38e8b300)


## Result :
Thus the Opening and Closing operation is used in the image using python and OpenCV.
