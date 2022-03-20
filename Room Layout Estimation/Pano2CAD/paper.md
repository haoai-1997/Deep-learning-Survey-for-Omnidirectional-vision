## Pano2CAD: Room Layout From A Single Panorama Image

- year: 2017

- dataset: SUN360 dataset  and a synthetic dataset of 88 rooms

- abstract: Assuming Manhattan World geometry, weformulate the task as an inference problem in which we es-timate positions and orientations of walls and objects. Themethod combines surface normal estimation, 2D object de-tection and 3D object pose estimation. 
- Contributions:
(1) We follow a Manhattan World assumption,reconstructing the complete shape of the room. 
(2) Objectlocation and pose is estimated using top-down object detec-tion and 3D pose estimation using a public library of 3Dmodels
(3) We introduce a context prior for object and wallrelationships in order to sample plausible room hypotheses.

- structure: Generative model

![image](https://github.com/VLISLAB/360-DL-Survey/Images/Pano2CAD.png)

- results：
![image](https://github.com/VLISLAB/360-DL-Survey/Images/Pano2CAD_result.png)
![image](https://github.com/VLISLAB/360-DL-Survey/Images/Pano2CAD_sundataset.png)

-analysis: （对文章的分析）
