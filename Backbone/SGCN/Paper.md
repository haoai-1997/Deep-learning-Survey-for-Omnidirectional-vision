## Rotation Equivariant Graph Convolutional Network for Spherical Image Classification

- **year**: 2020

- **Publication Conference**: CVPR

- **Experimental Dataset**:  Spherical MNIST, Spherical CIFAR10(classification), ModelNet40 (3D object detection)

- **Motivation**:
Existing methods to transfer CNNs from perspective to spherical images introduce **significant computational costs and/or degradations in accuracy**. And they pursue one of three approaches:

&nbsp; &nbsp; &nbsp; &nbsp; (1) spherical images contains different geometrical properties from planar images.

&nbsp; &nbsp; &nbsp; &nbsp; (2) it is still challenging to generalize CNNs to analyzing spherical images defined on the non-Euclidean spheres, as distortions may be incurred when spherical images are projected onto a flat Euclidean surface to accommodate the grid-based architectures in CNNs.

&nbsp; &nbsp; &nbsp; &nbsp; (3) Previous works can be divided into two categories: 1)、projecting the spherical images into the planar format that can be processed directly by CNNs; 2)、extend CNNs to nonEuclidean domains to avoid the projection distortions. However, for the first approach, without the guidance of rotation-equivariance, although model parameters could be reduced by sharing the kernels across all pixels, the model performance declines inevitably. For the second approach, rotation-equivariant spherical cross-correlation in the spectral domain leadsto high computational cost and significant memory overhead and the Hierarchical Equal Area isoLatitude Pixelation (HEALPix) applied in the **DeepSphere** sitll does not maintain the rotation-equivariance.

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) Authors generalized the grid-based CNNs to a non-Euclidean space by taking into account the geometry of spherical surfaces and proposed a Spherical Graph Convolutional Network (SGCN) to encode rotation equivariant representations.

&nbsp; &nbsp; &nbsp; &nbsp; (2) SGCN constructs a **regular** spherical graph based on two proposed quantitative measures which are used to evaluate the degree of irregularity for a spherical graph. The Geodesic ICOsahedral Pixelation (GICOPix) is adopted to construct spherical graphs with the minimum degree of irregularity compared to the current popular pixelation schemes.

&nbsp; &nbsp; &nbsp; &nbsp; (3) Authors designed a hierarchical pooling layer to keep the rotation-equivariance, followed by a transition layer to enforce the invariance to the rotations for spherical image classification

- **Proposing Framework**:

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SGCNstructure.png" width="800"/>
</div>

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SGCN_pooling.png" width="400"/><img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SGCN_graph.png" width="400"/>
</div>

The resultant features [μ0, σ0, μ1, σ1, ..., μK , σK ] are invariant to the rotation since they are spatially agnostic to the responses of vertices in the spherical graph.

- **Experimental Results**：
- 
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SGCN_result.png" width="300",heigh = "600">
</div>
