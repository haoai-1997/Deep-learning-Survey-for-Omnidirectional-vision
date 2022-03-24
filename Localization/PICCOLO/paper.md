## PICCOLO: Point Cloud-Centric Omnidirectional Localization

- year: 2021

- dataset: Stanford2D-3D-S dataset, OmniScenes dataset (self-collected), and MPO dataset

- Abstract: 
We present PICCOLO, a simple and efficient algorithm for omnidirectional localization. Given a colored point cloud and a 360-degree panorama image of a scene, our objective is to recover the camera pose at which the panorama image is taken.
- Contributions:
  (1) We introduce PICCOLO, a simple yet effective omnidirectional localization algorithm.
  (2) The gradient of our proposed sampling loss can be effi- ciently obtained with differentiable sampling
  (3) In addition, we introduce a new dataset called OmniScenes to highlight the practicality of PICCOLO.

<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PICCOLO.png" width="70%" height="70%">

- Results：
  <img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PICCOLO_exp1.png" width="50%" height="50%">
  <img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PICCOLO_exp2.png" width="50%" height="50%">

-Analysis: This method is not data-driven and can be implemented efficiently. They also provide a dataset named "OmniScenes".
