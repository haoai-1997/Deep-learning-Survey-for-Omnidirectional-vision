## SpherePHD: Applying CNNs on a Spherical PolyHeDron Representation of 360&deg; Images

- **year**: 2019

- **Publication Conference**: CVPR

- **Experimental Dataset**:  Spherical MNIST dataset(classifcation), SYNTHIA dataset(object detection), Stanford2D3D (Semantic segmentation)

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) Most of previous works use image representations (ERP, Cubemap, Tangent) in the Euclidean space defined by transforming the omni-directional views originally in the non-Euclidean space. This transformation leads to shape distortion due to nonuniform spatial resolving power and loss of continuity.

&nbsp; &nbsp; &nbsp; &nbsp; (2) During the transformation from the nonEuclidean space to the Euclidean space, some important properties can be lost. For example, the non-Euclidean space that omni-directional images are defined in has a cyclical property, however, during the transformation from the non-Euclidean space to the Euclidean space through the ERP, the continuity and cyclical properties are lost.

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1)  In this paper, authors propose a **spherical polyhedron-based representation of images, called SpherePHD**, followed by new convolution and pooling methods to apply CNNs based on the proposed representation.

&nbsp; &nbsp; &nbsp; &nbsp; (2) The proposed projection will give less variance of spatial resolving power and distortion than others. Furthermore, the rotational symmetry of the spherical geometry will allow the image processing algorithms to be rotation invariant.

&nbsp; &nbsp; &nbsp; &nbsp; (3) Lastly, the spherical polyhedron provides a continuity property; there is no border where the image becomes discontinuous. This particular representation aims to resolve both the issues raised in using ERP and cube map representations.

&nbsp; &nbsp; &nbsp; &nbsp; (4) The contributions of this paper also include designing the convolution kernel and a specific method of applying convolution kernels and pooling kernelsto use CNNs on the proposed spherical polyhedron representation of images.

- **Proposing Framework**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SpherePHD.png" width="400" height="260"><img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SpherePHD1.png" width="400" height="260">
</div>

&nbsp; &nbsp; &nbsp; &nbsp; The left figure shows icosahedral geodesic polyhedron and proposed SpherePHD and the right firgure suggests that **a regular convex polyhedron with a greater number of faces can have much lower irregularity when it is subdivided and turned into a spherical polyhedron**.

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SpherePHDconv.png" width="400" height="200"><img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SpherePHDpool.png" width="400" height="260">
</div>

&nbsp; &nbsp; &nbsp; &nbsp; More details about the CNN implementation on spherePHD can be referred to the Sec3.6 in the paper.

- **Experimental Results**：

&nbsp; &nbsp; &nbsp; &nbsp; For the sake of comparison, the authors evaluated the proposed method on both SSIM and PSNR. The baseline consists of two part. For the FoV estimation, DeepFocal (estimates the horizontal FOV of a single image using pre-trained features on AlexNet architecture) is employed as the baseline. And for the panorama synthesis,  pix2pixHD (conditional GANs) is applied as the baseline.

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SpherePHDseg.png" width="400" height="400"><img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SpherePHDclassification.png" width="400" height="260"><img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SpherePHDdetection.png" width="400" height="600">
</div>
