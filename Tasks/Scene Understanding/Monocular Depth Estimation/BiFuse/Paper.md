## BiFuse: Monocular 360-degree Depth Estimation via Bi-Projection Fusion

- **year**: 2020

- **Publication Conference**: CVPR

- **Experimental Dataset**: Stanford2D3D dataset, 3D60 dataset, PanoSUNCG dataset and Matterport3D dataset

- **Motivation**: 

- The authors proposed to predict the depth map of a monocular 360&deg image by mimicking both peripheral and foveal vision of the human eye. Accordingly, authors adopt a two-branch neural network leveraging two common projections: equirectangular projections(ERP) and cubemap projections(CP).

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) An end-to-end two-branch network is proposed, which incorporates both equirectangular and cubemap projections, to mimic the combination of peripheral and foveal vision of the human eye, respectively.
&nbsp; &nbsp; &nbsp; &nbsp; (2) To share the information of different projections, a bi-projection fusion procedure is proposed with learnable masks to balance the information from two projections.
&nbsp; &nbsp; &nbsp; &nbsp; (3) Authors propose spherical padding to extend the field-of-view of cubemap projection and reduce the boundary inconsistency of each face.

- **Proposing Framework**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/BiFuse.png" width="800" height="350">
</div>

- **Experimental Results**：
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/BiFuse_exp1.png" width="50%" height="50%">
</div>
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/BiFuse_exp2.png" width="50%" height="50%">
</div>

- **Analysis**： 

This paper employ two projection formats of 360-degree images to better extracting and fusing information.

