## LED2-Net: Monocular 360◦Layout Estimation via Differentiable DepthRendering

- year: 2021

- dataset: Realtor360, Matterport3D, PanoContext, Stanford2D3D

- abstract:
Exsiting room layout methods aim to reduce the loss inthe 2D pixel coordinate rather than exploiting the roomstructure in the 3D space.
we formulate the task of 360◦layout estimation as a problem of predicting depth on the horizon line of a panorama.
Specifically, we propose the Differentiable Depth Rendering procedure to make the conversion from layout to depth prediction differentiable,
thus making our proposed model end-to-end trainable while leveraging the 3D geometric information, without the need of providing the ground truth depth.

- contributions:
(1) We reformulate the task of 360◦layout estimation to a unique 360◦depth estimation problem that optimizes a loss in 3D while maintaining the simplicity of layout estimation.
(2) We propose a differentiable layout-to-depth procedure to convert the layout into horizon-depth through ray-casting of a few points, which enables the end-to-end training on layout estimation datasets.
(3) We show that our framework can be seamlessly pre-trained by 360◦depth datasets, which further improves the generalizability on cross-dataset evaluations.

- structure:
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LED2-Net-framework.png)

- loss function

L1 loss to measure the errors between depth maps

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LED2-Net-loss.png)

- result:
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LED2-Net-result_1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/LED2-Net-result_2.png)





