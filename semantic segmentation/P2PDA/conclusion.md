## Transfer beyond the Field of View: Dense Panoramic Semantic Segmentation via Unsupervised Domain Adaptation

- conference: IEEE Transactions on Intelligent Transportation Systems, 2021

- dataset: DensePASS

- abstract: the paper proposes a 360 monocular depth estimation pipeline - OmniFusion - to tackle the spherical distortion issue. And we propose a new framework to handle the discrepancy between patch-wise predictions. An iterative depth refinement mechanism is introduced to further refine the estimated depth based on the more accurate geometric features.

- contributions: 
(1)We present a 360 monocular depth prediction pipelinethat addresses the distortion issue via geometry-aware fusion and achieves the state-of-the-art performance. 
(2)We introduce a geometric embedding network to provide 3D geometric features to mitigate the discrepancyin patch-wise image features. 
(3)We incorporate a self-attention-based transformer toglobally aggregate patch-wise information which en-hances the estimation of the physical scale of depth. 
(4)We propose an iterative mechanism to further improvethe depth estimation with structural details.

- structure:
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/semantic%20Segmentation/P2PDA_framework.png)

- results:
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/OmniFusion_exp.png)
