## DensePASS: Dense Panoramic Semantic Segmentation via Unsupervised Domain Adaptation with Attention-Augmented Context Exchange

- year: 2021

- dataset：  **( DENSEPASS - a novel densely annotated dataset for panoramic segmentation under cross-domain conditions, specifically built to study the PINHOLE→PANORAMIC transfer and accompanied with pinhole camera training examples obtained from Cityscapes.)**  

- abstract:In this work, we look at this problem through the lens of domain adaptation and bring panoramic semantic segmentation to a setting, where labelled training data originates from a different distribution of conventional pinhole camera images
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DensePASSabstract.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DensePASSstructure.png)
- Contributions:

1) We create and publicly release DensePASS – a new benchmark for panoramic semantic segmentation collected from locations all around the world and densely annotated with 19 classes in accordance to the pinhole camera dataset Cityscapes to enable proper PINHOLE→PANORAMIC evaluation. 
2) We formalize the problem of unsupervised domain adaptation for panoramic segmentation focused on transfer from label-rich pinhole datasets to DensePASS and propose a generic P2PDA framework and investigate different DA modules both in a separate and joint manner, validating their effectiveness with various networks designed for self-driving scene segmentation.



- structure:
First, we formalize the task of unsupervised domain adaptation for panoramic semantic segmentation, where a network trained on labelled examples from the source domain of pinhole camera data is deployed in a different target domain of panoramic images, for which no labels are available.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DensePASSstructure1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DensePASSstructure2.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DensePASSstructure3.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DensePASSstructure4.png)
- dataset：DENSEPASS covers both, labelled- and unlabelled 360◦ images, with the labelled data comprising 19 classes which explicitly fit the categories available  in the source domain (i.e. pinhole) data



- results：
metrics: **(mIoU)**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/DensePASSresult.png)

- analysis: In this work, we introduced the new task of cross-domain semantic segmentation for panoramic driving scenes, which extends the standard panoramic segmentation with the premise of the training data originating from a different domain (e.g. pinhole camera images).
