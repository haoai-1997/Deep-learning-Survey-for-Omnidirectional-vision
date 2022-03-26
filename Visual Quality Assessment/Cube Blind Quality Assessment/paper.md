## Cubemap-Based Perception-Driven Blind Quality Assessment for 360-degree Images

- year: 2021

- dataset: MVAQD dataset (self-collected)

- Abstract: In this paper, we propose a new blind 360-IQA framework to handle this imbalance problem. In the proposed framework, cubemap projection (CMP) with six inter-related faces is used to realize the omnidirectional viewing of 360-degree image. A multi-distortions visual attention quality dataset for 360-degree images is firstly established as the benchmark to analyze the performance of objective 360-IQA methods. Then, the perception-driven blind 360-IQA framework is proposed based on six cubemap faces of CMP for 360-degree image, in which human attention behavior is taken into account to improve the effectiveness of the proposed framework. 
- Contributions:
(1) The re-projected distortion changes between ERP image and SP image are analyzed for subjective and objective quality assessment. It is found that the re-projected distortion of CMP image is more consistent with that of SP image, rather than ERP image. To study how CMP images can be better applied to 360-IQA, a more comprehensive multi-distortions visual attention quality dataset (MVAQD) for 360-degree images is established, and a new way for designing 360-IQA metrics is provided.
2) Based on six cubemap faces of CMP image and their corresponding HM and EM hotspot maps, a cubemap quality feature subset and two different attention fea- ture subsets with corresponding attention feature matri- ces are designed. On this basis, a CPBQA framework with three schemes is proposed. The proposed framework is also applicable to be combined with the exist- ing BIQA methods designed for 2D plane image and machine learning based pooling schemes to achieve better performance.
- Structure: BiFuse

<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/cube bqa.png" width="70%" height="70%">

-Analysis: It is found that the re-projected distortion of CMP image is more consistent with that of SP image, rather than ERP image. In addition, perceptual quality of 360-degree image is correlated with user’s HM and EM, which are usually related to image saliency.Thus, a cubemap quality feature subset and two different attention feature subsets with corresponding attention feature matrices are designed.
