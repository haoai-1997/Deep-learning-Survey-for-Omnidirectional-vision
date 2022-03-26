## Corners for Layout: End-to-End Layout Recovery From 360 Images

- year: 2020

- dataset：  **(SUN360 and Stanford (2D-3D-S) in equirectangular projection (360◦).)**  

- abstract: In this work we present CFL (Corners for Layout), the first end-to-end model that predicts layout corners for 3D layout recovery on 360◦ images.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/CFLabstract.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/CFLabstract1.png)
- Contributions:
1) In this work, we present Corners for Layout (CFL), the first end-to-end neural network that predicts a map of the corners of the room to directly obtain the 3D layout from a single 360◦ image. This makes CFL **more than 100 times faster than the state of the art**, while still outperforming the accuracy of current approaches.

2) our proposal is not limited by typical scene assumptions, meaning that it can predict complex geometries, such as rooms with more than four walls or non strict Manhattan structures.

3） we propose a novel implementation of the convolution for 360◦ images in the equirectangular projection.

- structure:  The proposed FCN follows the encoder-decoder structure and builds upon ResNet-50. We replace the final fullyconnected layer with a decoder that jointly predicts layout edges and corners locations already refined. 
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/CFLstructure.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/CFLstructure1.png)

- results：

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/CFLresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/CFLresult1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/CFLresult2.png)

- analysis: In this work we present CFL, the first end-to-end algorithm for layout recovery in 360◦ images. 
**The first one** implemented using Standard Convolutions, reduces the computation in 100times and it is very suitable for images taken with a tripod (recommended if the time is a critical issue). 
**The second one** uses our proposed implementation of Equirectangular Convolutions that adapt their shape to the equirectangular projection of the spherical image (recommended if looking for robustness and better generalization).


