## Spherical_Transformer

- **year**: 2022

- **Publication Conference**: Arxiv

- **Experimental Dataset**:  SPH-MNIST, SPH-CIFAR, and SUN360 datasets

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) Project distortion : This distortion is defined as inconsistency of the shape of a local pattern. It is caused by the planar projection and salient in ERP.

&nbsp; &nbsp; &nbsp; &nbsp; (2) This distortion is caused by the rotation of input data. If 3D rotation is applied to spherical signals, local patterns only change their locations on the sphere. However, a subsequent planar projection makes the local patterns with the same shape have different shapes.
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphericalTransformer.png" width="500" height="500">
</div>

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) It is the first to leverage the transformer architecture to perform representation learning for 360&deg; images. We demonstrate that the proposed transformer architecture is suitable for reducing the projection and rotation distortions.

&nbsp; &nbsp; &nbsp; &nbsp; (2) The proposed spherical transformer (SPHTR) can be easily plugged into existing sampling methods. Using highly uniform sampling methods, our method can significantly reduce the projection distortion. For this, we define the uniformity measure to evaluate the uniformity of sampling methods.

&nbsp; &nbsp; &nbsp; &nbsp; (3) Authors leverage the permutation equivariance of SPHTR and show that an element of the symmetry rotation group can be reduced to permutation of the input sequence. Thus, we argue that the rotation distortion can be effectively alleviated.

- **Proposing Framework**:

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphericalTransformer1.png" width="600" height="500">
</div>
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphericalTransformer2.png" width="500" height="350">
</div>

- **Experimental Results**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphericalTransformer3.png" width="450" height="350">
</div>
