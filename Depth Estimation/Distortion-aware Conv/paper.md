## Distortion-Aware Convolutional Filters for Dense Prediction in Panoramic Images

- year: 2018

- dataset: Stanford2D3D dataset (for testing) and NYU Depth v2 dataset (for training)

- Abstract: 3D sensors able to capture 3D panoramic data are expensive and/or hardly available. To fill this gap, we propose a learning approach for panoramic depth map estimation from a single image. Thanks to a specifically developed distortion-aware deformable convolution filter, our method can be trained by means of conventional perspective images, then used to regress depth for panoramic images, thus bypassing the effort needed to create annotated panoramic training dataset.
- Contributions:
We propose to modify the network’s convolutions by leveraging geometrical priors for the image distortion, by means of a novel distortion-aware convolution that adapts its receptive field by deforming the shape of the convolutional filter according to the distortion and projection model. Thus, these modified filters can compensate for the image distortions directly during the convolutional operation, so to rectify the receptive field. In particular, the advantage is that panoramic depth prediction can be trained by means of standard perspective images. 

- Structure: Distortion-aware convolution

<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Distortion.png" width="70%" height="70%">

- Results：
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Distortion_exp1.png" width="50%" height="50%">
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Distortion_exp2.png" width="50%" height="50%">

-Analysis: 


