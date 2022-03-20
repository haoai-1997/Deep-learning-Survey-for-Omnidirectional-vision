## A Deep Ranking Model for Spatio-Temporal Highlight Detection from a 360-degree Video

- year: 2018

- dataset: Pano2Vid dataset and 360-degree video highlight dataset

- abstract: We address the problem of highlight detection from a 360-degree video by summarizing it both spatially and temporally. Given a long 360-degree video, we spatially select pleasantly-looking normal field-of-view (NFOV) segments from unlim- ited field of views (FOV) of the 360◦ video, and temporally summarize it into a concise and informative highlight as a selected subset of subshots.
- Contributions:
(1) We follow a Manhattan World assumption,reconstructing the complete shape of the room. 
(2) Objectlocation and pose is estimated using top-down object detec-tion and 3D pose estimation using a public library of 3Dmodels
(3) We introduce a context prior for object and wallrelationships in order to sample plausible room hypotheses.

- structure: Generative model

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Pano2CAD.png)

- results：
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Pano2CAD_result.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images /Pano2CAD_sundataset.png)

-analysis: 将room layout工作进行拆分成，surface normal estimation, 2D object detection and 3D object pose estimation,利用生成模型和概率论进行参数推理。

