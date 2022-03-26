## Orientation-Aware Semantic Segmentation on Icosahedron Spheres

- year: 2019

- dataset: 2D3DS dataset(which consists of 1413 equirectangular RGB-D images), Omni-SYNTHIA

- abstract:
In our work, we propose an orientation-aware CNN frame-work for the icosahedron mesh.
Our representation allows for fast network operations, as our design simplifies to standard network operations of classical CNNs, but under consideration of north-aligned kernel convolutions for featureson the sphere.

- contributions:
(1) We propose and implement a memory efficient icosahedron-based CNN framework for spherical data.
(2) We introduce fast interpolation for orientation-aware filter convolutions on the sphere
(3) We present weight transfer from kernels learned through classical CNNs, applied to perspective data.

- structure:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/icosahedron_spheres_process.png)

- loss function

cross-entropy loss

- result:
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/result_on_2D3DS.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/result_on_Omni-SYNTHIA.png)

- limitation

One limitation of the proposed approach is the poor segmentation accuracy for small objects (e.g. “pedestrian” and“cyclist”) which we attribute to unbalanced dataset.  
