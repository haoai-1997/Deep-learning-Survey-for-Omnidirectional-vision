## Rotation Equivariant Graph Convolutional Network for Spherical Image Classification

- year: 2020

- dataset：  **(the Spherical MNIST (S-MNIST), Spherical CIFAR-10 (S-CIFAR-10))**  

- abstract:  In this paper, we generalize the grid-based CNNs to a non-Euclidean space by taking into account the geometry of spherical surfaces and propose a Spherical Graph Convolutional Network (SGCN) to encode rotation equivariant representations. 
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SGCNabstract.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SGCNabstract1.png)
- Contributions:

In this paper, we propose a Spherical Graph Convolutional Network (SGCN) to encode rotation-equivariance for spherical image analysis. Specially, we develop a graph convolutional layer through exploring the isometric transformation equivariance of the graph Chebyshev polynomial filters which is isotropy, a hierarchical pooling layer to exploit the multi-scale resolutions of the spherical images and keep the rotation-equivariance, and a transition layer to calculate the rotation-invariant statistics across multiple feature maps of the hierarchical pooling layer.

- structure: 

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SGCNstructure.png)

- results：
metrics: **(equivariance error, Accuracy)**

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SGCNresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SGCNresult1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SGCNresult2.png)

- analysis: In this paper, we have presented the spherical graph convolutional network (SGCN) based on GICOPix to encode rotation-equivariance for spherical image analysis. We proposed a spherical graph construction criterion and constructed the spherical graph based on GICOPix with the minimum degree of irregularity. 


