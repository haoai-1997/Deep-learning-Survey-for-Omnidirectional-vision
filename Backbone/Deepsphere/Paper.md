## DeepSphere: a graph-based spherical CNN

- **year**: 2020

- **Publication Conference**: ICLR

- **Experimental Dataset**:  SHREC'17 (3D shapes), climate event segmentation, weather stations

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) As neural networks (NNs) have proved to be great tools for inference, variants have been developed to handle spherical data. Exploiting the locally Euclidean property of the sphere, early attempts used standard 2D convolutions on a grid sampling of the sphere. While simple and efficient, those convolutions are not equivariant to rotations.

&nbsp; &nbsp; &nbsp; &nbsp; (2) On the other side of this tradeoff, previous work proposed to perform proper spherical convolutions through the spherical harmonic transform. While equivariant to rotations, those convolutions are expensive.

&nbsp; &nbsp; &nbsp; &nbsp; (3) As a lack of equivariance can penalize performance and expensive convolutions prohibit their application to some real-world problems, methods standing between these two extremes are desired.

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) First, authors studied both theoretically and empirically how equivariance is affected by the underlying graph with respect to the number of vertices and neighbors.

&nbsp; &nbsp; &nbsp; &nbsp; (2) Second, authors evaluated DeepSphere, a method based on a graph representation of the sampled sphere, strikes a controllable balance between these two desiderata, on relevant problems.

&nbsp; &nbsp; &nbsp; &nbsp; (3) DeepSphere leverages graph convolutions to achieve the following properties: (i) computational efficiency, (ii) sampling flexibility, and (iii) rotation equivariance.

- **Proposing Framework**:

&nbsp; &nbsp; &nbsp; &nbsp; The main idea is to model the sampled sphere as a graph of connected pixels: the length of the shortest path between two pixels is an approximation of the geodesic distance between them. Authors used the graph CNN formulation and a pooling strategy that exploits hierarchical samplings of the sphere.

The following figure shows the equivariance error for different parameter sets of DeepSphere for the HEALPix sampling

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/deepsphere.png" width="400" height="500">
</div>

- **Experimental Results**：

&nbsp; &nbsp; &nbsp; &nbsp; For the sake of comparison, the authors evaluated the proposed method on both SSIM and PSNR. The baseline consists of two part. For the FoV estimation, DeepFocal (estimates the horizontal FOV of a single image using pre-trained features on AlexNet architecture) is employed as the baseline. And for the panorama synthesis,  pix2pixHD (conditional GANs) is applied as the baseline.

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/deepsphere_results.png" width="600" height="200"><img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/deepsphere_results1.png" width="600" height="200">
</div>


- **Inspriration (provided by the authors)**：

&nbsp; &nbsp; &nbsp; &nbsp; A potential drawback of graph Laplacian-based approaches is the isotropy of graph filters, reducing in principle the expressive power of the NN. Experiments from Cohen et al. (2019) and Boscaini et al. (2016) indeed suggest that more general convolutions achieve better performance. Our experiments on 3D shapes (section 4.1) and climate (section 4.3) however show that DeepSphere's isotropic filters do not hinder performance. Possible explanations for this discrepancy are that NNs somehow compensate for the lack of anisotropic filters, or that some tasks can be solved with isotropic filters. The distortions induced by the icosahedral projection in (Cohen et al., 2019) or the leakage of curvature information in (Boscaini et al., 2016) might also alter performance. 

&nbsp; &nbsp; &nbsp; &nbsp; Developing graph convolutions on irregular samplings that respect the geometry of the sphere is another research direction of importance. Practitioners currently interpolate their measurements (coming from arbitrarily positioned weather stations, satellites or telescopes) to regular samplings. This practice either results in a waste of resolution or computational and storage resources. Our ultimate goal is for practitioners to be able to work directly on their measurements, however distributed.
