## Bending Reality: Distortion-aware Transformers for Adapting to Panoramic Semantic Segmentation

- year: 2022

- dataset: indoor Stan-ford2D3D, outdoor DensePASS, Cityscapes

- abstract: Distortions and the distinct image-feature distribution in360◦ panoramas impede the transfer from the annotation-rich pinhole domainand therefore come with a big dent in performance. 
To get around this domain difference and bring together semantic annotations from pinhole and360◦ surround visuals, we propose to learn object deformations and panoramic image distortions in the Deformable Patch Embedding(DPE) and Deformable MLP (DMLP) components which blend into our Transformer for PAnoramic Semantic Segmenta-tion (Trans4PASS)model.

- contributions:
(1) We consider panoramic deformations in our distortion-aware Transformer for Panoramic Semantic Segmenta-tion (Trans4PASS) with deformable patch embedding and deformable MLP modules.
(2) We present Mutual Prototypical Adaptation to transfer models via distilling dual-domain prototypical knowledge, boosting performance by coupling it with pseudo-labels in feature and output space.
(3) Our framework for transferring models from PIN2PAN yields excellent results on two competitive bench-marks.

- structure:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Bending_Reality_framework.png)

- loss function

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SEG_loss.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SSL_loss.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/MPA_loss.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/final_loss.png)

- result:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Bending_Reality_result.png)




