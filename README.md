# TemplateMatching

## Beginner.ipynb || Expert.ipynb

### Sklearn based fast, normalized cross-correlation
Here I have tried using Sklearn based fast, normalized cross-correlation method to match Template images with test image. 
This approach able to find almost all images separately differentiatied by rectangular red boxes.


### ORB with BFMatcher based feature matching
Here I have tried to explore feature mapping approach using ORB and BFMatcher with cv.NORM_HAMMING and cv.NORM_L2 method


### SIFT with BFMatcher based fature matching
A feature mapping approach using SIFT and BFMatcher methods

### SIFT with FLANN based fature matching
A feature mapping approach using SIFT and FLANN methods

### Multi scale template matching

Here all we need to do is apply a little trick:

Loop over the input image at multiple scales (i.e. make the input image progressively smaller and smaller).
Apply template matching using cv2.matchTemplate and keep track of the match with the 
largest correlation coefficient(along with the x, y-coordinates of the region with the largest correlation coefficient).
After looping over all scales, take the region with the largest correlation coefficient and use that as your “matched” region.

### Template matching with different available methods in CV2
There are six methods available in CV2.matchTemplate as 'cv2.TM_CCOEFF', 'cv2.TM_CCOEFF_NORMED', 'cv2.TM_CCORR','cv2.TM_CCORR_NORMED', 'cv2.TM_SQDIFF', 'cv2.TM_SQDIFF_NORMED'

### Template matching using MTM package
Multi-Template-Matching is a python package to perform object-recognition in images using one or several smaller template images.
The main function MTM.matchTemplates returns the best predicted locations provided either a score_threshold and/or the expected number of objects in the image.

### Scipy based correlation between image and template
Here I tried to find out cross correlate between two images. Cross-correlation is a measurement that tracks the movements of two or more sets of time series data relative to one another.
