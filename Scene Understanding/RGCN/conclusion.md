## DeepPanoContext: Panoramic 3D Scene Understanding with Holistic Scene Context Graph and Relation-based Optimization


- conference: ICCV, 2021

- dataset: the proposed DensePASS and Cityscapes, WildDash.

- abstract: Firstly, this work builds a novel dataset DensePASS for semantic segmentation in 360 degree domain. Secondly, this paper introduces P2PDA - a generic framework for PINHOLE→PANORAMIC semantic segmentation which addresses the challenge of domain divergence with different variants of attention-augmented domain adaptation modules, enabling the transfer in output-, feature-, and feature confidence spaces. P2PDA intertwines uncertainty-aware adaptation using confi- dence values regulated on-the-fly through attention heads with discrepant predictions. The proposed method performs greater on the novel dataset DensePASS than other baseline methods.

- contributions: 
(1) We pro-pose the first deep learning based pipeline for holistic 3D scene understanding that recovers 3D room layout and de-tailed shape, pose, location for objects in the scene from a single color full-view panorama image. 
(2) We design a novel context model that predicts the relationship among objects and room layout, followed by a new differentiable relationship-based optimization module to refine the initial results.
(3) A new dataset is created for total panoramic 3D scene un-derstanding.
(4) Our model achieves the state-of-the-art perfor-mance on both geometry accuracy and 3D object arrange-ment.

- Framework:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/scene%20understanding/RGCN_framework.png)

- results:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/scene%20understanding/RGCN_result.png)
