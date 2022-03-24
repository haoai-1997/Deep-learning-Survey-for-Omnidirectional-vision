## Deep Multi Depth Panoramas for View Synthesis

- year: 2020

- dataset：  **(datasets are generated from the same 21 large-scale scenes, which consist of indoor and outdoor scenes modeled with high resolution textures and complex scene geometry)**  

- abstract: We propose a learning-based approach for novel view synthesis for multi-camera 360◦ panorama capture rigs. we present a novel scene representation—Multi Depth Panorama (MDP)—that consists of multiple RGBDα panoramas that represent both scene geometry and appearance. We demonstrate a deep neural network-based method to reconstruct MDPs from multi-camera 360◦ images. MDPs are more compact than previous 3D scene representations and enable high-quality, efficient new view rendering. 

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/MDPabstract.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/MDPabstract1.png)
- Contributions:
1) a 360◦ layered scene representation called Multi Depth Panorama (MDP), offering a more compact and versatile 3D representation than previous work.
2) a learning-based method to convert images from common 360◦ camera setups into our MDP representation.
3) an efficient novel view synthesis method based on MDP.

- structure: To train our method, we adopt a two-step training scheme. During the first step, we train the 3D CNN on the first dataset to output a per-view MPI volume. The first step is performed by selecting 6 neighboring views, using a random set of 5 as inputs and using the last image as a target view for supervision. During the second step, the 3D CNN is fine-tuned end-to-end with our second dataset by synthesizing a target view from its closest 5 cameras. 

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/MDPstructure.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/MDPstructure1.png)
- results：

metrics: **( PSNR, SSIM, L1)**

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/MDPresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/MDPresult1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/MDPresult2.png)

- analysis:  We presented a novel 3D scene representation—Multi Depth Panoramas, or MDP—that represents complex scenes using multiple layers of concentric RGBDα panoramas. MDPs are more compact than prior scene representations such as **multiple plane images** （MPIs）. As such, they can be used to generate high-quality novel view synthesis results with translational motion parallax, using our proposed forward-splatting rendering method. Furthermore, we presented a learning-based method to accurately reconstruct MDPs from commercial 360◦ camera rigs.

