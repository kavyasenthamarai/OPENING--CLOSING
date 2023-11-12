# OPENING--CLOSING
## Aim
To implement Opening and Closing using Python and OpenCV.

## Software Required
1. Anaconda - Python 3.7
2. OpenCV
## Algorithm:
### Step1:
Import the necessary packages


### Step2:
Read the image

### Step3:
Create the structuring element

### Step4:
Use Opening operation

### Step5:
Use Closing Operation

### Step6:
Display all the output images

 
## Program:
```
Developed By: Kavya K
Register NO: 212222230065
```
``` Python
# Import the necessary packages
import cv2
import numpy as np



# Create the Text using cv2.putText
img= np.zeros((350,1400),dtype ='uint8')
font = cv2.FONT_HERSHEY_SIMPLEX
cv2.putText(img,'JEEVA ABISHAKE A',(15,200),font,5,(255),10,cv2.LINE_AA)
cv2.imshow('created_text',img)
cv2.waitKey(0)
cv2.destroyAllWindows()



# Create the structuring element
struct_ele= np.ones((9,9),np.uint8)



# Use Opening operation
opening = cv2.morphologyEx(img,cv2.MORPH_OPEN,struct_ele)
cv2.imshow('Opening',opening)
cv2.waitKey(0)
cv2.destroyAllWindows()




# Use Closing Operation
closing = cv2.morphologyEx(img,cv2.MORPH_CLOSE,struct_ele)
cv2.imshow('Closing',closing)
cv2.waitKey(0)
cv2.destroyAllWindows()




```
## Output:

### Display the input Image
![image](https://github.com/kavyasenthamarai/OPENING--CLOSING/assets/118668727/3276759b-21cb-4964-8248-5bfd4a4f47d5)

### Display the result of the Opening
![image](https://github.com/kavyasenthamarai/OPENING--CLOSING/assets/118668727/f1d0071e-ad4f-4eb2-a9e8-56f4eb8b4441)

### Display the result of Closing
![image](https://github.com/kavyasenthamarai/OPENING--CLOSING/assets/118668727/5ebc7238-97a3-461e-af4f-5feb66fe2bfc)

## Result
Thus the Opening and Closing operation is used in the image using python and OpenCV.
