## Distortion-Aware Convolutional Filters for Dense Prediction in Panoramic Images

- year: 2021

- dataset: Stanford2D3D dataset, Matterport3D dataset, and 3D60 dataset

- Abstract: 
We introduce a novel deep neural network to estimate a depth map from a single monocular indoor panorama. The network directly works on the equirectangular projection, exploiting the properties of indoor 360-degree images.
- Contributions:
(1) We introduce a slice-based representation of an omni-directional image; 
(2) We specialize and refine feature flattening, which has proven to be effective to regress one-dimensional tensors, for bi-dimensional depth encoding;
(3) We introduce, for depth estimation from a single image, a LSTM multi-layer module to effectively recover long and short term spatial relationships between slices in the presence of a large number of features per slice due to the concatenation of multiscale representations.

- Structure: ResNet and RNN

<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SliceNet.png" width="70%" height="70%">

- Results：
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SliceNet_exp1.png" width="50%" height="50%">

-Analysis: SliceNet is designed specifically for ERP. This work also provides a RNN scheme to construct relationships between slices.



