## Pano Popups: Indoor 3D Reconstruction with a Plane-Aware Network

- conference: International Conference on 3D Vision (3DV), 2019

- dataset: Scene Un- derstanding and Modeling (SUMO) dataset

- abstract: In this work we present a method to train a plane-aware convolutional neural network for dense depth and surface normal estimation as well as plane boundaries from a single indoor 360◦image. Using our proposed loss function,our network outperforms existing methods for single-view, indoor, omnidirectional depth estimation and provides an initial benchmark for surface normal prediction from 360◦images. Our improvements are due to the use of a novel plane-aware loss that leverages principal curvature as an indicator of planar boundaries. We also show that including geodesic coordinate maps as network priors provides a significant boost in surface normal prediction accuracy. Finally, we demonstrate how we can combine our network's outputs to generate high quality 3D "pop-up" models of in-door scenes.

- contributions: 
(1) We propose a plane-aware cost function to estimate depth, surface normals, and plane boundaries from a single 360◦image.
(2) We demonstrate that the inclusion of geodesic coordinate maps as extra inputs to the network improves surface normal prediction from omnidirectional images.
(3) We qualitatively show that our network can be used to generate a 3D planar model from a single 360◦image.

- Framework:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/3D%20reconstruction/Pano_Popups_framework.png)

- results:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/3D%20reconstruction/Pano_Popups_result.png)
