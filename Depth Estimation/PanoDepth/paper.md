## PanoDepth: A Two-Stage Approach for Monocular Omnidirectional Depth Estimation

- year: 2021

- dataset: three panorama RGBD benchmark datasets -- Stanford2D3D, 360D and the omnidirectional Stereo Dataset

- abstract: In this paper, we propose a novel, model-agnostic, two-stage pipeline for omnidirectional monocular depth estimation. 
In the second stage, we propose a differentiable Spherical Warping Layer to handle omnidirectional stereo geometry efficiently and effectively.

- contributions:
(1) We propose a novel, model-agnostic, two-stage frame-work PanoDepth, including view synthesis and stereo matching, to fully exploit the synthesized 360 views and spherical stereo constraints
(2) PanoDepthout performs the state-of-the-art monocular omnidirectional depth estimation approaches by a large margin.
(3) We propose a novel differentiable Spherical Warp-ing Layer (SWL) which adapts regular stereo matching networks to 360 stereo geometry, and enables advanced features such as multi-view stereo and cascade mechanism for stereo performance boost.

- structure:
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PanoDepth.png)

- loss function
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PanoDepth_total_loss.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PanoDepth_coarse_loss.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PanoDepth_loss_stereo.png)

- results:
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PanoDepth_result.png)

- analysis
There are several research venues we would like to further explore in the future, such as alternative view synthesis methods like, and360 depth estimation in outdoor scenarios for applications like autonomous driving.


