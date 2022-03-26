## Self-supervised Representation Learning Using 360◦ Data

- year: 2019

- dataset：**(PanoContext; Stanford 2D-3D; Matterport3D;  a specific testing set of a hundred images: AtlantaLayout)**  

- abstract:  In this paper, we present the first work to exploitunlabeled 360◦ data for image representation learning. We propose middle-out, a new self-supervised learning task, which leverages the spatial configuration of normal field-of-view images sampled from a 360◦ image as supervisory signal. 

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SSRLabstract.png)

- Contributions:
1) most previous methods train the network to learn about object parts, whereas our method encourages the network to learn a higher-level understanding of the scene beyond single object and develop common sense knowledge about the structure of the visual world. 
2) unlike previous methods that use input images with fixed FoV, our method can adjust the FoV of the input perspective images. Therefore, our method can generate multi-scale input images and enable the network to learn robust representation for objects of different sizes.

- structure: a Siamese triplet architecture with three parallel Convolutional Networks (ConvNets) to solve the middle image identification task.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SSRLstructure.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SSRLstructure1.png)

- results：
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SSRLresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SSRLresult1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SSRLresult2.png)
- analysis: In this work, we propose a novel formulation of self-supervised representation learning by exploiting a new data source: unlabeled 360◦ images. We train a ConvNet model to identify the middle image among the three shuffled images which are sampled by applying perspective projections on a 360◦ image.
