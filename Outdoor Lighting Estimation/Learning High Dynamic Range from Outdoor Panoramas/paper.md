## Learning High Dynamic Range from Outdoor Panoramas

- year: 2017

- dataset：  **(synthetic data Laval HDR Sky Database; a novel collected dataset of real photographs with ground truth )**  

- abstract: In this work, we propose an alternative approach. We first capture lighting with a regular, LDR omnidirectional camera, and aim to recover the HDR after the fact via a novel, learning-based inverse tonemapping method. We propose a deep autoencoder framework which regresses linear, high dynamic range data from non-linear, saturated, low dynamic range panoramas. 
<!-- ![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LHDRabstract.png) -->

- Contributions:
1) we present a full end-to-end learning approach which directly regresses HDR from LDR information in an outdoor panorama.
2) a novel dataset of real LDR panoramas and associated HDR ground truth.
3) to show the applicability of our approach on three novel applications: single shot light probe, visualizing virtual objects and image matching in large LDR panorama database.

- structure: As for synthesis in the 3D space, we implement a cascaded network architecture with two hourglass modules to generate pointwise coarse and fine features from semantics and per-class latent vectors, followed by projection to frames and an upsampling module to obtain the final realistic video.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LHDRabstract.png)

- results：

metrics: **(MAE on the HDR sky; RMSE on the sun elevation;  RMSE on the “spiky sphere” ender ; RMSE on the predicted sun intensity )**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LHDRresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LHDRresult1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LHDRresult2.png)

- analysis:  We present a full end-to-end learning approach to estimate the extremely high dynamic range of outdoor lighting from a single, LDR 360◦ panoram. Our main insight is to exploit a large dataset of synthetic data composed of a realistic virtual city model, lit with real world HDR sky light probes, to train a deep convolutional autoencoder. 

- **Limitation**: 
1) we note a certain sensitivity to the tonemapping function of the input LDR.
2) A second limitation is that our approach is limited to outdoor scenes and the sun, when visible, needs to be centered in the panorama.
3) the resolution of the output is limited at 64 × 128, which, while sufficient for relighting applications, cannot extrapolate the HDR information in a full-resolution LDR background image.

- future: the adaptation of the network to learn high resolution HDR textures from limited field-of-view LDR images.
