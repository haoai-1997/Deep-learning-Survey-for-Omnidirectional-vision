## Panoramic Image Reflection Removal

- year: 2021

- dataset：  **(synthesis dataset selected from SUN RGB-D and Cityscapes)**  

- abstract: This work aims at reliving the content ambiguity between reflection and transmission scenes.  We propose a two-step approach to solve this problem, by first accomplishing geometric and photometric alignment for the reflection scene via a coarse-to-fine strategy, and then restoring the transmission scene via a recovery network.

- Contributions:

(1) We present the first work to explicitly relieve the content ambiguity for reflection removal using a
panoramic image.
(2) We solve the geometric and photometric misalignment between reflection scenes in panoramic and glass-reflected views, accompanying with high-fidelity transmission recovery after the alignment.
(3) We show that our method not only achieves superior performance advantage over single-image methods but also generalizes well to casual users without
panoramic cameras.


- structure:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PIRPstructure1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PIRPstructure2.png)
- results：
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PIRPresult1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PIRPresult2.png)


- analysis: We consider relieving the content ambiguity by taking a panoramic image as the input for **(reflection removal)**. We show that the major challenge of this problem is the geometric and photometric misalignment between the panoramic reflection scene and the glass-reflected reflection image, based on which a two-step solution composing of reflection alignment and transmission recovery is proposed.
