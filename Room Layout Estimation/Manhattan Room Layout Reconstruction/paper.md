## Gaze360: Physically Unconstrained Gaze Estimation in the Wild

- year: 2020

- dataset：PanoContext dataset, Stanford 2D-3D.

- abstract: Recent approaches for predicting layouts from 360◦ panoramas produce excellent results. 
   These approaches build on a common framework consisting of three steps: a pre-processing step based on 
   edge-based alignment, prediction of layout elements, and a post-processing step by fitting a 3D layout to the layout elements. 
   Until now, it has been difficult to compare the methods due to multiple different design decisions, such as the encoding network, type of elements predicted, 
   or method of fitting the 3D layout. To address this challenge, we sum- marize and describe the common framework, 
   the variants, and the impact of the design decisions.


- Contributions:
(1) We introduce two frameworks, LayoutNet v2 and DuLaNet v2, which extend the corresponding state-of-the-art approaches of 3D Manhattan layout reconstruction from an RGB panoramic image.
(2) We conduct extensive experiments for LayoutNet v2, DuLa-Net v2 and another state-of-the-art approach, HorizonNet.
(3) We extend the Matterport3D dataset with general Manhattan layout annotations.

- structure: We propose a video-based gaze-tracking model using bidirectional Long Short-Term Memory capsules.In this paper, we utilize sequences of 7 frames to predict the gaze of the central frame. Note that other sequence lengths including a single central frame alone are also possible.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Gaze360structure.png)


- results：
metrics: **(the mean angular errors )**

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Gaze360result.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Gaze360result1.png)

- analysis: We presented a new temporal appearance-based gaze model using a novel loss function to estimate error quantiles. Finally we demonstrated the value of (i) our dataset via careful crossdataset performance comparison versus three existing 3D gaze datasets, and (ii) our model via application to unconstrained unseen imagery from YouTube videos.
