## Automatic Content-aware Projection for 360◦ Videos (traditional)

- year: 2018

- abstract:  In this paper, we propose a fully-automated framework for generating content-aware 2D normal-view perspective videos from 360◦ videos. Especially, we focus on the projection step preserving important image contents and reducing image distortion. Basically, our projection method is based on Pannini projection model.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ACPabstract.png)


- Contributions:
1) we propose a contents-preserving projection method optimizing a single Pannini projection model. 
2) we utilize multiple Pannini projection models to globally minimize contents distortion. 
3) we enforce the temporal consistency for image projection to produce temporally stable normal-view videos.

- results：

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ACPresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ACPresult1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ACPresult2.png)


- analysis: We proposed multi-model based Pannini projection optimization method that preserves both linear structures and salient objects which are automatically extracted. Additionally, we considered temporal consistency to generate temporally stable videos.


