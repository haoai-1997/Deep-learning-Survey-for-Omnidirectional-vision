## Learning Spherical Convolution for Fast Features from 360&deg; Imagery

- **year**: 2017

- **Publication Conference**: NIPS

- **Experimental Dataset**:  Pano2Vid and PASCAL VOC datasets

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) Convolutional neural networks (CNNs) trained on images from perspective cameras yield "flat" filters, yet 360&deg; images cannot be projected to a single plane without significant distortion.

&nbsp; &nbsp; &nbsp; &nbsp; (2) Repeatedly projecting the viewing sphere to all tangent planes is accurate, but much too computationally intensive for real problems.

&nbsp; &nbsp; &nbsp; &nbsp; (3) Authors propose to learn a spherical convolutional network that translates a planar CNN to process 360&deg; imagery directly in its equirectangular projection.

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1)  In this paper, the authors studied efficient feature extraction for 360&deg; images and video,.

&nbsp; &nbsp; &nbsp; &nbsp; (2)  The ability to leverage powerful pre-trained networks researchers have carefully honed (together with massive labeled image training sets) for perspective images. (Specifically, besides providing fast general feature extraction for 360° imagery, our approach provides a bridge from 360° content to existing heavily supervised datasets dedicated to perspective images.)

&nbsp; &nbsp; &nbsp; &nbsp; (3) This work aims to learn a CNN that processes a 360&deg; image in its equirectangular projection (fast) but mimics the "flat" filter responses that an existing network would produce on all tangent plane projections for the original spherical image (accurate). 

- **Proposing Framework**:
(**There exists one prior condition that backprojecting the regular grid on the planar plane into the equirectangular plane is fixed at the  0&deg; longitude and the latitude can be flexibly changed.**)

See the following figure, the convolution kernel should transform accordingly. The approach 1) adjusts the shape of the convolution kernel to account for the distortion (in the ERP), in particular the content expansion, and 2) reduces the number of max-pooling layers to match the pixel sizes in N<sub>e</sub>(a spherical convolution network) and N<sub>p</sub>(a perspective convolution network).

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/sphconv.png" width="800" height="350">
</div>

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/sphconv1.png" width="800" height="300">
</div>

- **Limitations (provided by the authors)**：
- 
One limitation of SPHCONV is that it cannot handle very close objects that span a large FOV. Because the goal of SPHCONV is to reproduce the behavior of models trained on perspective images, the capability and performance of the model is bounded by the target model N<sup>p<sup>; Another limitation of SPHCONV is the resulting model size. Because it unties the kernel weights along θ, the model size grows linearly with the equirectangular image height. **The model size can easily grow to tens of gigabytes as the image resolution increases.**
