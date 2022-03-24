## Sat2Vid: Street-view Panoramic Video Synthesis from a Single Satellite Image

- year: 2021

- dataset：  **(extend London panorama dataset used in S2G by generating the ground truth of street-view video snippets)**  

- abstract: We present a novel method for synthesizing both temporally and geometrically consistent street-view panoramic video from a single satellite image and camera trajectory. For geometrical and temporal consistency, our approach explicitly creates a 3D point cloud representation of the scene and maintains dense 3D-2D correspondences across frames that reflect the geometric scene configuration inferred from the satellite view.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Sat2Vidabstract.png)

- Contributions:
1) We present the **first** work for satellite-to-ground video synthesis from a single satellite image with a trajectory.
2) We propose a novel cross-view video synthesis method that ensures both spatial and temporal consistency by explicitly modeling a cross-frame correspondence using a 3D point cloud representation and building projective geometry constraints into our network architecture.

- structure: As for synthesis in the 3D space, we implement a cascaded network architecture with two hourglass modules to generate pointwise coarse and fine features from semantics and per-class latent vectors, followed by projection to frames and an upsampling module to obtain the final realistic video.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Sat2Vidstructure.png)

- results：

metrics: **(PSNR, SSIM, sharpness difference, PAlex, PSqz, PVGG denote the evaluation results based on the
backbone of AlexNet, SqueezeNet and VGG.)**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Sat2Vidresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Sat2Vidresult1.png)

- analysis:  we presented a multi-stage pipeline that takes as input a single satellite image with a given trajectory, and generates a street-view panoramic video with both geometrical and temporal consistency constrained in a 3D point cloud. 

-**Limitation**: Since the proposed method builds on the height estimation and semantic segmentation of the satellite image, the final synthesized video may suffer from some geometric inconsistency for the potential inaccurate estimated height and semantics. Besides, our method also fails to handle buildings with overhanging structures such as overpasses or protruding roofs because they cannot be well represented in the 2.5D height map from the top view. Furthermore, the point cloud size will explode with increasing numbers of video frames, leading to potential memory problems in the 3D convolutions.
