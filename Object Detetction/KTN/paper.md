## Kernel Transformer Networks for Compact Spherical Convolution

- year: CVPR 2019

- dataset: introduce four training dataset, namely UrbanCity360(synthetic), Archinterior360(synthetic), HungHom360(real) and Lab360(real) 

- abstract: We present the Kernel Trans- former Network (KTN) to efficiently transfer convolution kernels 
from perspective images to the equirectangular pro- jection of360◦ images. Given a source CNN for 
perspective images as input, the KTN produces a function parameter- ized by a polar angle and kernel as output. 
Given a novel 360◦ image, that function in turn can compute convolutions for arbitrary layers and kernels 
as would the source CNN on the corresponding tangent plane projections. Distinct from all existing methods,
KTNs allow model transfer: the same model can be applied
to different source CNNs with the same base architecture. 
This enables application to multiple recognition tasks without re-training the KTN

- contributions:
(1) KTN are its transferability and compactness—both of which owe to our function-based design.
(2)Results show KTN models are orders of magnitude smaller than the most accurate competitor

- structure:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/object%20detection/KTN_framework.png)

- results:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/object%20detection/KTN_result.png)
