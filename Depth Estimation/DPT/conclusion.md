## Improving 360◦ Monocular Depth Estimation via Non-local Dense Prediction Transformer and Joint Supervised and Self-supervised Learning
- conference: CVPR, 2021

- dataset: Stanford and 3D60.

- abstract: we propose 360◦ monocular depth estimation methods which improve on the areas that limited previous studies. 
First, we introduce a self-supervised 360◦ depth learning method that only utilizes gravity-aligned videos. Second, we propose a joint learning scheme realized by combining supervised and self-supervised learning. Third, we propose a non-local fusion block, which can further retain the global information encoded by vision transformer when reconstructing the depths. 

- contributions: 
(1) We propose a self-supervised method for the learning of depth that only utilizes gravity-aligned video sequences.
(2) we propose a joint learning scheme realized by combining supervised and self-supervised learning.
(3) we propose a non-local fusion block which improves on the areas missed by vision transformers for dense prediction.
(4) Our approaches achieve significant improvements over previous works on several benchmarks, thus establishing a state of the art.

- Framework:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/depth%20estimation/DPT_framework.png)

- results:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/depth%20estimation/DPT_result.png)
