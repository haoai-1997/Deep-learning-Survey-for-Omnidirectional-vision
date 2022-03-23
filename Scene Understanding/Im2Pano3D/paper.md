## Im2Pano3D: Extrapolating 360° Structure and Semantics Beyond the Field of View

- year: 2018

- dataset：  **(synthetic dataset : SUNCG and Matterport3D)**  

- abstract: We present Im2Pano3D, a convolutional neural network that generates a dense prediction of 3D structure and a probability distribution of semantic labels for a full 360◦ panoramic view of an indoor scene when given only a partial observation (≤ 50%) in the form of an RGB-D image. 
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Im2Pano3Dabstract.png)

- Contributions:
1) We propose the task of semantic-structure view extrapolation and present Im2Pano3D, a unified framework able to produce a complete room structure and semantic labeling when given a partial observation of a scene. 

-structure: Our network architecture follows an encoder-decoder structure, where the encoder produces a latent vector from an input panorama with missing regions, and the decoder uses that latent vector to produce an output panorama where the missing regions are filled

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Im2Pano3Dstructure.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Im2Pano3Dstructure1.png)

- results：

metrics: **(Normal angle: the mean and median angles, Surface distance: the mean and median L2 distances, Probability over ground truth (PoG), Class existence (exist), Class size (size), Earth Mover’s Distance (EMD), IoU, Accuracy (acc), Inception score (incept.))**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Im2Pano3Dresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Im2Pano3Dresult1.png)

- analysis:  Im2Pano3D, a unified framework to produce a complete room structure and semantic estimation
conditioned on a partial observation of the scene。

**Possible future directions** may include: explicitly modeling semantics at the instancelevel as opposed to category-level, and exploring alternative data representations that consider occluded regions.
