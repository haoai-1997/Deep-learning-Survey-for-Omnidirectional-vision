## 3D Manhattan Room Layout Reconstruction from a Single 360 Image

- year: 2019

- dataset: Matterport3D Dataset

- abstract:
Recent approaches for predicting layouts from360◦ panoramas produce excellent results. These approaches build on a common framework consisting of three steps: a pre-processing step based on edge-based alignment, prediction of layout elements, and a post-processing step by fitting a 3D layout to the layout elements. Until now, it has been difficult to compare the methods due to multiple different design decisions, such as the encoding network (e.g., Seg- Net or ResNet), type of elements predicted (e.g., corners, wall/floor boundaries, or semantic segmentation), or method of fitting the 3D layout. To address this challenge, we summarize and describe the common framework, the variants, and the impact of the design decisions. For a complete evaluation, we also propose extended annotations for the Matterport3D dataset [3], and introduce two depth-based evaluation metrics.

- contribution:
(1) Two frameworks, LayoutNet v2 and DuLa-Net v2, which extend the corresponding state-of-the-art approaches of 3D Manhattan layout reconstruction from an RGB panoramic image.
(2) Analysis of the effects of encoders,post-processing steps, performance for different room shapes, and time consumption.
(3) Matterport3D dataset with general Manhattan layout annotations which contain panoramas depicting room shapes of various complexity.

- structure:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/3D reconstruction/3D_Manhattan_Room_Layout_framwork_1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/3D reconstruction/3D_Manhattan_Room_Layout_framwork_2.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/3D reconstruction/3D_Manhattan_Room_Layout_framwork_3.png)