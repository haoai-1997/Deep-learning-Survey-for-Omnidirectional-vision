## Spatially-Varying Outdoor Lighting Estimation from Intrinsics

- year: 2021

- dataset：  **(Synthetic Dataset : SOLID-Img;  a small real dataset )**  

- abstract: We present SOLID-Net, a neural network for spatiallyvarying outdoor lighting estimation from a single outdoor image for any 2D pixel location. we generate spatially-varying local lighting environment maps by combining global sky environment map with warped image information according to geometric information estimated from intrinsics.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SOLIDabstract.png)

- Contributions:
1) We train a single-in-multi-output CNN to decompose an input image into intrinsic parts: albedo (material-related), normal and plane distance (geometry-related), and shadow (lightingrelated). 
2) With the estimated geometry from decomposed intrinsics, we further warp the input image and estimated shadow map with limited FOV to a spherical projection centered at the target location.
3) We use the Blender SceneCity [2] to create city models that contain a large set of outdoor scenes and render a synthetic outdoor lighting estimation dataset with labeled location information and corresponding lighting effects using a physically-based path-tracer to facilitate the training of our network.

-structure: we propose a two-stage framework to jointly solve these problems by: 1) proposing an intrinsic image decomposition network (denoted asINet) that takes a limited FOV image as input and estimates its intrinsic components as well as a global sky environment map and 2) designing a panoramic completion module (denoted as P-Net) that estimates local lighting from outputs in the previous stage and the input location.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SOLIDstructure.png)

- results：
metrics: **( mean absolute error (MAE) on the HDR sky environment map, angular error on the sun position and sun azimuth/elevation angles, and SSIM on the detailed local lighting as error metrics)**

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SOLIDresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SOLIDresult1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SOLIDresult2.png)

- analysis:  We present the **first** end-to-end outdoor spatially-varying lighting estimation framework and demonstrate it significantly outperforms previous works via extensive evaluations on both synthetic and real datasets.

- **Limitation**:  
1) Due to the material diversity gap between synthetic and real data, the intrinsic decomposition results on real data may not be as accurate as those on synthetic data.
2) Although SOLID-Net estimates HDR lighting environment map to support realistic relighting effects, our lighting model is not suitable for generating animations that are sensitive at harsh lighting boundaries.
