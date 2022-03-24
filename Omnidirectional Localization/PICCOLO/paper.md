## PICCOLO: Point Cloud-Centric Omnidirectional Localization


- year: 2021

- dataset：**(OmniScenes; Stanford2D-3D-S and Multi-Modal Panoramic 3D Outdoor (MPO) dataset)**  

- abstract: We present PICCOLO, a simple and efficient algorithm for omnidirectional localization. Given a colored point cloud and a 360˝ panorama image of a scene, our objective is to recover the camera pose at which the panorama image is taken. Our pipeline works in an off-the-shelf manner with a single image given as a query and does not require any training of neural networks or collecting ground-truth poses of images. Instead, we match each point cloud color to the holistic view of the panorama image with gradientdescent optimization to find the camera pose
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PICCOLOabstract.png)

- structure:
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PICCOLOstructure.png)

- results：
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PICCOLOresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PICCOLOresult1.png)

