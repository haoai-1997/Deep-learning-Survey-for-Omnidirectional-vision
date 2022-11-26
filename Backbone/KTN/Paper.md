## Kernel Transformer Networks for Compact Spherical Convolution

- **year**: 2019

- **Publication Conference**: CVPR

- **Experimental Dataset**:  Spherical MNIST(classification), Pano2Vid and Pascal VOC(object detection)

- **Motivation**:
Existing methods to transfer CNNs from perspective to spherical images introduce **significant computational costs and/or degradations in accuracy**. And they pursue one of three approaches:

&nbsp; &nbsp; &nbsp; &nbsp; (1) The first adapts the network architecture for equirectangular projection and trains kernels of variable size to account for its distortions. While accurate, this approach suffers from significant model bloat.

&nbsp; &nbsp; &nbsp; &nbsp; (2) The second approach instead adapts the kernels on the sphere, resampling the kernels or projecting their tangent plane features. While allowing kernel sharing and hence smaller models, this approach degrades accuracy *—especially for deeper networks—* due to an implicit interpolation assumption, as we will explain below.

&nbsp; &nbsp; &nbsp; &nbsp; (3) The third approach defines convolution in the spectral domain, which has significant memory overhead and thus far limited applicability to realworld data.

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) **Key highlights of the proposed KTN are its transferability and compactness—both of which owe to our functionbased design.**

&nbsp; &nbsp; &nbsp; &nbsp; (2) Proposed Kernel Transformer Network (KTN) efficiently transfers convolution kernels from perspective images to the equirectangular projection of 360&deg; images.
&nbsp; &nbsp; &nbsp; &nbsp; (3) Results show KTN models are orders of magnitude smaller than the most accurate competitor, SphConv. Compared with Spherical U-Net and SphereNet, KTN is much more data efficient because it does not require any annotated 360&deg; images for training, and it is more accurate because it avoids their feature interpolation assumption.

- **Proposing Framework**:

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/KTN_framework.png" width="400"/><img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/KTN_framework1.png" width="400"/>
</div>

&nbsp; &nbsp; &nbsp; &nbsp; We use a Residual Network-like architecture. For both the residual and shortcut branches, we first apply the row dependent projection to resize the kernel to the target size. The residual branch then applies depthwise separable convolution twice. Our depthwise separable convolution block consists of ReLU-pointwise conv-ReLU-depthwise conv. The two branches are added together to generate the output kernel, which is then applied to a 360&deg; feature map.

- **Experimental Results**：

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/KTN_results.png" width="400"/><img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/KTN_results1.png" width="400"/>
</div>
