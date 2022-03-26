## Recovering 3D existing-conditions of indoor structures from spherical images (traditional)

- year: 2018

- dataset：  **(a variety of indoor scenes, including real-world residential and commercial buildings and various scenes from the public SUN360 dataset; )**  

- abstract:  We present a vision-based approach to automatically recover the 3D existing-conditions information of an indoor structure, starting from a small set of overlapping spherical images. 

- Contributions:
We first recover the underlying 3D structure as interconnected rooms bounded by walls. This is done by combining geometric reasoning under an Augmented Manhattan World model and Structurefrom-Motion. Then, we create, from the original registered spherical images, 2D rectified and metrically scaled images of the room boundaries. Using those undistorted images and the associated 3D data, we automatically detect the 3D position and shape of relevant wall-, floor-, and ceiling-mounted objects, such as electric outlets, light switches, air-vents and light points. 

- structure: 

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/R3Dstructure.png)

- results：

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/R3Dresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/R3Dresult1.png)


- analysis: 
First of all, we expand over purely single view by exploiting multiple views to automatically reconstruct global and consistent multi-room environments through geometric reasoning.
Second, we exploit the reconstructed model to enhance image-based search for the elements located on room boundaries. 


