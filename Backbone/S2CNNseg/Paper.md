## Equivariance versus Augmentation for Spherical Images
- **year**: 2022

- **Publication Conference**: ICML

- **Experimental Dataset**:  spherical MNIST, Fashion-MNIST (Semantic Segmentation)

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; To compare the performance of the group equivariant networks known as S2CNNs and standard non-equivariant CNNs trained with an increasing amount of data augmentation. 

- **Attractive points**:

&nbsp; &nbsp; &nbsp; &nbsp; We conduct comparisons for several datasets to elucidate the influence of the type and complexity of the task on the performance. Our overall aim is to investigate whether equivariant architectures offer an inherent advantage over data augmentation in non-equivariant CNN models. In fact, the theoretical development applies to any homogeneous space, and the question of equivariance versus data augmentation is relevant also in the general setting.

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; 1) define a new group equivariant CNN layer, as:
![image](https://user-images.githubusercontent.com/101921451/205205927-5f4716d5-3cbd-42d9-9145-164515fa30de.png)
designed for the task of semantic segmentation for arbitrary Lie groups G. And by adding a layer to S2CNN architecture, S2CNN allows for equivariant outputs on the sphere as required for semantic segmentation tasks.

&nbsp; &nbsp; &nbsp; &nbsp; 2) Some observation: non-equivariant classification models require considerable data augmentation to reach the performance of smaller equivariant networks; semantic segmentation models saturates well below that of equivariant models as the amount of data augmentation is increased.

&nbsp; &nbsp; &nbsp; &nbsp; 3) Most importantly, this work systematically compare data augmentation with increased training data sizes for different tasks, datasets and several non-equivariant models with an equivariant architecture.

- **Proposing Framework**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/S2CNNseg.png" width="800" height="200">
</div>


- **Experimental Results**：

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/S2CNNseg_results.png" width="400" height="400"><img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/S2CNNseg_results1.png" width="400" height="400">
</div>

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/S2CNNseg_results2.png" width="400" height="400"><img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/S2CNNseg_results3.png" width="400" height="400">
</div>
