---
layout: page
title:
tags: [research, satwik, kottur, cmu, graduate, iitb]
modified: 2014-08-08T20:53:07.573882-04:00
comments: false
---

### Static Vehicle Detection and Analysis in Aerial Imagery using Depth

*Internship at [IRIS](http://iris.usc.edu/iris.html), University of Southern California, Summer 2013*  
Guide: Prof. Gerard Medioni  
[[Report](/reports/VehicleDetection-Report.pdf)] [[Poster](/reports/VehicleDetection-Poster.pdf)]  

Vehicle detection and identification in urban scenarios has many civilian, security and surveillance application. 
The easy availability of aerial images along with its advantage of spanning wide areas due to large field of view, makes the problem of such identification in aerial images interesting. 
Primarily, this work proposes a detection algorithm using depth information for identification of static vehicles, particularly in parking lots. 
The scene depth is obtained from Digital Surface Model (DSM) of the urban landscape. 
Finally, the dependence of performance on the 3D model parameters is analyzed.

<figure class="half">
    <a href="/images/vehicle-orig-image.jpg"><img src="/images/vehicle-orig-image.jpg"></a>
    <a href="/images/vehicle-detect-image.jpg"><img src="/images/vehicle-detect-image.jpg"></a>
    <figcaption>Original aerial image (left), detections based on depth (right).</figcaption>
</figure><br/>

From the approaches proposed by various researchers in the community, **[1, 2, 3, 4]** are closely related to the current work.
**[1]** provides the 3D model of the landscape used in the proposed algorithm. 
Depth features have been explored for vehicle identification by B. Yang et al. in **[2]**. However, **[2]** uses LIDAR data unlike **[1]** which uses stream of aerial images for estimating scene depth.  

In this work, depth features are obtained from **[1]**, which itself is a novel technique to simultaneously solve for camera positions and dense depth estimation. For a given image, height is backprojected onto it using the 3D model. Haar-like features are used for a small portion of the image using sliding window, to estimate the presence or absence of a vehicle. In order to improve the accuracy, validation is incorporated using the edge-saliency of wire frame model as proposed in <b>[4]</b>. To understand the behavior of the system better, analysis of the performance is performed by varying the parameters of optical flow (regularization term, number of iterations, etc.) used in 3D model generation. A high negative correlation between the regularization term and accuracy of the system can be clearly concluded. This analysis can be used to better the overall system thereby an indicative of the scope for improvement.

### References:

1. Zhouliang Kang, Gerard Medioni. 3D Urban Reconstruction from Wide Area Aerial Surveillance Video. *Workshop on Applications for Aerial Video Exploitation (WAVE), 2015*.
[[Paper](http://www-scf.usc.edu/~zkang/wave2015.pdf)]
1. Bo Yang, Pramod Sharma, Ram Nevatia. Vehicle Detection from Low Quality Aerial LIDAR Data. [[Paper](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.309.8325)]
1. Y. Lin H. Liao and G. Medioni. Aerial 3D reconstruction with line-constrained dynamic programming. <i>In ICCV,2011.</i> [[Paper](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.309.9111)]
1. Stefan Hinz. Integrating local and global features for vehicle detection in high resolution aerial imagery. <i>ISPRS Archives,2003, XXXIV(3/W8)</i> [[Paper](http://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.97.7312)]  
  
[[TOP](/research/projects/aerial-vehicle/)][[BACK](/research/#static-vehicle-detection-and-analysis-in-aerial-imagery-using-depth)]  
