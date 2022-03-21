## ACDNet: Adaptively Combined Dilated Convolution for Monocular Panorama Depth Estimation

- year: 2021

- dataset: Stanford2D3D(real-world), Matterport3D(real-world), Structured3D(Synthetic)

- abstract: In this paper, we propose an ACDNet based on the adaptively combined dilated convolution to predict the dense depth map for a monocularpanoramic image.
Meanwhile, we introduce an adaptive channel-wise fusion module to summarize the feature maps and get diverse attention areas in the receptive field along the channels.

- contributions:
(1) We propose the adaptively combined dilated convolution to process the panorama images for monocular depth estimation, and it can be easily embedded into convolution networks by replacing the regular convolution.
(2) The interest areas can be obtained by learning different attention scores in different channels, which is more suitable for panoramic images than explicitly deforming convolution kernels in different latitudes.
(3) We perform the monocular panorama depth estimation experiments on both virtual and real-world RGB-Dpanorama datasets, which outperforms the SOTA methods in both quantitative metrics and visual effects.

- strutcure:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ACDNet.png)

- loss function

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ACDNet_loss.png)

- result:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ACDNet_result.png)

- Analysis:

That is worth further researching for panorama images in the future.
In addition, we will studyour ACDConv in other existing depth prediction models and its effects on other various panoramic image tasks such as image classification and semantic segmentation.
