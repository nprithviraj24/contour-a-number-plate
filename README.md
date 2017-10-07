# Contour a number plate.
Extract a number plate contour from a car image. This project is open and anyone can contribute!

##### Contour:  Outline of something. 

# Getting Started

So this project will give you a hands-on on major tasks done in image processing. I'll walk you through all the function which are used in the code. 

## Prerequisites
- Basic programming skills in python or any another language. This is written in python.
- OpenCV V.2.0+
- Python 2.7+ or Python 3.5+.

## Some of the additional libraries that are required: 
1. Numpy: Strictly for fast computations.
2. OS : for making command line calls.

### The functions used are from the the official [OpenCV Documentation](http://docs.opencv.org/2.4/modules/imgproc/doc/imgproc.html)

##### 1. cvtColor(x,y)
Used to convert one form an image to another form. [Official documentation](http://docs.opencv.org/2.4/modules/imgproc/doc/miscellaneous_transformations.html#cv.CvtColor).

##### 2. cv2.bilateralFilter
<strong>Why do we need filtering?</strong>
<br />
 For each pixel location (x,y) in the source image (normally, rectangular), its neighborhood is considered and used to compute the response. In case of a linear filter, it is a weighted sum of pixel values. In case of morphological operations, it is the minimum or maximum values, and so on. The computed response is stored in the destination image at the same location (x,y) . It means that the output image will be of the same size as the input image. Normally, the functions support multi-channel arrays, in which case every channel is processed independently. Therefore, the output image will also have the same number of channels as the input one.
 
 <strong>So why bilateralFilter?</strong>
 The function applies bilateral filtering to the input image, as described in [link](http://www.dai.ed.ac.uk/CVonline/LOCAL_COPIES/MANDUCHI1/Bilateral_Filtering.html). So, bilateralFilter can reduce unwanted noise very well while keeping edges fairly sharp. However, it is very slow compared to most filters.


# Author
~ Prithvi Raju
