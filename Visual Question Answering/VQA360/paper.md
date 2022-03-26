## Visual Question Answering on 360{\deg} Images
- year: 2020

- dataset：  **(the first VQA 360◦ dataset, containing around 17,000 realworld image-question-answer triplets for a variety of question types)**  

- abstract: We introduce VQA 360◦ , a novel task of visual question answering on 360◦ image. We collect the first VQA 360◦ dataset. And then we study two different VQA models on VQA 360◦, including one conventional model that takes an equirectangular image (with intrinsic distortion) as input and one dedicated model that first projects a 360◦ image onto cubemaps and subsequently aggregates the information from multiple spatial resolutions.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VQA360abstract.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VQA360dataset.png)
- Contributions:

1) We define a novel task named VQA 360◦ . We point out the intrinsic difficulties compared to VQA on NFOV images. We further collect the first real VQA 360◦ dataset, which is designed to include complicated questions specifically for 360◦ images.
2)We comprehensively evaluate two kinds of VQA models for VQA 360◦ , including one that can effectively handle spatial distortion while performing multi-level spatial reasoning. We then point out future directions for algorithm design for VQA 360◦.

- structure:
Equirectangular-based Models and Cubemap-based Models
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VQA360structure.png)

- results：

We demonstrate that the cubemap-based model with multi-level fusion and attention diffusion performs favorably against other variants and the equirectangular-based models.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VQA360result.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VQA360result1.png)


- analysis: We introduce VQA 360◦ , a novel VQA task on a challenging visual domain, 360◦ images. We collect the first VQA 360◦ dataset and experiment with multiple VQA models. We then present a multi-level attention model to effectively handle spatial distortion (via cubemaps) and perform sophisticated reasoning. Experimental results demonstrate the need to explicitly model intrinsic properties of 360◦ images, while the noticeable gap between humans’ and machines’ performance reveals the difficulty of reasoning on 360◦ images compared to NFOV images.

