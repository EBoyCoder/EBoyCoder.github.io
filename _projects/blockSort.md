---
layout: page
title: Robotic Arm Block Sorting
description: A colored block sorting implementation using a YahBoom DofBot
img: assets/img/robotArm.png
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
    In the top left, you can see the identified colors of each position, in order from left to right looking at the mat while standing in front of the robot. It has correctly identified the order as being 'R','Y','  ','B','G'. The top right shows the identified area of the image in which the  block is present. The bottom left shows an example initial configuration, with the desired configuration being 'B','Y','  ','R','G'. The blocks already in their desired positions are marked with a green check, and the blocks not in their desired positions are marked with a red X. The bottom right shows joint angle sets used to take the images of the blocks in each respective location.
</div>
