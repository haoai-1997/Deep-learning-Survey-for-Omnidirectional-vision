## DS-PASS: Detail-Sensitive Panoramic Annular Semantic Segmentation
through SwaftNet for Surrounding Sensing

- year: 2019

- dataset：**( extended PASS dataset)**  

- abstract: In this paper, we propose a network adaptation framework to achieve Panoramic Annular Semantic Segmentation (PASS), which allows to re-use conventional pinhole-view image datasets, enabling modern segmentation networks to comfortably adapt to panoramic images.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DS-PASSabstract.png)

- Contributions:

1) we adapt our proposed SwaftNet to enhance the sensitivity to details by implementing attention-based lateral connections between the detail-critical encoder layers and the context-critical decoder layers. 

- structure: We adapt our proposed SwaftNet to enhance the sensitivity to details by implementing attention-based lateral connections between the detail-critical encoder layers and the context-critical decoder layers.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DS-PASSstructure1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DS-PASSstructure2.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DS-PASSstructure3.png)

- results：
metrics: **(mIoU)**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DS-PASSresult1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DS-PASSresult2.png)

- analysis: DS-PASS is presented with a general network adaptation method that enables state-of-theart semantic segmentation network trained on perspective imaging datasets to work comfortably in panoramic imagery domain. Specifically, we put forward a real-time semantic segmentation network named SwaftNet, by blending semantically-meaningful deep layers with spatially-detailed shallow layers using lateral attentional skip-connections, to perform segmentation both swiftly and accurately.
