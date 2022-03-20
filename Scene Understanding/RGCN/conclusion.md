## DeepPanoContext: Panoramic 3D Scene Understanding with Holistic Scene Context Graph and Relation-based Optimization


- conference: ICCV, 2021

- dataset: the proposed DensePASS and Cityscapes, WildDash.

- abstract: Firstly, this work builds a novel dataset DensePASS for semantic segmentation in 360 degree domain. Secondly, this paper introduces P2PDA - a generic framework for PINHOLE→PANORAMIC semantic segmentation which addresses the challenge of domain divergence with different variants of attention-augmented domain adaptation modules, enabling the transfer in output-, feature-, and feature confidence spaces. P2PDA intertwines uncertainty-aware adaptation using confi- dence values regulated on-the-fly through attention heads with discrepant predictions. The proposed method performs greater on the novel dataset DensePASS than other baseline methods.

- contributions: 
(1)We create and publicly release DENSEPASS – a new benchmark for panoramic semantic segmentation collected from locations all around the world and densely annotated with 19 classes in accordance to the pinhole camera dataset Cityscapes to enable proper PINHOLE→PANORAMIC evaluation.
(2)We propose a generic P2PDA framework and investigate various DA modules both in a separate and joint man- ner, validating their effectiveness with various networks designed for self-driving scene segmentation.
(3) We advocate attentional domain adaptation by integrating attention-augmented adversarial- and attention-regulated self-learning adaptation, verifying that uncertainty-aware distillation with adapted knowledge can further boost the DA performance significantly.
(4)With the DANet baseline, our P2PDA framework achieves +13.5% and +16.2% mIoU gains by adapting from Cityscapes and further adding WildDash.

- Framework:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/semantic%20Segmentation/P2PDA_framework.png)

- RCDAM module

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/semantic%20Segmentation/P2PDA_RCDAM.png)

- SDAM module

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/semantic%20Segmentation/P2PDA_SDAM.png)

- ADAM module

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/semantic%20Segmentation/P2PDA_ADAM.png)

- results:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/semantic%20Segmentation/P2PDA_result.png)
