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
### Developed By: S.SAFA
### Register Number: 212220230040
i) #To Read,display the image
```
import cv2
color_image=cv2.imread('lol.jpg',1)
cv2.imshow('colorimage',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()

```
ii) #To write the image
```
cv2.imwrite('sky.jpg',color_image)
cv2.imshow('sky Image',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()



```
iii) #Find the shape of the Image
```
import cv2
color_image=cv2.imread('lol.jpg',-1)
print(color_image.shape)



```
iv) #To access rows and columns

```
import cv2
import random
color_img=cv2.imread('lol.jpg',1)
for i in range(100):
    for j in range(color_img.shape[1]):
        color_img[i][j]=[random.randint(0,255),random.randint(0,255),random.randint(0,255)]
        cv2.imshow('212220230040, S.SAFA',color_img)
cv2.waitKey(0)
cv2.destroyAllWindows()



```
v) #To cut and paste portion of image
```
import cv2
color_image=cv2.imread('lol.jpg',1)
cut=color_image[260:280,100:300]
color_image[60:80,100:300]=cut
cv2.imshow('cutimage',color_image)
cv2.waitKey(0)
cv2.destroyAllWindows()



```

## Output:

### i) Read and display the image

![DI-EXP1 A](https://user-images.githubusercontent.com/75234912/161386777-5b45acaf-318a-4b5b-aa7c-2880864a9e0f.png)


### ii)Write the image
![DI-EXP1 B](https://user-images.githubusercontent.com/75234912/161386784-35e6a405-2aec-4c95-af2f-22b4521b169b.png)



### iii)Shape of the Image
![shape](https://user-images.githubusercontent.com/75234912/161386791-54b030e8-e804-4d08-8587-7425ef1a9dfd.png)



### iv)Access rows and columns

![DI-EXP1 C](https://user-images.githubusercontent.com/75234912/161386803-3ae38161-f460-4ce1-8db8-6d25f56b04ba.png)

### v)Cut and paste portion of image
![cut image](https://user-images.githubusercontent.com/75234912/161386818-316a5331-b88e-4550-aeac-114b0685568c.png)


## Result:
Thus the images are read, displayed, and written successfully using the python program.


