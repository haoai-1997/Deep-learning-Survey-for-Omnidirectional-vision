## Learning Spherical Convolution for Fast Features from 360°Imagery

- year: 2018

- dataset：  **(360° PASCAL)** and  **(Pano2Vid)** 

- abstract: We propose tolearna spherical convolutional networkthat translates a planar CNN to process360°imagery directly in its equirectan-gular projection. Our approach learns to reproduce the flat filter outputs on360°data, sensitive to the varying distortion effects across the viewing sphere
- Contributions:
 1) efficient feature extraction for 360°images and video
 2) the ability to leverage powerful pre-trained networks researchers have carefully honed(together with massive labeled image training sets) for perspective images. 

- structure：learn spherical convolutions in equirectangular projection given a target networktrained on perspective images
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/leanring_sph_conv.png)
- results：
metrics: **(Network output error, Detector network performance, Proposal network performance)**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/sph_conv_detection.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/sph_conv_outputerror.png)


- analysis: Our solution entails a new form of **(distillation)** across camera projection models. Compared to current practices for feature extraction on 360°images/video, spherical convolution benefits efficiency by avoiding performing multiple perspective projections, and it benefits accuracy by adapting kernels to the distortions in equirectangular projection.
