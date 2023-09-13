# READ AND WRITE AN IMAGE
## AIM
To write a python program using OpenCV to do the following image manipulations.
i) Read, display, and write an image.
ii) Access the rows and columns in an image.
iii) Cut and paste a small portion of the image.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Choose an image and save it as a filename.jpg
### Step2:
Use imread(filename, flags) to read the file.
### Step3:
Use imshow(window_name, image) to display the image.
### Step4:
Use imwrite(filename, image) to write the image.
### Step5:
End the program and close the output image windows.
## Program:
### Developed By:JEEVITHA E
### Register Number: 212222230054
i) #To Read,display the image
```
import cv2
color_image=cv2.imread('rose.jpg',1)
cv2.imshow('212222230054_JEEVITHA',color_image)
cv2.waitKey(0)


```
ii) #To write the image
```
import cv2
img = cv2.imread('waterb.jpg', 1)
new_img = cv2.imwrite('rose.jpg', img)
cv2.imshow('212222230054_JEEVITHA', img)
cv2.waitKey(0)



```
iii) #Find the shape of the Image
```python3

import cv2
img = cv2.imread('rose.jpg', 1)
print(img.shape)


```
iv) #To access rows and columns

```python3
import cv2
import random
img = cv2.imread('rose.jpg', 1)
for i in range(100):
    for j in range(img.shape[1]):
        img[i][j] = [random.randint(0, 255), random.randint(0, 255), random.randint(0, 255)]
cv2.imshow('part image', img)
cv2.waitKey(0)
cv2.destroyAllWindows()


```
v) #To cut and paste portion of image
```python3

import cv2
img = cv2.imread('rose.jpg', 1)
tag = img[200:400, 200:400]
img[100:300,100:300] = tag
cv2.imshow('212222230054_jeevitha', img)
cv2.waitKey(0)


```

## Output:

### i) Read and display the image


![WhatsApp Image 2023-09-13 at 17 16 29](https://github.com/Jeevithaelumalai/READ-AND-WRITE-IMAGE/assets/118708245/ff30abab-3f5b-4c20-a6c3-73a6f4e5bb3b)



### ii)Write the image


![WhatsApp Image 2023-09-13 at 17 16 29](https://github.com/Jeevithaelumalai/READ-AND-WRITE-IMAGE/assets/118708245/4e84300b-6aac-4b67-9478-4e08ec9a1e0a)


### iii)Shape of the Image

![WhatsApp Image 2023-09-13 at 17 16 29](https://github.com/Jeevithaelumalai/READ-AND-WRITE-IMAGE/assets/118708245/81ab1fe3-e1fb-4cf2-bdaf-c19de81f451f)


### iv)Access rows and columns

![WhatsApp Image 2023-09-13 at 17 15 26](https://github.com/Jeevithaelumalai/READ-AND-WRITE-IMAGE/assets/118708245/16be4ef7-3ecc-4ad2-905d-e5f47481cd01)



### v)Cut and paste portion of image

![WhatsApp Image 2023-09-13 at 20 51 59](https://github.com/Jeevithaelumalai/READ-AND-WRITE-IMAGE/assets/118708245/f9c82e24-9332-4a58-85c0-a6c49e18c1e4)




## Result:
Thus the images are read, displayed, and written successfully using the python program.
