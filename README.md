import cv2
import numpy as np
img = cv2.imread('butterfly_2.jpeg')
dst = cv2.fastNlMeansDenoisingColored(img, None, 10, 10, 7,
15)
cv2.imshow("original img",img)
cv2.imshow("denoising_img", dst)
