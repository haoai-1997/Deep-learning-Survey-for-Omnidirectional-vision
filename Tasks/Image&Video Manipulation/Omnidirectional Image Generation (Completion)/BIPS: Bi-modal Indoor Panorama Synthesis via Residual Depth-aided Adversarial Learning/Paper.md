## BIPS: Bi-modal Indoor Panorama Synthesis via Residual Depth-aided Adversarial Learning

- **year**: 2022

- **Publication Conference**: ECCV

- **Experimental Dataset**:  Structured3D dataset,  Matterport3D, and 2D-3D-S dataset
- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) As omnidirectional RGB-D data is not always available, synthesizing RGB-D panorama data from limited information of a scene can be useful.

&nbsp; &nbsp; &nbsp; &nbsp; (2) Previous works for RGB panorama image generation suffer from limited image quality and can not be directly extended for RGB-D panorama synthesis;

&nbsp; &nbsp; &nbsp; &nbsp; In this paper, the authors proposed a novel research problem: ***RGB-D panorama synthesis** under the **arbitrary configurations** of cameras and depth sensors*.

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1)  The authors proposed a **bi-modal panorama synthesis** (BIPS) framework, mainly for indoor environments.

&nbsp; &nbsp; &nbsp; &nbsp; (2)  As there is no tailored evaluation metric for RGB-D panorama synthesis, the authors proposed a novel metric to effectively evaluate its perceptual quality, called Fr ́echet Auto-Encoder Distance (FAED).

- **Proposing Framework**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Task/Image&Video Manipulation/bips.png" width="1000" height="480">
</div>

&nbsp; &nbsp; &nbsp; &nbsp; With both the RGB image $I^{rgb}_ {in}$ and depth data $I^{d}_ {in}$ as the input, the goal of the proposed framework is to directly generate the RGB panorama $ERP^{rgb}$ and depth panorama $ERP^{d}$ simultaneously via a mapping function G, which can be described as $(I^{rgb} _{out}, I^{d} _{out}) = (ERP^{rgb}, ERP^{d} ) = G(I^{rgb} _{in}, I^{d} _{in}) )$.  **As the information in the left and right boundaries in ERP images should be connected, the designed G uses circular padding before each convolutional operation.**

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Task/Image&Video Manipulation/bips generator.png" width="400" height="250"><img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Task/Image&Video Manipulation/bips faed.png" width="400" height="250">
</div>

- **Experimental Results**：

&nbsp; &nbsp; &nbsp; &nbsp; The method displayed a superior FID score than those of the other methods, meaning that our method can generate plausible images by capturing the distribution of high-order features of the spherical images.

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Task/Image&Video Manipulation/bips result.png" width="1000" height="550">
</div>

 
