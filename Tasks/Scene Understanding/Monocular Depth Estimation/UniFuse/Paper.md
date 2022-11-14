## UniFuse: Unidirectional Fusion for 360° Panorama Depth Estimation

- **year**: 2021

- **Publication Conference**: IEEE Robotics and Automation Letters

- **Experimental Dataset**:  Matterport3D, Stanford2D3D, 3D60, and PanoSUNCG

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) applying well-studied CNNs for perspective images to the standard representation of spherical panoramas, i.e., the equirectangular projection, is suboptimal, as it becomes distorted towards the poles.

&nbsp; &nbsp; &nbsp; &nbsp; (2) Another representation is the cubemap projection, which is distortion-free but discontinued on edges and limited in the field-of-view.

&nbsp; &nbsp; &nbsp; &nbsp; (3) We argue that feeding the ERP features to the CMP branch is unnecessary, as the ultimate goal is to output an equirectangular depth map. Optimizing the cube map depth may cause the training to lose focus on the equirectangular depth. Furthermore, performing the fusion at the encoding stage may disturb the learning of the encoder, as it is usually initialized with ImageNet pretrained parameters.

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1)  Authors proposed a new fusion framework, which unidirectionally feeds the features extracted from CMP to the ERP branch only at the decoding stage to better support the ERP prediction

&nbsp; &nbsp; &nbsp; &nbsp; (2)  Authors design a fusion module for our fusion framework, aiming at using Cubemap to Enhance the Equirectangular features (noted as CEE).

&nbsp; &nbsp; &nbsp; &nbsp; (3) Authors perform experiments to show our approach's effectiveness, and the final model establishes the state-of-the-art performance and has advantages on the complexity and generalization ability.

- **Proposing Framework**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/depth%20estimation/UniFuse_framework.png" width="800" height="250">
</div>

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/depth%20estimation/UniFuse_fusion_module.png" width="800" height="335">
</div>

- **Experimental Results**：
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/depth%20estimation/UniFuse_results.png" width="800" height="550">
</div>
