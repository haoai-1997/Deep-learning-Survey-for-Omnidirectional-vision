## HoHoNet: 360 Indoor Holistic Understanding with Latent Horizontal Features

- year: CVPR 2021

- dataset：  **(Stanford2D3D and Matterport3D)**  

- abstract: This work presents a novel framework, HoHoNet, which is the first step to learning compact latent horizontal 
features for dense modalities modeling of omnidirectional images. HoHoNet is fast, versatile, and accurate for solving layout reconstruction,
depth estimation, and semantic segmentation with accuracy on par with or better than the state-of-the-art.

(1) HoHoNet can yield dense modalities for a high- resolution 512 × 1024 panorama at 52 FPS and 110 FPS with ResNet-50 and ResNet-34 respectively.
(2) Our method relaxes the final prediction space upon the compact LHFeat from O(W) to the most common O(HW), capable of modeling layout, dense depth, and semantic segmentation.
(3) The performances of HoHoNet on semantic segmentation and layout reconstruction are on par with the recent state-of-the-art. On dense depth estimation, HoHoNet outperforms prior arts by a margin


- structure:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/scene%20understanding/HohoNet_Framework.png)

-EHC block

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/scene%20understanding/HohoNet_EHC.png)

- results：

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/scene%20understanding/HohoNet_result.png)
