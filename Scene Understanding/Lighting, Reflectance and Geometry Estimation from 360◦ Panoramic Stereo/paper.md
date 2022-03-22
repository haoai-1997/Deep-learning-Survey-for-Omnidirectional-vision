## Lighting, Reflectance and Geometry Estimation from 360◦ Panoramic Stereo

- year: 2021

- dataset：  **Structured3D(synthetic indoor dataset)**  

- We propose a method for estimating high-definition spatially-varying lighting, reflectance, and geometry of a scene from 360◦ stereo images.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LGRabstract.png)

- Contributions:

1) A near-field environment light that can generate spatially-varying and 3D coherent high-definition illumination maps when given any 3D location within the scene.
2) A deep learning model that can estimate the reflectance and surface normal of the entire scene.
3) A rendering and refinement model that leverages the physical constraints between lighting and geometry to jointly estimate a finer reflectance.

- structure:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LGRstructure.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LGRstructure1.png)


- results：
To demonstrate ZInD’s benefits, we benchmark with **(HorizonNet)** on room layout estimation from single panoramas and multi-view registration.
metrics: **(sMSE for reflectance and MAE in degrees for normal.)**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LGRresult.png)


- analysis: we jointly estimate spatially-varying and 3D coherent lighting in high-definition, reflectance, and geometry of the entire scene. Our lighting model accurately reconstructs 3D illumination maps, enabling mirror-like objects to be inserted in the scene with realistic effect. We also leverage the physical constraints between the lighting and geometry to infer both surface reflectances and normals of the environment.
