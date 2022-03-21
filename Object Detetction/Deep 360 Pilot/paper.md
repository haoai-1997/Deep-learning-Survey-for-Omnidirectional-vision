## Deep 360 Pilot: Learning a Deep Agent for Piloting through 360◦ Sports Videos

- year: 2018

- dataset：  **(Sports-360 Dataset)** 

- abstract: To relieve the viewer from this “360 piloting” task, we propose “deep 360 pilot”–a deep learning-based agent for piloting through 360◦ sports videos automatically. At each frame, the agent observes a panoramic image and has the knowledge of previously selected viewing angles. The task of the agent is
to shift the current viewing angle (i.e. action) to the next
preferred one (i.e., goal).  Specifically, we leverage a state-of-the-art object detector to propose a few candidate objects of interest (yellow boxes in Fig. 1). Then, a recurrent neural network is used to select the main object (green dash boxes in Fig. 1). Given the main object and previously selected viewing angles, our method regresses a shift in viewing angle to move to the next one.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Deep360Pilot.png)

- Contributions:

(1) We develop the first human-like online agent for automatically navigating 360◦ videos for viewers. The online processing nature suits the agent for streaming videos and predicting views for foveated VR rendering. (2) We propose a jointly trainabl pipeline for learning the agent. Since the main object selection objective is non-differentiable, we employ a policy gradient technique to optimize the pipeline. 
(3) Our agent considers both viewing angle selection accuracy and transition smoothness. 
(4) We build the first 360◦ sports videos dataset to train and evaluate our “deep 360 pilot” agent.



- structure:

(1)a regression loss measuring the distance between the selected and ground truth viewing angles
(2)a smoothness loss encouraging smooth transition in viewing angle
(3) maximizing an expected reward of focusing on a foreground object

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Deep360PilotStructure.png)
- results：
metrics: **(Mean Overlap (MO) and Mean Velocity Difference (MVD))**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Deep360PilotResult1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Deep360PilotResult2.png)


- analysis: Our solution entails a new form of **(distillation)** across camera projection models. Compared to current practices for feature extraction on 360°images/video, spherical convolution benefits efficiency by avoiding performing multiple perspective projections, and it benefits accuracy by adapting kernels to the distortions in equirectangular projection.
