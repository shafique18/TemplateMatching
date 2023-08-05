# image Template Matching using python

## Beginner.ipynb

### Sklearn based fast, normalized cross-correlation in images
Here I have tried using Sklearn based fast, normalized cross-correlation method to match Template images with the new input image. 
This approach able to find almost all images separately differentiatied by rectangular red boxes.

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.18.52%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.26.14%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.26.20%20PM.png)


### ORB with BFMatcher based feature matching
Here I have tried to explore feature mapping approach using ORB and BFMatcher with cv.NORM_HAMMING and cv.NORM_L2 method available in python library 

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.28.55%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.29.06%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.26.49%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.26.59%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.27.07%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.27.18%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.27.28%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.27.37%20PM.png)


### SIFT with BFMatcher based fature matching
A feature mapping approach using SIFT and BFMatcher methods using sklearn

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.29.20%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.27.53%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.28.01%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.28.09%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.28.17%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.28.25%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.28.32%20PM.png)



### SIFT with FLANN based fature matching
A feature mapping approach using SIFT and FLANN methods

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.29.29%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.28.52%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.29.01%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.29.09%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.29.19%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.29.27%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.29.36%20PM.png)



### Multi scale template matching

Here all we need to do is apply a little trick:

Loop over the input image at multiple scales (i.e. make the input image progressively smaller and smaller).
Apply template matching using cv2.matchTemplate and keep track of the match with the 
largest correlation coefficient(along with the x, y-coordinates of the region with the largest correlation coefficient).
After looping over all scales, take the region with the largest correlation coefficient and use that as your “matched” region.

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.29.40%20PM.png) 
![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.29.48%20PM.png)
![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.29.56%20PM.png)
![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.30.15%20PM%201.png)
![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.30.28%20PM.png)
![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.30.47%20PM.png)
![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.30.54%20PM.png)


![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.29.45%20PM.png)
![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.29.53%20PM.png)
![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.30.31%20PM.png)

### Template matching with different available methods in CV2
There are six methods available in CV2.matchTemplate as 'cv2.TM_CCOEFF', 'cv2.TM_CCOEFF_NORMED', 'cv2.TM_CCORR','cv2.TM_CCORR_NORMED', 'cv2.TM_SQDIFF', 'cv2.TM_SQDIFF_NORMED'

cv2.TM_CCOEFF

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.31.03%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.31.02%20PM.png)

cv2.TM_CCOEFF_NORMED

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.31.10%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.31.02%20PM.png)

cv2.TM_CCORR

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.31.23%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.31.10%20PM.png)

cv2.TM_CCORR_NORMED

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.31.33%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.31.10%20PM.png)

cv2.TM_SQDIFF

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.31.46%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.31.17%20PM.png)

cv2.TM_SQDIFF_NORMED

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.32.49%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.31.02%20PM.png)

### Template matching using MTM package
Multi-Template-Matching is a python package to perform object-recognition in images using one or several smaller template images.
The main function MTM.matchTemplates returns the best predicted locations provided either a score_threshold and/or the expected number of objects in the image.

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.36.50%20PM.png)
![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.37.00%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.31.45%20PM.png)
![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.31.55%20PM.png)
![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.32.03%20PM.png)
![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.32.12%20PM.png)

### Scipy based correlation between image and template
Here I tried to find out cross correlate between two images. Cross-correlation is a measurement that tracks the movements of two or more sets of time series data relative to one another.

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%204.37.16%20PM.png)

![alt text](https://github.com/shafique18/TemplateMatching/blob/main/images/Screen%20Shot%202021-08-23%20at%205.32.51%20PM.png)
