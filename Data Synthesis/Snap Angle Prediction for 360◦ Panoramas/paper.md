## Snap Angle Prediction for 360◦ Panoramas

- year: 2018

- dataset：  **(We collect a dataset of 360◦ images to evaluate our approach, which contains 150 videos and 14,076 total frames sampled at 1 FPS.)**  

- abstract:  We explore how intelligent rotations of a spherical image may enable content-aware projection with fewer perceptible distortions. To discover the relationship between these optimal snap angles and the spherical panorama’s content, we develop a reinforcement learning approach for the cubemap projection model.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SAPabstract.png)


- Contributions:
1) snap angles better preserve important objects;
2) our RL solution efficiently pinpoints the best snap angle; 
3) cubemaps unwrapped after snap angle rotation suffer less perceptual distortion than the status quo cubemap
4) snap angles even have potential to impact recognition applications, by orienting 360◦ data in ways that better match the statistics of normal FOV photos used for today’s pretrained recognition networks.

- structure: 

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SAPstructure.png)

- results：

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SAPresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SAPresult1.png)


- analysis: We introduced the snap angle prediction problem for rendering 360◦ images and present a framework to efficiently and accurately predict the snap angle in novel panoramas


