# Finding Lanes on Road

The goal of the project is to find lanes on Road using computer vision on either Image or Videos. 

# Tools used 

1. Numpy - Inbuilt python library used for mathematical operations. 
2. OpenCV - OpenCV is an open source computer vision and machine learning library which is mainly used in this project. more about opencv can be found at opencv.org
3. moviepy - moviepy is used to process video in the project. 

libraries can be installed by using the pip command 
> pip install numpy
> pip install moviepy
> pip install 
# Overview 

The project uses image data given as test and is processed by using various techniques such as  
Canny edge detection ,  Gaussian Blur, and Hough lines. 

1. Canney Edge :- 
  The Canny edge detector is an edge detection operator that uses a multi-stage algorithm to detect a wide range of edges in images 

2. Gaussian Blue :- 
  In image processing, a Gaussian blur (also known as Gaussian smoothing) is the result of blurring an image by a Gaussian function. 
  It is a widely used effect in graphics software, typically to reduce image noise and reduce detail.
3. Hough Lines :- 
  The Hough transform is a feature extraction technique used in image analysis, computer vision, and digital image processing.
  The purpose of the technique is to find imperfect instances of objects within a certain class of shapes by a voting procedure.
  This voting procedure is carried out in a parameter space,from which object candidates are obtained as local maxima in a so-called accumulator space that is explicitly constructed by the algorithm for computing the Hough transform
  In the project we define the region by calling the function and initializing the vertices or region.
# Plotting the Lines 

The most challenging segment of the project was to plot the lines through hough transformation for which we use the tehcnique of extrapolating the lines

first we would calculate the slope for right and left and comapre using the given parameters. 

after, which we would calculate each line and take the average slope of the biggest line. 

By using the average recieved from both the lines on the right and left we can extrapolate to the bottom and top of the lines.

# Input 






# Output 





#improvements 

Instead of using a linear technique to plot the lines we can use a ploynomial technique to plot the lines even through a curve which would help us achieve a good output and precise output.

Similarly , While trying to plot for a curved lane the line just goes out of bound and then returns back this is due to the parameters set at the beggining which could be set to taking the average and processing. 



