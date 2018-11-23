---
layout: page
title:
tags: [research, satwik, kottur, cmu, graduate, iitb]
modified: 2014-08-08T20:53:07.573882-04:00
comments: false
---

### Human Activity Recognition

*B.Tech project-I, IIT Bombay, Fall 2013*  
Guide: Prof. Subhasis Chaudhuri  
[[Report](/reports/HumanActivity-Report.pdf)] [[Poster](HumanActivity-Poster.pdf)]  

The need for security and surveillance is always on the rise. This work is an attempt to address this problem in a social gathering using a single, calibrated camera. To begin with, it is a survey of existing methods&mdash;studying the advantages and suitability to the problem at hand. Next, a pipeline of approach is proposed similar to the work of Neha et al. in <b>[2]</b>. Finally, suitable improvements are suggested for the scenario considered.

<figure align="center">
    <a href="/images/human-pipeline.jpg"><img src="/images/human-pipeline.jpg"></a>
    <figcaption>Proposed Pipeline.</figcaption>
</figure><br/>

Human Activity is one of the most actively pursued topic owing to its wide range of applications. It has been studied mainly under two approaches&mdash;holistic and reductionist. The former considers the crowd as a single entity while the latter models individuals seperately and studies their interaction. <b>[1]</b> and <b>[2]</b> provide the respective examples. This work falls under the latter category.

<figure class="half">
    <a href="/images/human-dpm.jpg"><img src="/images/human-dpm.jpg"></a>
    <a href="/images/human-track.jpg"><img src="/images/human-track.jpg"></a>
    <figcaption>Results of DPM (left), tracking feature points (right).</figcaption>
</figure><br/>

Following a pipeline similar to <b>[2]</b>, frames from the calibrated camera are used to detect humans. Deformable part models (<b>[5]</b>) is employed for the first stage of detection. Due to high computation time, only intermittent frames are used to identify humans and corresponding parts. These detected parts form the feature points and are tracked by the Lucas-Kanade algorithm for remaining frames. This reduces the overall complexity and makes the execution real-time. The feature points on the image plane (2D) are converted to 3D points in world co-ordinates (classically known as 2.5D) using average height plane assumption. Finally, linear cylic pursuit model (LCP) is employed to predict the short-term trajectories of these points for further analysis. Finer details can be found in the report.

### References:
1. Viswanthan Srikrishnan and Subhasis Chaudhuri. Crowd motion analysis using linear cyclic pursuit.<i>In Pattern Recognition (ICPR), 2010 20th International Conference on, pages 3340–3343. IEEE, 2010.</i>
1. Neha Bhargava, Subhasis Chaudhuri and Guna Seetharaman. Linear cyclic pursuit based prediction of personal space violation in surveillance video. <i>Applied Imagery Pattern Recognition Workshop, 2013.</i>
1. Arpita Sinha. Multi-agent consensus using generalized cyclic pursuit strategies. 2009.
1. Carlo Tomasi and Takeo Kanade. Detection and tracking of point features. <i>International Journal of Computer Vision, 1991.</i>
1. P. F. Felzenszwalb, R. B. Girshick, D. McAllester, and D. Ramanan. Object detection with discriminatively trained part based models. <i>IEEE Transactions on Pattern Analysis and Machine Intelligence, 32(9):1627–1645, 2010.</i>
[[TOP](/research/projects/human-activity/)][[BACK](/research/#human-activity-recognition)]  
