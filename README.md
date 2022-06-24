# <p align='center'>CannyEgdeDetection</p>

## Program:
```
Developed By:SARAN M
Register NUmber:212220230044
```

```python

import cv2
import numpy as np
import matplotlib.pyplot as plt

# Load the image, Convert to grayscale and remove noise
image1=cv2.imread ('username.jpg')
plt.subplot(1,2,1)
gray = cv2.cvtColor(image1, cv2.COLOR_BGR2GRAY)

plt.title('GRAY IMAGE')
plt.imshow(gray, cmap = 'gray') 

#canny edge detection
canny_edges = cv2.Canny(gray, 120, 150)
plt.subplot(1,2,2)
plt.imshow(canny_edges, cmap='gray')
plt.title('canny_edges')
plt.axis("off")
plt.show()

```
## Output:

![image](https://user-images.githubusercontent.com/75235427/175646445-ffcb6cf2-463c-4ec7-865c-d2673b59c849.png)
