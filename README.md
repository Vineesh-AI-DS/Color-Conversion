# Color Conversion
## AIM
To perform the color conversion between RGB, BGR, HSV, and YCbCr color models.

## Software Required:
Anaconda - Python 3.7
## Algorithm:
### Step1:
Import cv2 and save and image as filename.jpg.
<br>

### Step2:
Use imread(filename, flags) to read the file.
<br>

### Step3:
Use cv2.cvtColor(src, code, dst, dstCn) to convert an image from one color space to another.
<br>

### Step4:
Split and merge the image using cv2.split and cv2.merge commands.

<br>

### Step5:
End the program and close the output image windows.
<br>

## Program:
```python
# Developed By:Vineesh.M
# Register Number:212221230122.
# i) Convert BGR and RGB to HSV and GRAY:
import cv2
sun_color_image = cv2.imread('img.jpg')
cv2.imshow('Original image', sun_color_image)
hsv_image = cv2.cvtColor(sun_color_image, cv2.COLOR_BGR2HSV)
cv2.imshow('BGR2HSV' ,hsv_image )
gray_image1 = cv2.cvtColor (sun_color_image, cv2.COLOR_RGB2GRAY)
cv2.imshow('RGB2GRAY', gray_image1)
cv2.waitKey(0)
cv2. destroyAllWindows()
```
``` python
# ii)Convert HSV to RGB and BGR:
import cv2
sun_color_image = cv2.imread('img.jpg')
cv2.imshow('Original image', sun_color_image)
hsv_image = cv2.cvtColor(sun_color_image, cv2.COLOR_HSV2RGB)
cv2.imshow('HSV2RGB' ,hsv_image )
gray_image1 = cv2.cvtColor (sun_color_image, cv2.COLOR_HSV2BGR)
cv2.imshow('HSV2BGR', gray_image1)
cv2.waitKey(0)
cv2. destroyAllWindows()
```
``` python
# iii)Convert RGB and BGR to YCrCb:
import cv2
sun_color_image = cv2.imread('img.jpg')
cv2.imshow('Original image', sun_color_image)
gray_image1 = cv2.cvtColor (sun_color_image, cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGB2YCrCb', gray_image1)
gray_image1 = cv2.cvtColor (sun_color_image, cv2.COLOR_BGR2YCrCb)
cv2.imshow('BGR2YCrCb', gray_image1)
cv2.waitKey(0)
cv2. destroyAllWindows()
```
``` python

# iv)Split and Merge RGB Image:
import cv2
sun_color_image = cv2.imread('img.jpg')
cv2.imshow('Original image', sun_color_image)
gray_image1 = cv2.cvtColor (sun_color_image, cv2.COLOR_RGB2YCrCb)
cv2.imshow('RGB2YCrCb', gray_image1)
gray_image1 = cv2.cvtColor (sun_color_image, cv2.COLOR_BGR2YCrCb)
cv2.imshow('BGR2YCrCb', gray_image1)
cv2.waitKey(0)
cv2. destroyAllWindows()
```
``` python

# v) Split and merge HSV Image:
import cv2
image = cv2.imread('image.jpg')
hsv = cv2.cvtColor(image, cv2.COLOR_BGR2HSV)
h,s,v = cv2.split(hsv)
cv2.imshow('Hue-Image',h)
cv2.imshow('Saturation-Image',s)
cv2.imshow('Gray-Image',v)
Merged_HSV = cv2.merge((h,s,v))
cv2.imshow('Merged HSV Image',Merged_HSV)
cv2.waitKey(0)
cv2.destoryAllWindows()

```
## Output:
### i) BGR and RGB to HSV and GRAY:

![Screenshot (96)](https://user-images.githubusercontent.com/93427254/163664023-aacda81c-2f29-4f9f-91f8-492194da5a77.png)

<br>

### ii) HSV to RGB and BGR:

![Screenshot (97)](https://user-images.githubusercontent.com/93427254/163664057-5f87ea22-a454-4643-8844-daa8407fc837.png)

<br>
<br>

### iii) RGB and BGR to YCrCb:

![Screenshot (98)](https://user-images.githubusercontent.com/93427254/163664065-4e4a62b2-cef6-4af6-be0f-88e1b73e93cf.png)

<br>
<br>

### iv) Split and merge RGB Image:

![Screenshot (99)](https://user-images.githubusercontent.com/93427254/163664082-4df8f626-75a3-4e6f-ab5d-f2ed43ee9216.png)

<br>
<br>

### v) Split and merge HSV Image:

![Screenshot (100)](https://user-images.githubusercontent.com/93427254/163664093-f45eac9b-c8db-44b2-8420-1b978b403ce3.png)
![Screenshot (101)](https://user-images.githubusercontent.com/93427254/163664097-0c4c7935-d374-493b-bd4f-c5f74001d8a9.png)

<br>
<br>


## Result:
Thus the color conversion was performed between RGB, HSV and YCbCr color models.
