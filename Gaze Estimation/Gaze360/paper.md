## Gaze360: Physically Unconstrained Gaze Estimation in the Wild

- year: 2021

- dataset：**(Columbia - high-resolution close-up faces; MPIIFaceGaze - faces captured by webcams; RTGENE - low-resolution faces using in-painting to mask out eye-tracking glasses; Gaze360 (Ours) - faces with varying resolution;)**  

- abstract: In this work, we present Gaze360, a large-scale gaze-tracking dataset and method for robust 3D gaze estimation in unconstrained images.  Our proposed 3D gaze model extends existing models to include temporal information and to directly output an estimate of gaze uncertainty.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Gaze360abstract.png)

- dataset:Our dataset consists of 238 subjects in indoor and outdoor environments with labelled 3D gaze across a wide range of head poses and distances. It is the largest publicly available dataset of its kind by both subject and variety, made possible by a simple and efficient collection method.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Gaze360dataset.png)

- Contributions:
1) we train a variety of 3D gaze estimation models on the dataset before converging on a final model which uniquely takes a multi-frame input (to help resolve single frame ambiguities) and employs a pinball regression loss for error quantile regression to provide an estimate of gaze uncertainty;
2) we demonstrate the usefulness of our dataset versus existing datasets by means of a cross-dataset model performance comparison (training on one dataset and testing on another), and introduce a simple method for self-supervised domain adaptation of gaze models;
3) finally we demonstrate how our Gaze360 model can be applied to real-world use cases, such as estimating a customer’s focus of attention in a supermarket.

- structure: We propose a video-based gaze-tracking model using bidirectional Long Short-Term Memory capsules.In this paper, we utilize sequences of 7 frames to predict the gaze of the central frame. Note that other sequence lengths including a single central frame alone are also possible.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Gaze360structure.png)


- results：
metrics: **(the mean angular errors )**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Gaze360result.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Gaze360result1.png)

- analysis: We presented a new temporal appearance-based gaze model using a novel loss function to estimate error quantiles. Finally we demonstrated the value of (i) our dataset via careful crossdataset performance comparison versus three existing 3D gaze datasets, and (ii) our model via application to unconstrained unseen imagery from YouTube videos.
