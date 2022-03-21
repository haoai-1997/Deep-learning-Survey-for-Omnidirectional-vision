## 360MonoDepth: High-Resolution 360° Monocular Depth Estimation

- conference: Arxiv, 2021

- dataset: Matterport3D and Replica

- abstract: we propose a flexible framework for monocular depth estimation from high-resolution 360° images using tangent images. We project the 360° input image onto a set of tangent planes that produce perspective views, which are suitable for the latest, most accurate state-of-the-art perspective monocular depth estimators. We recombine the individual depth estimates using deformable multi-scale alignment followed by gradient-domain blending to improve the consistency ofdisparity estimates.

- contributions: 
(1) A modular framework for high-resolution 360° monocular depth estimation based on aligning and blending depth maps predicted from perspective tangent images.
(2) Support for increased resolutions using more tangent images, and improved quality by forward compatibility for future monocular depth estimation approaches.
(3) We provide 2048×1024 ground-truth depth maps for Matterport3D’s stitched skyboxes to enable future high- resolution.

- Framework:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/depth%20estimation/360Momodepth_framework.png )

- results:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/depth%20estimation/360Momodepth_result.png)
