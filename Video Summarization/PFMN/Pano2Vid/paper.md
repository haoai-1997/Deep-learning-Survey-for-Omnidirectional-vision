## Pano2Vid: Automatic Cinematography for Watching 360-degree Videos


- year: 2016

- dataset: Pano2Vid dataset (self-collected)

- Abstract: we propose to predict the depth map of a monocular 360◦ image by mimicking both peripheral and foveal vision of the human eye. To this end, we adopt a two-branch neural network lever- aging two common projections: equirectangular and cubemap projections.
- Contributions:
  (1) We propose an end-to-end two-branch network, which incorporates both equirectangular and cubemap projections, to mimic the combination of peripheral and foveal vision of the human eye, respectively.
  (2) To share the information of different projections, we propose a bi-projection fusion procedure with learnable masks to balance the information from two projections.
  (3) We propose spherical padding to extend the field-of-view of cubemap projection and reduce the boundary inconsistency of each face.

- Structure: BiFuse

<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/BiFuse.png" width="70%" height="70%">

- Results：
  <img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/BiFuse_exp1.png" width="50%" height="50%">
  <img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/BiFuse_exp2.png" width="50%" height="50%">

-Analysis: Utilize two projection formats of 360-degree images to better extracting and fusing information.
