## OmniDepth: Dense Depth Estimation for Indoors Spherical Panoramas
- conference: ECCV, 2018

- dataset: 3D60.

- abstract: Monocular depth estimation models trained on traditional images produce sub-optimal results on omnidirectional images,
showcasing the need for training directly on 360o datasets, which however, are hard to acquire. In this work, 
we circumvent the challenges associated with acquiring high quality 360 
datasets with ground truth depth annotations, by re-using recently released large scale 3D datasets and re-purposing them to 360o via rendering.
- contributions: 
(1) We present the first learning based dense depth estimation method that was trained with and operates directly on omnidirectional content in the form of equirectangular images.
(2) We offer a dataset consisting of 360 color images paired with ground truth 360o depth maps in equirectangular format.
(3) We propose and validate, a CNN auto-encoder architecture specifically designed for estimating depth directly on equirectangular images.
(4) We show howmonocular depth estimation methods trained on traditional 2D images fall short or produce low quality results when applied to 
equirectangular inputs, highlighting the need for learning directly on the 360 domain.

- Framework:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/depth%20estimation/OmniDepth_framework1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/depth%20estimation/OmniDepth_framework2.png)

- results:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/depth%20estimation/OmniDepth_result1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/depth%20estimation/OmniDepth_result2.png)
