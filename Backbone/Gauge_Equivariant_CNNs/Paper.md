## auge Equivariant Convolutional Networks and the Icosahedral CNN

- **year**: 2019

- **Publication Conference**: ICML

- **Experimental Dataset**:  IcoMNIST, Climate Pattern Segmentation, Stanford 2D-3D-S

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; The principle of equivariance to symmetry transformations enables a theoretically grounded approach to neural network architecture design. Here we show how this principle can be extended beyond global symmetries to local gauge transformations. This enables the development of a very general class of convolutional neural networks on manifolds that depend only on the intrinsic geometry, and which includes many popular methods from equivariant and geometric deep learning.

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1)  We implement gauge equivariant CNNs for signals defined on the surface of the icosahedron, which provides a reasonable approximation of the sphere.

&nbsp; &nbsp; &nbsp; &nbsp; (2)  By choosing to work with this very regular manifold, we are able to implement the gauge equivariant convolution using a single conv2d call, making it a highly scalable and practical alternative to Spherical CNNs.

&nbsp; &nbsp; &nbsp; &nbsp; (2)  Using this method, we demonstrate substantial improvements over previous methods on the task of segmenting omnidirectional images and global climate patterns.

- **Proposing Framework**:

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/GE_SCNN.png" width="500" height="400">
</div>

- **Limitations (provided by the authors)**：

Although we have only touched on the connections to physics and geometry, there are indeed interesting connections, which we plan to elaborate on in the future. From the perspective of the mathematical theory of principal fiber bundles, our definition of manifold convolution is entirely natural. Indeed it is clear that gauge invariance is not just nice to have, but necessary in order for the convolution to be geometrically well-defined. In future work, we plan to implement gauge CNNs on general manifolds and work on further scaling of spherical CNNs.

