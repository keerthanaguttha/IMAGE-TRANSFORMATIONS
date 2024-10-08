# Histogram-of-an-images
## Aim
To obtain a histogram for finding the frequency of pixels in an Image with pixel values ranging from 0 to 255. Also write the code using OpenCV to perform histogram equalization.

## Software Required:
Anaconda - Python 3.7

## Algorithm:
### Step1:
Read the gray and color image using imread()

### Step2:
Print the image using imshow().

### Step3:
Use calcHist() function to mark the image in graph frequency for gray and color image.

### step4:
Use calcHist() function to mark the image in graph frequency for gray and color image.

### Step5:
The Histogram of gray scale image and color image is shown.


## Program:
### Developed By: KEERTHANA G
### Register Number: 212223240045
### Input Grayscale Image and Color Image
## Gray Image:
```
import cv2
import matplotlib.pyplot as plt
image = cv2.imread('nebula.jpg')
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)
plt.imshow(gray_image, cmap='gray')
plt.title('Original Grayscale Image')
plt.axis('on')
```
![image](https://github.com/user-attachments/assets/6a051d09-ff63-4e76-bdfc-0785f662c70f)


### Histogram of Grayscale Image and any channel of Color Image
## Histrogram:
```p
plt.plot(hist_original, color='black')
plt.title('Original Histogram')
plt.xlim([0,256])
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/3a616cdd-3683-4afb-828b-f639e4cc9aa5)



### Histogram Equalization of Grayscale Image.

## Equalized Image:
```
equalized_image = cv2.equalizeHist(gray_image)
plt.imshow(equalized_image, cmap='gray')
plt.title('Equalized Image')
plt.axis('on')
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/2d0c2c37-25f1-4b10-8cbd-fd70ff6fc8e5)



## Histrogram:
```
plt.plot(hist_equalized, color='black')
plt.title('Equalized Histogram')
plt.xlim([0, 256])
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/07771e29-8cd4-42b4-bd5f-8acfca5cd4e6)


## Result: 
Thus the histogram for finding the frequency of pixels in an image with pixel values ranging from 0 to 255 is obtained. Also,histogram equalization is done for the gray scale image using OpenCV.
