## Learning SO(3) Equivariant Representations with Spherical CNNs

- **year**: 2018

- **Publication Conference**: ECCV

- **Experimental Dataset**:  the SHREC'17 contest and ModelNet40 datasets

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) To address the the problem of 3D rotation equivariance in convolutional neural networks.

&nbsp; &nbsp; &nbsp; &nbsp; (2) The difference between convolution that has spherical outputs and correlation that has outputs in the rotation group SO(3).

&nbsp; &nbsp; &nbsp; &nbsp; (3) Convolutions cannot be applied with spatially-invariant impulse responses (masks), but can be exactly computed in the spherical harmonic domain through pointwise multiplication.

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1)  In this paper, the authors proposed **the first neural network based on spherical convolutions**.

&nbsp; &nbsp; &nbsp; &nbsp; (2)  The authors introduce pooling and parameterization of filters in the spectral domain, with enforced spatial localization and capacity independent of the resolution. 

&nbsp; &nbsp; &nbsp; &nbsp; (3) Their network has much lower capacity than non-spherical networks applied on 3D data without sacrificing performance.Our

- **Proposing Framework**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SO3ER_framework.png" width="800" height="450">
</div>

&nbsp; &nbsp; &nbsp; &nbsp; In this network, the spherical convolution based on the spherical harmonics and can be seen as **marginalizing the angle responsible for rotating the filter about its north pole, or equivalently considering zonal filters on the sphere**.


&nbsp; &nbsp; &nbsp; &nbsp; As shown in the framework figure, authors defined a block as one spherical convolutional layer, followed by optional pooling, and nonlinearity. A weighted global average pooling is applied at the last layer to obtain an invariant descriptor. This section details the architectural design choices

- **Experimental Results**：

&nbsp; &nbsp; &nbsp; &nbsp; The greatest advantage of this model is inherent equivariance to SO(3); authors focusd the experiments in problems that benefit from it; namely, shape classification and retrieval in arbitrary orientations, and shape alignment.

