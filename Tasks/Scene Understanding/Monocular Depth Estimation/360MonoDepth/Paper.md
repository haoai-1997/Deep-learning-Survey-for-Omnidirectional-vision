## 360MonoDepth: High-Resolution 360° Monocular Depth Estimation

- **year**: 2022

- **Publication Conference**: CVPR

- **Experimental Dataset**:  Matterport3D and Replica datasets (High-resolution and high-quality)

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) Monocular depth estimation remains a challenge for 360° data, particularly for high resolutions (e.g., 2048×1024). Current
CNN-based methods do not support such high resolutions due to limited GPU memory.

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1)  In this paper, the authors proposed a flexible framework for monocular depth estimation from high-resolution 360&dag images **based on aligning and blending depth maps predicted from perspective tangent images**.

&nbsp; &nbsp; &nbsp; &nbsp; (2)  Support for increased resolutions using more tangent images, and improved quality by forward compatibility for future monocular depth estimation approaches.

&nbsp; &nbsp; &nbsp; &nbsp; (3) Authors provide 2048×1024 ground-truth depth maps for Matterport3D’s stitched skyboxes to enable future high- resolution.

- **Proposing Framework**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/depth%20estimation/360Momodepth_framework.png" width="800" height="350">
</div>

- **Experimental Results**：
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/depth%20estimation/360Momodepth_result.png" width="800" height="450">
</div>

- **Limitations (provided by the authors)**：

(1) Propsoed method can fail if the tangent disparity estimates are incorrect, e.g. for large plain walls, saturated skies, or photorealistic wallpapers. (2) Authors also saw inconsistencies in the ground-truth depth maps, such as mirrors or missing lamps or chandeliers that are visible in the image.
