## Eliminating the Blind Spot: Adapting 3D Object Detection and Monocular Depth Estimation to 360◦ Panoramic Imagery

- year: 2018

- dataset：  **(the crowd-funded street-level imagery of Mapillary as well as quantitatively using synthetic data generated using the CARLA automotive environment simulator.)**  

- abstract:  We present an approach to adapt contemporary deep network architectures developed on conventional rectilinear imagery to work on equirectangular 360◦ panoramic imagery. we adapt contemporary automotive dataset, via style and projection transformations, to facilitate the cross-domain retraining of contemporary algorithms for panoramic imagery and then retrain and adapt existing architectures to recover scene depth and 3D pose of vehicles from monocular panoramic imagery without any panoramic training labels or calibration parameters. 

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/EBSabstract.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/EBSstructure.png)

- Contributions:
1) a novel approach to convert deep network architectures operating on rectilinear images for equirectangular panoramic images based on style and projection transformations;
2) a novel approach to reuse and adapt existing datasets in order to train models for panoramic imagery;
3) the subsequent application of these approaches for monocular 3D object detection using a simpler formulation than earlier work, additionally operable on conventional imagery without modification; further application of these techniques to monocular depth recovery using an adaptation of the rectilinear imagery approach of Godard et al.

- structure: 

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/EBSabstract1.png)

- results：
metrics: **( mAP, Depth Error Metrics (Abs. rel,Sq. rel, RMSE ,RMSE log), δ < 1.25)**

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/EBSresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/EBSresult1.png)


- analysis: We have adapted existing deep architectures and training datasets, proven on
forward-facing rectilinear camera imagery, to perform on panoramic images. The
approach is based on domain adaptation using geometrical and style transforms
and novel updates to training loss to accommodate panoramic imagery. Our
approach is able to recover the monocular depth and the full 3D pose of vehicles.


