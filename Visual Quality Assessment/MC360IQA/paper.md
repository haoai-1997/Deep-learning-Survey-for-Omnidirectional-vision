## MC360IQA: A Multi-channel CNN for Blind360-Degree Image Quality Assessment

- year: 2019

- dataset: CVIQ and OIQA databases(synthetic)

- abstract:
In this paper,we present a study on both subjective and objective quality as-sessment of compressed virtual reality (VR) images.
We first build a compressed VR image quality (CVIQ) database including 16 reference images and 528 compressed ones with three prevailing coding technologies. 
Then, we propose a multi-channel convolution neural network (CNN) for blind 360-degree image quality assessment (MC360IQA). 

- contributions
(1) We establish a large compressed VR image quality database.
(2) We propose a multi-channel CNN model for NR 360-degree image quality assessment. 
(3) We propose to use the hyper-CNN architecture as the baseCNN channel for the MC360IQA, which can incorporate the features from the intermediate layers.

- structure:
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/MC360IQA-network.png)

- loss function

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/loss_function_MC360IQA.png)

- result:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/result_on_CVIQ.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/result_on_QIQA.png)
