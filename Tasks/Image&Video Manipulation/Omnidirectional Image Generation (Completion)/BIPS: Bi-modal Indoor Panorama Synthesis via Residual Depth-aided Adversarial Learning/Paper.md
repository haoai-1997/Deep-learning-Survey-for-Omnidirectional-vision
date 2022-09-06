## BIPS: Bi-modal Indoor Panorama Synthesis via Residual Depth-aided Adversarial Learning

- **year**: 2022

- **Publication Conference**: ECCV

- **Experimental Dataset**:  Sun360 Dataset (Not avaliable Now)

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) As omnidirectional RGB-D data is not always available, synthesizing RGB-D panorama data from limited information of a scene can be useful.

&nbsp; &nbsp; &nbsp; &nbsp; (2) Previous works for RGB panorama image generation suffer from limited image quality and can not be directly extended for RGB-D panorama synthesis;

&nbsp; &nbsp; &nbsp; &nbsp; In this paper, the authors proposed a novel research problem: ***RGB-D panorama synthesis** under the **arbitrary configurations** of cameras and depth sensors*.

- **Challenge**:

&nbsp; &nbsp; &nbsp; &nbsp; (1)  

&nbsp; &nbsp; &nbsp; &nbsp; (2)  

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1)  The authors proposed a **bi-modal panorama synthesis** (BIPS) framework, mainly for indoor environments.

&nbsp; &nbsp; &nbsp; &nbsp; (2)  As there is no tailored evaluation metric for RGB-D panorama synthesis, the authors proposed a novel metric to effectively evaluate its perceptual quality, called Fr ́echet Auto-Encoder Distance (FAED).

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
 
