---
layout: page
title: Robotic Arm Block Sorting
description: A colored block sorting implementation using a YahBoom DofBot
img:
importance: 3
category: Coursework
---

To complete our goal of sorting blocks, we relied on hard-coded positions that the robot would need to pick and place blocks at [1]. This was done by using two predefined angle sets, one for the initial camera position for scanning block color (shown in Figure 1 below) and one for getting the gripper to each of the set locations. First, the robot will scan each location using the camera angle sets, iterating through all five spots and taking an image that would be used to detect a block and the block’s color at each location.
