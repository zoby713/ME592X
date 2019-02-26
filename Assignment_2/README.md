# Git Repository for M E 592X Homework 2 (Spring 2019)

**Theme Group: Robotics**

**Group Members:**
* Rahmat Adesunkanmi	- rahmatADE
* Brian Bates			- bkbates      
* Jacob Zobrist			- zoby713   
* Mehdi Saraeian		- MehdiSaraeian

## Problem Concept
This assignment was to take rgb-d data from a Microsoft Kinect, preprocess the
data and then package it for visualization in ROS.

The data comes from: [Technical University of Munich](https://vision.in.tum.de/data/datasets/rgbd-dataset/)

## Executing the Python scripts
The first script `1_AssociateFixed.py` is run from the command line

```
 python3.6 1_AssociateFixed.py rgb.txt depth.txt --max_difference=0.002
 ```

This chooses the two files with timestamps and data we want to associated, the RGB dataset and Depth dataset.
Because the timestamps in the data of the two datasets do not match exactly, the argument `max_difference` is
used to compare the differences in the timestamps for association.
