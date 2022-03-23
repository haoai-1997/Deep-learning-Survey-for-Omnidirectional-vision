## OmniMVS: End-to-End Learning for Omnidirectional Stereo Matching

- year: 2021

- dataset：  **(synthetic datasets (OmniThings and OmniHouse) for training and testing omnidirectional multi-view stereo algorithms.)**  
11K ground-truth depth maps and 45K fisheye images in four orthogonal directions with various objects and environments. 

- abstract: we propose a novel end-to-end deep neural network model for omnidirectional depth estimation from a wide-baseline multi-view stereo setup. 
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/OmniMVSdataset.png)

- Contributions:
1) We propose a novel end-to-end deep learning model to estimate an omnidirectional depth from multiple fisheye cameras. The proposed model directly projects feature maps to the predefined global spheres, combined with the 3D encoder-decoder block enabling to utilize global contexts for computing and regularizing the matching cost.
2) We offer large-scale synthetic datasets for the omnidirectional depth estimation. The datasets consist of multiple input fisheye images with corresponding omnidirectional depth maps. The experiments on the realworld environments show that our datasets successfully train our network

- structure:

The images captured with ultra wide field-of-view (FOV) cameras on an omnidirectional rig are processed by the feature extraction module, and then the deep feature maps are warped onto the concentric spheres swept through all candidate depths using the calibrated camera parameters. The 3D encoderdecoder block takes the aligned feature volume to produce the omnidirectional depth estimate with regularization on uncertain regions utilizing the global context information.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/OmniMVSstructure.png)

- results：

metrics: **(MAE and RMSE)**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/OmniMVSresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/OmniMVSresult1.png)

- analysis: OmniMVS, as the first work, converts the input fisheye images into the unary feature maps, and builds the 4D feature volume using the calibration and spherical sweeping.
