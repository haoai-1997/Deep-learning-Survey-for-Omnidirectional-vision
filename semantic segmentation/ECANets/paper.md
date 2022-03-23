## Capturing Omni-Range Context for Omnidirectional Segmentation

- year: 2022

- dataset：**( PASS ; Wild Panoramic Semantic Segmentation (WildPASS), a dataset designed to capture diverse scenes from all around the globe)**  

- abstract: To bridge the gap in terms of FoV and structural distribution between the imaging domains, we introduce Efficient Concurrent Attention Networks (ECANets), directly capturing the inherent long-range dependencies in omnidirectional imagery.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ECANEtsabstract.png)

- Contributions:

1) Rethink omnidirectional semantic segmentation from the context-aware perspective and propose Efficient Concurrent Attention Networks, capturing inherent long-range dependencies across the 360◦
2) Introduce multi-source omni-supervised learning, integrating unlabeled panoramic images into training, empowering models to learn rich contextual priors.
3) Present the diverse WildPASS dataset: Collected from 6 continents and 65 cities, enabling evaluation of panoramic semantic segmentation in the wild.

- structure:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ECANEtsstructure1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ECANEtsstructure2.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ECANEtsstructure3.png)

- dataset：Wild PAnoramic Semantic Segmentation dataset: Overall, we gather 2500 panoramas in 65 cities from all continents Asia, Europe, Africa, Oceania, North and South America (excluding only Antarctica). Following PASS and RainyNight, 500 panoramas from 25 cities are precisely annotated for the most critical navigation-related classes. We extend the semantics defined for panoramic segmentation to 8 classes: Car, Road, Sidewalk, Crosswalk, Curb, Person, Truck and Bus. The remaining 2000 panoramas from 40 different cities are collected for omni-supervised learning. All images have a 360◦×70◦ FoV at 2048×400.



- results：
metrics: **(mIoU)**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ECANEtsresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ECANEtsresult1.png)

- analysis: We look into omnidirectional image segmentation from the context-aware perspective. To bridge the gap in terms of FoV and structural distribution, our proposed ECANet captures inherent omni-range dependencies that stretch across 360◦ , whose generalization is optimized via multisource omni-supervision and multi-space fusion.
