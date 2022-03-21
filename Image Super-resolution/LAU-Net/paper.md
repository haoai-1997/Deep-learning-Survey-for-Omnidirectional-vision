## LAU-Net: Latitude Adaptive Upscaling Network for Omnidirectional Image Super-resolution

- year: 2021

- dataset: ODI-SR dataset (self-collected), and SUN 360 Panorama Dataset

- Abstract: In this work, we propose a novel latitude adaptive upscaling network (LAU-Net) for ODI super-resolution, which allows pixels at different latitudes to adopt distinct upscaling factors. Specifically, we introduce a Laplacian multi-level separation architecture to split an ODI into different latitude bands, and hierarchically upscale them with different factors. In addition, we propose a deep reinforcement learning scheme with a latitude adaptive reward, in order to automatically select optimal upscaling factors for different latitude bands.
- Contributions:
(1) We establish a large database for ODI SR, which consists of 1,000 high-quality ODI images, with diverse image resolutions and content;
(2) We propose a new network named LAU-Net for ODI SR, in which different latitude bands are allowed to have distinct upscaling factors for resource efficiency;
(3) We develop an RL scheme to automatically select the optimal upscaling factors for different latitude bands, which significantly improves the SR performance using less computational resource.

- Structure: Distortion-aware convolution

<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LAU_1.png" width="70%" height="70%">
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LAU_2.png" width="70%" height="70%">

- Results：
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LAU_exp1.png" width="50%" height="50%">
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LAU_exp2.png" width="50%" height="50%">

-Analysis: This work considers the different density of 360 image in latitude and addresses a single 360 image with different powers.



