---
layout: page
title:
tags: [research, satwik, kottur, cmu, graduate, iitb]
modified: 2014-08-08T20:53:07.573882-04:00
comments: false
---

###Autonomous Underwater Vehicle (AUV-IITB)
*AUVSI and ONR's International Robosub Competition, San Diego, USA*  
*Vision (Spring 2012 - Spring 2013)*  
Guides: Dr. Hemendra Arya and Dr. Leena Vachhani  
[[Journal Paper (2012)](/reports/IIT_Bombay_Journal_Paper_2012.pdf)] [[Journal Paper (2013)](/reports/IIT_Bombay_Journal_Paper_2013.pdf)]  

Designing and developing an unmanned autonomous underwater vehicle (AUV) that localizes itself and performs realistic missions based on feedback from visual, inertial, acoustic and depth sensors using thrusters and pneumatic actuators. Matsya (sanskrit word for fish) is the AUV from IIT Bombay to participate in the International Robosub competition, San Diego which sees teams of different universities from countries all over the world.

<figure class="half">
    <a href="/images/auv-machine1.jpg"><img src="/images/auv-machine1.jpg"></a>
    <a href="/images/auv-machine2.jpg"><img src="/images/auv-machine2.jpg"></a>
    <figcaption>Matsya 2.0 (2013) (left), Matysa 1.0 (2012) (right).</figcaption>
</figure><br/>
<figure align="center">
    <a href="/images/auv-team.jpg"><img src="/images/auv-team.jpg"></a>
    <figcaption>Team (2013) at SSC Transdec, San Diego.</figcaption>
</figure><br/>


More information about the competition can be found [here](http://www.auvsifoundation.org/foundation/competitions/robosub/).
Details about the AUV IITB team are present [here](http://auv-iitb.org/).

Machine vision for Autonomous Underwater Vehicles poses three important challenges:

1. Degraded image quality due to the medium&mdash;Low visibility, color casting (blue or green), poor constrast, varying illuminations, brightness artifacts and blurring are of primary concern. Hence, pre-processing of images to correct these degradations is necessary to ensure robust detection in later stages of analysis.
1. Limited on-board computational capacity&mdash;Since the vehicle has a centralized processor and a plethora of sensors and other peripherals, power management is of utmost importance. Such a conservation lays a direct contraint on the amount of computing available for the current mission. This eliminates the scope for using processor-intensive techniques thereby increasing the challenge further.
1. Real-time requirement for navigation of the machine&mdash;The two on-board cameras are an importance source of feedback for the vehicle. For a reliable navigation and actuator control, detection algorithms have an additional condition of real-time execution.

To tackle the above problems, we devised adaptive identification and correction of color casts in images, edge-saliency based color segmentation and adaptive enhancement based on corrected color cast, amongst other techniques formulated after thorough literature survey.  

#### References:
1. Zuiderveld, Karel. Constrast Limited Adaptive Histogram Equalization.
1. P. Felzenszwalb, D. Huttenlocher. Efficient Graph-based Image Segmentation.
1. Finlayson, G.D., E. Trezzi. Shades of Gray and Color Constancy.
1. Cosmin Ancuti, Codruta Orniana Ancuti,Tom Haber, Philippe Bekaert. Enhancing underwater images and vides by fusion. *Computer Vision and Pattern Recognition (CVPR), 2012*  

[[TOP](/research/projects/auv-iitb/)][[BACK](/research/#autonomous-underwater-vehicle-auv-iitb)]  
