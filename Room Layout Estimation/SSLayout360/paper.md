## SSLayout360: Semi-Supervised Indoor Layout Estimation from 360◦ Panorama

- year: 2021

- dataset：  **( PanoContext dataset and Stanford-2D3D dataset, MatterportLayout test dataset)**  

- abstract: We explore the intersection of these two fields, semisupervised learning and 3D room layout reconstruction.  We propose the first approach to learn representations of room corners and boundaries by using a combination of labeled and unlabeled data for improved layout estimation in a 360◦ panoramic scene
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SSLayout360abstract.png)

- Contributions:

1) We present SSLayout360, a neural architecture capable of learning representations of floor-wall, ceiling-wall, and wall-wall boundaries from a combination of labeled and unlabeled data for improved room layout estimation in a 360◦ panoramic scene. Our work is the first substantive attempt at semi-supervised 3D layout reconstruction of complex indoor scenes using as few as 20 labeled examples.
2) We establish the first comprehensive set of semisupervised benchmarks to measure the contribution of unlabeled data for indoor layout estimation. As part of this contribution, we propose a rigorous evaluation protocol to encourage the use of error bounds as standard practice and demonstrate the utility of unlabeled data across many experimental settings. We hope that our results serve as a strong baseline to inspire future research towards even more robust semi-supervised 3D layout reconstruction


- structure:
We train a neural network fθ(x), a stochastic prediction function parametrized by θ, to learn room layout boundaries by using a combination of DL and DU.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SSLayout360structure.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SSLayout360structure1.png)


- results：
metrics: **(3D IoU, Corner Error, Pixel Error, 2D IoU, δ1, RMSE)**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SSLayout360result.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SSLayout360result1.png)

- analysis: We presented SSLayout360, an approach that combines the strengths of HorizonNet and Mean Teacher, and extends them both to enable semi-supervised layout estimation from complex 360◦ panoramic indoor scenes. A distinct modification that allows our algorithm to work well is the loss formulation to regress real-valued prediction vectors to ground truth via L1 and L2 distances.
