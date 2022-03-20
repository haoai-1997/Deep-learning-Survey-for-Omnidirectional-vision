## SalGCN: Saliency Prediction for 360-Degree Images Based on Spherical Graph Convolutional Networks

- year: 2020

- dataset: Salient360 dataset

- Abstract: In this paper, we propose a saliency prediction framework for 360-degree images based on graph convolutional networks (SalGCN), which directly applies to the spherical graph signals. Specifically, we adopt the Geodesic ICOsahedral Pixelation (GICOPix) to construct a spherical graph signal from a spherical image in equirectangular projection (ERP) format. We then propose a graph saliency prediction network to directly extract the spherical features and generate the spherical graph saliency map.
- Contributions:
(1) Address the projection distortion problem. (2) The redundant image boundaries and repeated computations on different projection planes are avoided. (3) GCN will not interpolate the feature map, thus preventing interpolation errors.

- Structure: GCN, ICOsahedral

<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SalGCN.png" width="70%" height="70%">

- Results：
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SalGCN_exp1.png" width="50%" height="50%">

-Analysis: This work utilizes Icosahedral Pixelation to project ERP onto a spherical graph and extract features directly on the constructed graph, which avoids problems in ERP and CMP.



