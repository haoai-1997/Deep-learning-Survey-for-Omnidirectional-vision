## Learning SO(3) Equivariant Representationswith Spherical CNNs

- year: 2018

- dataset： retrieval dataset **(SHREC’17)** and a classification dataset **(ModelNet40)**  (点云数据集)

- abstract: Addressing the problem of 3D rotation equivariance in con-volutional  neural  networks. Authors model 3D data with multi-valued spherical functions and we propose a novel spherical convolutionalnetwork that implements exact convolutions on the sphere by realizingthem in the spherical harmonic domain. We apply a novel pooling on the spectral domain and our operations are independent of theunderlying spherical resolution throughout the network.
- Contributions:
(1) We propose the first neural network based on spherical convolutions. 
(2) We introduce pooling and parameterization of filters in the spectral domain,with enforced spatial localization and capacity independent of the resolution.
(3) Our network has much lower capacity than non-spherical networks appliedon 3D data without sacrificing performance.

structure：基于Group Convolution, 引入Spherical harmonics
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SO(3)_representation.png)
results：
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SO(3)_classification_result.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SO(3)_retrieval_result.png)

analysis: Resulting filters have local sym-metry and are localized by enforcing smooth spectra; much lower capacity and without requiring data augmen-tation.此方法用在点云数据集上未被用于360 image
