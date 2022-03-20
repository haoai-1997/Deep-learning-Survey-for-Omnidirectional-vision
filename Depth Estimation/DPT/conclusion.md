## Improving 360◦ Monocular Depth Estimation via Non-local Dense Prediction Transformer and Joint Supervised and Self-supervised Learning
- conference: CVPR, 2021

- dataset: Stanford and 3D60.

- abstract: Firstly, this work builds a novel synthetic dataset for scene understanding in 360 degree domain. Secondly, this work propose a novel method for panoramic 3D scene understanding which recovers the 3D room layout and the shape, pose, position, and semantic category for each object from a single full-view panorama image. In order to fully utilize the rich context information, we design a novel graph neural network based context model to pre- dict the relationship among objects and room layout, and a differentiable relationship-based optimization module to optimize object arrangement with well-designed objective functions on-the-fly. Realizing. The proposed method performs greater on the dataset than other baseline methods.

- contributions: 
(1) We pro-pose the first deep learning based pipeline for holistic 3D scene understanding that recovers 3D room layout and de-tailed shape, pose, location for objects in the scene from a single color full-view panorama image. 
(2) We design a novel context model that predicts the relationship among objects and room layout, followed by a new differentiable relationship-based optimization module to refine the initial results.
(3) A new dataset is created for total panoramic 3D scene un-derstanding.
(4) Our model achieves the state-of-the-art perfor-mance on both geometry accuracy and 3D object arrange-ment.

- Framework:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/depth%20estimation/DPT_framework.png)

- results:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/depth%20estimation/DPT_result.png)
