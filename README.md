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

```python

# Developed By: Vijayaragavan ARR
# Register Number: 212220230059

# To Read,display the image

import cv2
image_1=cv2.imread("pic_1.PNG")
image_2=cv2.imread("pic_2.PNG")
cv2.imshow("pic_1",image_1)
cv2.waitKey(0)
cv2.imshow("pic_2",image_2)
cv2.waitKey(0)

# To write the image

cv2.imwrite("pic_1",image_1)
cv2.imwrite("pic_2",image_2)

# Find the shape of the Image

print(image_1.shape)
print(image_2.shape)

# To access rows and columns

for i in range(70,90):
    for j in range(110,170):
        image_2[i][j]=[0,0,0]
cv2.imshow("pic_2",image_2)
cv2.waitKey(0)

# To cut and paste portion of image

image_2[70:90,110:175]=image_1[70:90,110:175]
cv2.imshow("pic_2",image_2)
cv2.waitKey(0)

```

## Output:

### i) Read and display the image

<br>

![Screenshot (6)](https://user-images.githubusercontent.com/75235488/160637901-41bf4705-0fa6-4d32-a1ab-71e4b7c1c774.png)

![Screenshot (7)](https://user-images.githubusercontent.com/75235488/160637970-e3c1659a-f887-49c3-b7e5-b9850f81e8b2.png)

<br>

### ii)Write the image

<br>

![Screenshot (8)](https://user-images.githubusercontent.com/75235488/160638028-5e4fc52c-ad38-4694-a9c3-04043ae14617.png)

<br>

### iii)Shape of the Image

![Screenshot (11)](https://user-images.githubusercontent.com/75235488/160641197-e200baae-3551-45c7-93f0-6921505f957e.png)



### iv)Access rows and columns
<br>

![Screenshot (9)](https://user-images.githubusercontent.com/75235488/160638115-4acf9beb-7255-42c9-a143-727854cb645f.png)

<br>

### v)Cut and paste portion of image
<br>

![Screenshot (10)](https://user-images.githubusercontent.com/75235488/160638181-59eb9a91-783d-4eb5-bd88-02f06f2c8b0f.png)

<br>

## Result:
Thus the images are read, displayed, and written successfully using the python program.

