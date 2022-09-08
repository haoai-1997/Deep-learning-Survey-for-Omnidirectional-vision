## 360 Panorama Synthesis from a Sparse Set of Images with Unknown Field of View

- **year**: 2020

- **Publication Conference**: WACV

- **Experimental Dataset**:  Outdoor panoramic images from Sun360 Dataset (Not avaliable Now)

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) Spherical images can record all information on scenes across the horizontal and vertical viewing directions, and provide viewers with an outward-looking view of scenes and freedom to shift their viewing directions accordingly.

&nbsp; &nbsp; &nbsp; &nbsp; (2) With learning during a life time, human can easily expect what the image looks like in a larger FOV and estimate the scene outside of the viewing boundary. However, for computer vision, synthesizing full a 360&deg; panoramic image from a narrow field-of-view (NFOV) is still an ill-posed problem and highly challenging task.

&nbsp; &nbsp; &nbsp; &nbsp; (3) Previous generative adversarial network (GAN) synthesizes images from noise instance and works well on images with low resolutions but mainly struggles on images with high-resolution and suffers from instability problem during training. 

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1)  In this paper, the authors proposed a novel method to address the problem of **relative FoV estimation and synthesis of 360&deg;  panoramic images from a sparse set of images without any overlap**.

&nbsp; &nbsp; &nbsp; &nbsp; (2)  The authors proposed a model and network to estimate the relative FoV from a sparse set of images with an unknown FOV and no overlap. 

&nbsp; &nbsp; &nbsp; &nbsp; (3) For the panorama synthesis, the authors proposed a hierarchical approach approach.  The authors decomposed synthesizing a high-resolution panorama in a single run into synthesizing images with different scales step by step.

- **Proposing Framework**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Task/Image&Video Manipulation/360 panorama synthesis with multi-scale.png" width="800" height="600">
</div>

&nbsp; &nbsp; &nbsp; &nbsp; The network is composed of a CNN with GAN-based framework and the input to the proposed network is an ordered sequence of 4 images ( 4 cardinal directions of the compass rose: north, west, south, and east). 


&nbsp; &nbsp; &nbsp; &nbsp; **The first step** is relative FoV estimation. As the typical scene captured with standard camera normally have a FOV less than 90&deg;, the four input images are disconnected or without any overlap. The network takes smaller FOV images as the inputs and estimates the relative FOV, as shown in the following firgures. **CNN architecture is utilized to solve the FOV estimation task.**

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/eacf7e77b53b1e5004fef5ea8f75b9427130f69b/Images/Task/Image&Video%20Manipulation/360%20panorama%20synthesis%20with%20multi-scale%20fov.png" width="700" height="250">
</div>

&nbsp; &nbsp; &nbsp; &nbsp; **The second step** is panorama synthesis with a hierarchical approach. The generator consists of three sub-networks, namely $G^s$ , $G^m$ , and $G^l$ , each corresponding to a different scale.  **Weight parameters learned from the previous scale are reused and fine-tuned at each increased scale. This training process is repeated until the original scale is reached.**

- **Experimental Results**：

&nbsp; &nbsp; &nbsp; &nbsp; For the sake of comparison, the authors evaluated the proposed method on both SSIM and PSNR. The baseline consists of two part. For the FoV estimation, DeepFocal (estimates the horizontal FOV of a single image using pre-trained features on AlexNet architecture) is employed as the baseline. And for the panorama synthesis,  pix2pixHD (conditional GANs) is applied as the baseline.

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Task/Image&Video Manipulation/360 panorama synthesis with multi-scale result1.png" width="800" height="450">
</div>

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Task/Image&Video Manipulation/360 panorama synthesis with multi-scale result2.png" width="500" height="150">
</div>

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Task/Image&Video Manipulation/360 panorama synthesis with multi-scale result3.png" width="800" height="650">
</div>

- **Limitations (provided by the authors)**：

Although the performance of the proposed method is promising, it has a few limitations. **First**, the proposed method struggles in synthesizing scene with highly complex structure with many trees, foliage, and people. **Second**, the FOV estimation network is limited to handle input in an ordered non-overlapping sequence with an identical FOV angle. **Third**, in order to use the synthesized panorama in virtual reality equipment, the resolution should be much higher than current maximum resolution (512×1024).
