## GLPanoDepth: Global-to-Local Panoramic Depth Estimation

- year: 2022

- dataset: three benchmark datasets -- 360D, Matterport3D and Stanford2D3D

- abstract: To solve the current methods fail to capture rich global contexts from the panorama and  the distortion of equirectangu-lar projection in the panorama,
the paper proposes Cubemap Vision Transformers(CViT), a new transformer-based architecture that can model long-range dependencies and extract distortion-free global features from the panorama.
To preserve important local features, we further design a convolution-based branch in our pipeline (dubbedGLPanoDepth) and fuse global features from cubemap vision transformers at multiple scales.

- contributions:
(1) we adopt cubemap projection and construct a new Cubemap Vision Transformers(CViT) to model long-range dependencies in spherical signals and extract distortion-free global features.
(2) A fully convolutional branch is employed to capture strong 2D local structures that are not well handled by pure transformers.
(3) These two features are fused at multiple scale using aGatedFusion Moduleto produce high-quality depth maps.

- structure
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/GLPanoDepth.png)

- loss function

  BerHu loss
  ![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/BerHuloss.png)

- result:
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/GLPanoDepth_result.png)



