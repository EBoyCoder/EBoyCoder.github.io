---
layout: page
title: Robotic Arm Block Sorting
description: A colored block sorting implementation using a YahBoom DofBot
img:
importance: 3
category: Coursework
---

This project utilized a 5 degree of freedom robot arm with a wrist mounted camera to identify colored blocks and place them into a desired configuration. The code for this project was written in Python, utilizing the YahBoom Arm Device library to send commands and recieve servo readings and images from the hardware. The OpenCV library was used for the implementation of our computer vision processes, such as applying masks, finding contours, and determining colors. Inverse kinematics was utilized to determine the necessary joint angles to achieve good arm configurations for taking images and lifting the blocks. These configurations were then used to implement paths to achieve the desired block order.

<div class="row mt-3">
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="assets/video/IMG_9370_1.mp4" class="img-fluid rounded z-depth-1" controls=true autoplay=true %}
    </div>
</div>
<div class="caption">
    The Sorting Process, in Action!
</div>

<div class="row">
    <div class="col-sm mt-3 mt-md-0">
        {% include figure.liquid loading="eager" path="assets/img/cv2.png" title="Computer Vision Results Example" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
<div class="caption">
    In this image you can see the images taken by the wrist mounted camera, the identified regions of the images where the blocks are found, and the identified colors of the blocks in the order they are placed in the work space.
</div>
