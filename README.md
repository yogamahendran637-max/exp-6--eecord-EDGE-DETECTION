

# NAME: YOGAMAHENDRAN G
# REG NO:212225040500


# Aim
To perform edge detection using Sobel, Roberts, Prewitt, Laplacian, and Canny edge detectors.

# Software Required
Anaconda – Python 3.7

Jupyter Notebook / VS Code

OpenCV (cv2)

NumPy

Matplotlib

# Algorithm
Step 1:

Import all the necessary modules for the program.

Step 2:

Load an image using cv2.imread().

Step 3:

Convert the image to grayscale.

Step 4:

Apply Sobel operator using OpenCV to detect edges.

Step 5:

Apply Prewitt operator using custom kernels.

Step 6:

Apply Roberts operator using custom kernels.

Step 7:

Apply Laplacian operator using OpenCV.

Step 8:

Apply Canny edge detector using OpenCV.

Step 9:

Display all edge-detected images for comparison

# Program:
```
import cv2
import numpy as np
import matplotlib.pyplot as plt

image = cv2.imread('nature.jpeg') 
gray_image = cv2.cvtColor(image, cv2.COLOR_BGR2GRAY)

plt.imshow(cv2.cvtColor(image, cv2.COLOR_BGR2RGB))
plt.title('Original Image')
plt.axis('off')

```
<img width="478" height="409" alt="1a83cfd9-405c-49d9-923f-70f40a430608" src="https://github.com/user-attachments/assets/163d83cc-609c-4927-baa2-4d560f209f4a" />

```
laplacian = cv2.Laplacian(gray_image, cv2.CV_64F)
plt.imshow(laplacian, cmap='gray')
plt.title('Laplacian Edge Detection')
plt.axis('off')

```

<img width="478" height="409" alt="ec6271ca-2c3b-48de-a8b1-4d49ab59a1e6" src="https://github.com/user-attachments/assets/3b374df4-4109-4ae8-8c3d-b0edd98f3e8d" />

```

canny_edges = cv2.Canny(gray_image, 50, 150)
plt.imshow(canny_edges, cmap='gray')
plt.title('Canny Edge Detection')
plt.axis('off')

```
<img width="478" height="409" alt="f40efbd5-91cc-4767-8c29-32f90f45fd09" src="https://github.com/user-attachments/assets/da87bedf-b772-4219-8a2d-cc436f0a8757" />

# RESULT:

Thus, edges are successfully detected using Sobel, Prewitt, Roberts, Laplacian, and Canny edge detection techniques. Each method highlights edges differently based on gradient and intensity variations, improving feature extraction and analysis.

























