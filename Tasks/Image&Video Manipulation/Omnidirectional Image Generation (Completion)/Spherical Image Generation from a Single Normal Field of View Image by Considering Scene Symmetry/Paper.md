## Spherical Image Generation from a Single Normal Field of View Image by Considering Scene Symmetry

- **year**: 2021

- **Publication Conference**: AAAI

- **Experimental Dataset**:  Sun360 Dataset (Not avaliable Now)

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) Spherical images, with the FoV of all possible directions (360&deg×180&deg), can *capture environments around the main subject and represent the space itself as a subject*. Furthermore, *when viewed through a head-mounted display, spherical images allow one to enjoy a scene in a more immersive manner.*

&nbsp; &nbsp; &nbsp; &nbsp; (2) Capturing spherical images is not an easy task, as doing so requires a specific panoramic camera or specific software that *stitches together images taken from multiple directions*.

&nbsp; &nbsp; &nbsp; &nbsp; So generating a spherical image from a single normal-field-of-view (NFOV) image taken using a normal camera is more convenient and it would considerably expand the usage scenarios that require plausibility rather than reproducibility.

- **Challenge**:

&nbsp; &nbsp; &nbsp; &nbsp; (1)  Generating an image corresponding to the spherical structure; Conventional image-completion methods are not suitable for generating spherical images, because these methods are designed for planar NFOV images.

&nbsp; &nbsp; &nbsp; &nbsp; (2)  Controlling the high degree of freedom involved in generating a wide area, which includes the all directions of a plausible spherical image. Because a spherical image cannot be uniquely determined for an NFOV image, the generation of various plausible scenes must be controlled.

- **Proposing Framework**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Task/Image&Video Manipulation/Spherical Image Generation.png" width="1000" height="450">
</div>

&nbsp; &nbsp; &nbsp; &nbsp; The authors conducted a novel model to generate a spherical image x_g from a partial image (e.g., an NFOV image) x_l by using a scene-symmetry parameter $s \in \mathcal{R}^C$. The term s corresponds to the intensity of C types of rotational symmetry around the gravity-axis, and plane symmetry to vertical planes. To generate diverse images conditioned with the partial image, they employ **CVAEs** as a base framework, and they also incorporated scene-symmetry parameters as latent variables. Furthermore, the probability density functions are represented by the equirectangular projection-based CNNs, and scene symmetry is implemented as a **circular shift and a flip** of the hidden variables.

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/a207527aa8c2a1437c390a15a73772badf9e7e60/Images/Task/Image&Video%20Manipulation/circular%20padding.png" width="400" height="150"><img src="https://github.com/VLISLAB/360-DL-Survey/blob/a207527aa8c2a1437c390a15a73772badf9e7e60/Images/Task/Image&Video%20Manipulation/circular%20shift%20and%20padding.png" width="400" height="400">
</div>

- **Experimental Results**：

&nbsp; &nbsp; &nbsp; &nbsp; The method displayed a superior FID score than those of the other methods, meaning that our method can generate plausible images by capturing the distribution of high-order features of the spherical images.

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Task/Image&Video Manipulation/Spherical Image Generation result1.png" width="450" height="240">
</div>

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Task/Image&Video Manipulation/Spherical Image Generation result2.png" width="800" height="900">
</div>
 
