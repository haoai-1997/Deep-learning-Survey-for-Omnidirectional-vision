## Manhattan Room Layout Reconstruction from a Single 360 image: A Comparative Study of State-of-the-art Methods

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

- structure: 

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/layout%20reconstruction/Manhattan_DuLa-Net.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/layout%20reconstruction/Manhattan_HorizonNet.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/layout%20reconstruction/Manhattan_LayoutNet.png)



- results：

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/layout%20reconstruction/Manhattan_result.png)

- analysis: This is a detailed introduction for Layout estimation with 360 degree images.
