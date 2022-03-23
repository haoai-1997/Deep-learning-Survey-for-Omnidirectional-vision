## Privacy Protection in Street-View Panoramas using Depth and Multi-View Imagery

- year: 2019

- dataset：  **(a dataset of 1000 images)**  

- abstract: In this paper, we propose a framework that is an alternative to blurring, which automatically removes and inpaints moving objects (e.g. pedestrians, vehicles) in street-view imagery.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PPSVabstract.png)

- Contributions:
1) We propose a new multi-view framework for detecting and inpainting moving objects, as an alternative to
blurring in street-view imagery
2) We introduce a new moving object detection algorithm based on convolutional features that exploits depth consistencies from a set of consecutive images.
3) We train an inpainting GAN that utilizes multi-view information to obtain authentic and plausible results.
-structure: The proposed moving object detection algorithm, combines with results from a standard segmentation algorithm to obtain segmentation masks for moving objects.  Finally, to achieve an authentic completion of the removed moving objects, we use inpainting Generative Adversarial Network (GAN) that utilizes multi-view information

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PPSVstructure.png)

- results：

metrics: 
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PPSVresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PPSVresult1.png)

- analysis:  The proposed framework comprises of novel convolutional feature based moving object detection algorithm that is coupled with a multi-view inpainting GAN to detect, remove and inpaint moving objects.
