## VRSA Net: VR Sickness Assessment Considering Exceptional Motion for 360° VR Video

- year: 2019

- dataset：  **(a new dataset which consists of 360° videos (stimuli), corresponding physiological signals, and subjective questionnaires from subjective assessment experiments)**  

- abstract: In this paper, we propose a novel objective VR sickness assessment (VRSA) network based on deep generative model for automatically predicting the VR sickness score.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VRSANetabstract.png)

- Contributions:
1) We present a novel deep generative model-based objective VR sickness assessment network (VRSA Net)
considering exceptional motion pattern in VR content.
2) For the evaluation of the proposed objective VRSA, we built a newly collected 360-degree video dataset with the corresponding subjective scores and physiological signal data, as a benchmark for VRSA.

-structure: The proposed VRSA network consists of two parts, which are VR video generator and VR sickness score predictor. 
1) By training the VR video generator with common videos with non-exceptional motion, the generator learns the tolerance of VR sickness in human motion perception. As a result, the difference between the original and the generated videos by the VR video generator could represent exceptional motion of VR video causing VR sickness. 
2) In the VR sickness score predictor, the VR sickness score is predicted by projecting the difference between the original and the generated videos onto the subjective score space.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VRSANetstructure.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VRSANetstructure1.png)
- results：

metrics: **(Pearson linear correlation coefficient (PLCC), Spearman rank order correlation coefficient (SROCC), and root mean square error (RMSE).)**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VRSANetdataset.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VRSANetresult.png)

- analysis:  In this paper, we proposed a novel objective deep generative model-based VRSA Net for 360-degree videos. In the proposed method, instead of end-to-end training the regression model with a large number of VR datasets and corresponding subjective scores (i.e., ground truth), the VR video generator based on GAN was devised to learn the tolerance of VR sickness in human motion perception.
