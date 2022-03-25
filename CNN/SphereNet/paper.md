## SphereNet: Learning Spherical Representations for Detection and Classification in Omnidirectional Images

- year: 2018

- dataset：  **(Omni-MNIST; FlyingCars; OmPaCa)**  

- abstract:  In this work, we present SphereNet, a novel deep learning framework which encodes invariance against such distortions explicitly into convolutional neural networks. Towards this goal, SphereNet adapts the sampling locations of the convolutional filters, effectively reversing distortions, and wraps the filters around the sphere

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphereNetabstract.png)

- Contributions: 
1) We introduce SphereNet, a framework for learning spherical image representations by encoding distortion invariance into convolutional filters. SphereNet retains the original spherical image connectivity and, by building on regular convolutions, enables the transfer of perspective CNN models to omnidirectional inputs.
2) We improve the computational efficiency of SphereNet using an approximately uniform sampling of the sphere which avoids oversampling in the polar regions.
3) We create two novel semi-synthetic and real-world datasets for object detection in omnidirectional images。


- structure: 

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphereNetstructure.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphereNetstructure1.png)
- results：

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphereNetresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphereNetresult1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphereNetresult2.png)

- analysis: SphereNet lifts 2D convolutional neural networks to the surface of the unit sphere. By applying 2D convolution and pooling filters directly on the sphere’s surface, our model effectively encodes distortion invariance into the filters of convolutional neural networks.


