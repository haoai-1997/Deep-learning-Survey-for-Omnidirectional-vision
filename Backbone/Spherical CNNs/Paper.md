## Spherical CNNs

- **year**: 2018

- **Publication Conference**: ICLR

- **Experimental Dataset**: Spherical MNIST, SHREC17 and QM7 task

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) A naive application of convolutional networks to a planar projection of the spherical signal is destined to fail, because the space-varying distortions introduced by such a projection will make translational weight sharing ineffective.

&nbsp; &nbsp; &nbsp; &nbsp; (2) It follows that the result of a spherical correlation (the output feature map) is to be considered a signal on SO(3), not a signal on the sphere, S<sup>2</sup>

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) The **first** automatically differentiable implementation of the generalized Fourier transform for S<sup>2</sup> and SO(3). Our PyTorch code is easy to use, fast, and memory efficie

&nbsp; &nbsp; &nbsp; &nbsp; (2)  The first empirical support for the utility of spherical CNNs for rotation-invariant learning problems.

&nbsp; &nbsp; &nbsp; &nbsp; (3) The implementation of a spherical CNN (S<sup>2</sup>-CNN) involves two major challenges. Whereas a square grid of pixels has discrete translation symmetries, no perfectly symmetrical grids for the sphere exist. This means that there is no simple way to define the rotation of a spherical filter by one pixel. Instead, in order to rotate a filter we would need to perform some kind of interpolation. The other challenge is computational efficiency; SO(3) is a three-dimensional manifold, so a naive implementation ofSO(3) correlation is O(n6).

- **Proposing Framework**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/S2CNN_sc.png" width="700" height="300">
</div>
