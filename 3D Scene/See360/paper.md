## See360: Novel Panoramic View Interpolation

- year: 2022

- dataset: introduce four training dataset, namely UrbanCity360(synthetic), Archinterior360(synthetic), HungHom360(real) and Lab360(real) 

- abstract: the See360 model learns to rendernovel views by a proposed novel Multi-Scale Affine Transformer(MSAT), enabling the coarse-to-fine feature  rendering. We also propose a Conditional Latent space AutoEncoder(C-LAE) to achieve view interpolation at any arbitrary angle. The paper also introduce four datasets to show the versatility of the model.

- contributions:
(1)we propose a Multi-Scale Affine Transformer (MSAT) to render reference views in the feature domain using 2D affine transformation.
(2)we introduce the Conditional Latentspace AutoEncoder (C-LAE) to allow users to interactively manipulate views at any angle.
(3)In addition, we provide two different types of datasets totrain and test our model. 

- structure:
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/see360.png)

- results:
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/see360_exp_1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/see360_exp_2.png)



