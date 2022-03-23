## Joint 3D Layout and Depth Prediction from a Single Indoor Panorama Image

- year: 2020

- dataset: Stanford2D3D dataset (for depth estimation), PanoContext dataset (for 3D layout prediction)

- Abstract: In this paper, we propose a method which jointly learns the layout prediction and depth estimation from a single indoor panorama image.
- Contributions:
(1) We propose a novel neural network pipeline which jointly learns layout pre- diction and depth estimation from a single indoor panorama image. We show that layout and depth estimation tasks are highly correlated and joint learn- ing improves the performance for both tasks.
(2) We show that leveraging the layout depth map as an intermediate repre- sentation improves the layout prediction performance and refines the depth estimation.
(3) The proposed method outperforms the state-of-the-art methods for both layout prediction and depth estimation on the challenging real-world dataset Stanford 2D-3D and PanoContext dataset for layout prediction.
  
- Structure: ResNet

<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/joint3d.png" width="70%" height="70%">

- Results：
  <img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/joint3d_1.png" width="50%" height="50%">
  <img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/joint3d_2.png" width="50%" height="50%">

-Analysis: This work joints learn layout prediction and depth estimation. They estimate the layout depth as an intermediate representation of the network which encompasses the geometric information needed for both tasks.
