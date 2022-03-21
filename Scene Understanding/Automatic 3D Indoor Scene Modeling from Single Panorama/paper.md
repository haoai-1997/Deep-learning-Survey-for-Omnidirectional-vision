## Automatic 3D Indoor Scene Modeling from Single Panorama

- year: 2018

- dataset：  **(SUN360; dataset of 20 panoramas is created using textured3D point clouds that we captured using a FARO 3D scanner; dataset consists of 60 syntheticpanoramas we created using 3ds Max; )**  

- abstract: We describe a system that automatically extracts 3D geometry of an indoor scene from a single 2D panorama. 

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/automatic3Dabstract.png)

- Contributions:

Our system recovers the spatial layout and also recovers shapes of typical indoor objects. Using sampled perspective subviews, we extract geometric cues and these cues are used for ground plane estimation and occlusion reasoning. The recovered layout is then used to guide shape estimation of the remaining objects using their normal information.


- structure:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/automatic3Dstructure.png)


- results：

view selection capability on Pano2Vid dataset; the temporal summarization with a newly
collected 360◦ video dataset, another domain, with image-based storytelling VIST dataset
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/automatic3Dresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/automatic3Dresult1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/automatic3Dresult2.png)

- analysis: We have presented a new system to add depth to a 2D panorama of an indoor scene.  Our system uses semantic cues and geometric cues to partition the panorama into background (layout) and foreground (object). The layout which includes the ground plane, is recovered using geometric cues. Layout information is then used to help extract object depth.
