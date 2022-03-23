## BIPS: Bi-modal Indoor Panorama Synthesis via Residual Depth-aided Adversarial Learning

- year: 2021

- dataset：  **(synthetic dataset : Structured3D and real datasets: Matterport3D and 2D-3D-S dataset)**  

- abstract: In this paper, we study a new problem: RGB-D panorama synthesis under the arbitrary configurations of cameras and depth sensors. Accordingly, we propose a novel bi-modal (RGB-D) panorama synthesis (BIPS)framework. 
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/BIPSabstract.png)

- Contributions:
1) We introduce a new problem of generating RGB-D panoramas from partial and arbitrary RGB-D inputs.
2) We propose a BIPS framework that allows to synthesize RGBD panoramas via residual depth-aided adversarial learning.
3) We introduce a novel evaluation metric, FAED, for RGB-D panorama synthesis and demonstrate its validity.
- structure:

 We design a generator that fuses the bi-modal information and train it with residualaided adversarial learning (RDAL). RDAL allows to synthesize realistic indoor layout structures and interiors by jointly inferring RGB panorama, layout depth, and residual depth.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/BIPSstructure.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/BIPSstructure1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/BIPSstructure2.png)

- results：

metrics: **(RGB metric: PSNR, SSIM, LPIPS; Layout metric: 2D Corner error; Proposed metric: FAED)**, **(Depth metric: AbsREL, RMSE; Layout metric: 2D IoU; Proposed metric: FAED)**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/BIPSresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/BIPSresult1.png)


- analysis: we tackled a novel problem of synthesizing RGB-D indoor panoramas from arbitrary configurations of RGB and depth inputs. Our method can synthesize highquality RGB-D panoramas with the proposed BIPS framework by utilizing the bi-modal information and jointly training the layout and residual depth of indoor scenes.
