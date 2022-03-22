## HorizonNet: Learning Room Layout with 1D Representation and Pano Stretch Data Augmentation

- year: 2019

- dataset: PanoContext dataset, and the extended Stanford 2D-3D dataset.

- Abstract: We represent room layout as three 1D vectors that encode, at each image column, the boundary positions of floor-wall and ceiling-wall, and the existence of wall-wall boundary. The proposed network, HorizonNet, trained for predicting 1D layout, outperforms previous state-of-the-art approaches. The designed post-processing procedure for recovering 3D room layouts from 1D predictions can automatically infer the room shape with low computation cost.
- Contributions:
(1) We introduce a 1D O(W) representation that encodes the whole-room layout for a panoramic scene. Training with such a representation allows our method to outperform previous state-of-the-art results, yet requires fewer parameters and less computation time.
(2) We propose a data augmentation mechanism called Pano Stretch Data Augmentation, which generates panorama images on the fly during training and im- proves the accuracy under all settings in our experiments. This data augmentation mechanism also has the potential for boosting other tasks (e.g., semantic segmentation, object detection) that directly work on a panorama.
(4) We show that leveraging RNNs in a layout predic- tion task is helpful for improving the accuracy. RNNs are able to capture the long-range geometric pattern of room layouts.
(5) Owing to the 1D representation and our efficient post-processing procedure, the computation cost of our model is very low, and the model can be easily extended to handle complex scenes with layouts other than cuboid-shaped or L-shaped.

- Structure: RNN

<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Horizonnet_1.png" width="70%" height="70%">
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Horizonnet_2.png" width="70%" height="70%">

- Results：
  <img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Horizonnet_exp1.png" width="50%" height="50%">

-Analysis: This work represents room layout as three 1D vectors, which not only has better performance, but also has low computation cost.
