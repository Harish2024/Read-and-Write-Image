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

```
# Developed By: harish
# Register Number: 212220230021

# To Read,display the image
import cv2
image=cv2.imread("levi.jpg")
cv2.imshow("image",image)
cv2.waitKey(0)

# To write the image
cv2.imwrite("image2.jpg", image)

# Find the shape of the Image
print(image.shape)

# To access rows and columns
for i in range(70,90):
for j in range(110,170):
image[i][j]=[0,0,0]
cv2.imshow("image",image)
cv2.waitKey(0)

# To cut and paste portion of image
image[70:90,110:175]=image[70:90,110:175]
cv2.imshow("image",image)
cv2.waitKey(0)
```

## Output:

### i) Read and display the image

![harish 1](https://user-images.githubusercontent.com/75246297/164192310-4ba4a4a3-1927-440a-846d-905f83489349.jpg)



### ii)Write the image

![harish 1](https://user-images.githubusercontent.com/75246297/164192367-f0bf45f5-e726-4bf2-aa29-edfeb3a9b63e.jpg)

### iii)Shape of the Image

![harish 1](https://user-images.githubusercontent.com/75246297/164192381-21947b45-0862-43c0-b5c3-9d2533a586e7.jpg)

### iv)Access rows and columns
![harish 2](https://user-images.githubusercontent.com/75246297/164192467-adbc667f-786b-4cc4-aa27-4cd15967db54.jpg)


### v)Cut and paste portion of image
![harish 3](https://user-images.githubusercontent.com/75246297/164192516-ec899181-534a-49ed-956f-38bcfdffb795.jpg)


Thus the images are read, displayed, and written successfully using the python program.


