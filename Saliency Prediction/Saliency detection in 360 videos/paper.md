## Saliency Detection in 360◦Videos

- year: 2018

- dataset: 360◦videos from Sports-360 dataset, and remove the video clips whose length is less than 20 seconds, and use the remaining 104 video clips as the data used for saliency detection in360◦videos.

- abstract
This paper presents a novel spherical convolutional neural networkbased scheme for saliency detection for360◦videos.
Considering that the360◦ videos are usually stored with equirectangular panorama, we propose to implement the spherical convolution on panorama by stretching androtating the kernel based on the location of patch to be convolved.
We further takethe temporal coherence of the viewing process into consideration, and proposea sequential saliency detection by leveraging a spherical U-Net. 

- structure：

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Saliency_detection-algorithm.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Saliency_detection_parameter_sharing.png)

- loss

Spherical Mean Squared Error (MSE) Loss
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SMSE.png)

-result

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/U-Net-performance.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Saliency_detection_result.png)
