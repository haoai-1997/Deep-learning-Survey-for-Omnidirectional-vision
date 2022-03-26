## Deep Upright Adjustment of 360 Panoramas Using Multiple Roll Estimations

- year: 2018

- dataset：  **(Jung et al.’s test dataset and a new test dataset by collecting four scene categories from SUN360 dataset)**  

- abstract:  To automatically correct such mis-oriented 360 panoramas, this paper proposes a novel upright adjustment framework based on a convolutional neural network. Instead of directly predicting the 3D rotation of the camera on a given panorama image, our method estimates the rotation by analyzing the projected 2D rotations of multiple images sampled from the panorama.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DUAabstract.png)

- Contributions:
1) we propose a 3D camera rotation estimation method for 360 spherical panoramas by exploiting the geometric relationship between a 3D rotation and projected 2D rotations.

2) we generate a large-scale labeled narrow field-of-view image dataset that can be used for supervised learning of roll (in-plane image rotation) angle estimation, by cropping 360 spherical panoramas using various view orientations.


- structure: 
we propose a novel automatic upright adjustment framework for 360 panorama images based on a deep convolutional neural network. Instead of using hand-crafted features extracted from a given 360 spherical panorama, our method indirectly estimates the camera rotation by analyzing the projected 2D rotations estimated from multiple narrow field-of-view images sampled from the input panorama. Our proposed framework exploits the semantically trained CNN features rather than straight line segments and vanishing points, and can robustly handle a variety of scenes no matter whether they follow the Manhattan or Atlanta world assumption.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DUAstructure.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DUAstructure1.png)

- results：
metrics: **( MAE, the average absolute angular error)**

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DUAresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DUAresult1.png)


- analysis: By exploiting the relationship between a 3D camera rotation and projected 2D rotations of multiple sampled images, our method accurately estimates the 3D camera rotation relative to the scene from a given single 360 panorama. Differently from existing methods based on straight lines and vanishing points, our method uses a CNN for 2D roll estimation by training it using a massively generated 2D image dataset, enabling the network to learn semantic upright directions (e.g., standing people).


