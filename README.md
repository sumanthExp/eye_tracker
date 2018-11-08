# eye_tracker

This is based on an interesting paper "Eye Tracker for Everyone"
https://arxiv.org/abs/1606.05814

Dataset actually used in this paper is over 1400 students almost 2.5 million Frames. 
But for this project a smaller dataset 48,000 training samples and 5,000 validation samples is used. 
http://gazecapture.csail.mit.edu/

![alt text](https://github.com/Sumanthnr93/eye_tracker/blob/master/itracker_adv_arch.png)
Image source: https://arxiv.org/pdf/1606.05814.pdf

Overview of iTracker,  our eye tracking CNN. Inputs include left eye,  right eye,  and face images detected and cropped from the original frame (all of size 224×224). The face grid input is a binary mask used to indicate the location and size of the head within the frame (of size 25×25).  The output is the distance, in centimeters, from the camera.CONV represents convolutional layers (with filter size/number of kernels:\
CONV-E1,CONV-F1:11×11/96,\
CONV-E2,CONV-F2:5×5/256,\
CONV-E3,CONV-F3:3×3/384,\
CONV-E4,CONV-F4:1×1/64)\
FC represents fully-connected layers\
FC-E1: 128,\
FC-F1: 128,\
FC-F2: 64,\
FC-FG1: 256,\
FC-FG2: 128,\
FC1: 128,\
FC2: 2.\

This repository will be updated as the project progress 
