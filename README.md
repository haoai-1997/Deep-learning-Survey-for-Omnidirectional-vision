# (We are updating the information and adjusting the pages on this code! If you want to provide some good papers, please send us on the issues! Hope that we can provide some intreseting works for the omnidirectional vision!)

# &diams; Deep Learning for Omnidirectional Vision: A Survey and New Perspectives

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/main_page/survey.png" width="1000" height="410">
</div>

**Referenced paper** : [Deep Learning for Omnidirectional Vision: A Survey and New Perspectives](https://arxiv.org/abs/2205.10468)

## Table of Content
### &hearts; [Introduction](Introduction)

&nbsp; &nbsp; &nbsp; &nbsp; Omnidirectional image (ODI) data is captured with a  360°×180°  field-of-view and omnidirectional vision has attracted booming attention due to its more advantageous performance in numerous applications. Our survey presents a systematic and comprehensive review and analysis of the recent progress in Deep Learning methods for omnidirectional vision. 
 
&nbsp; &nbsp; &nbsp; &nbsp; **Especially, we create this open-source repository to provide a taxonomy of all the mentioned works and code links in the survey. We will keep updating our open-source repository with new works in this area and hope it can shed light on future research and build a community for researchers on omnidirectional vision.**
### &hearts; [Background](Background)
#### **Acquisition**
An ideal 360&deg; camera can capture lights falling on the focal point from all directions, making the projection plane a whole spherical surface. In practice, most 360&deg; cameras can not achieve it, which excludes top and bottom regions due to dead angles

### &hearts; [Convolution/Transformer Methods on ODIs](Backbone)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **Learning SO(3) Equivariant Representations with Spherical CNNs**  [Paper](Backbone/SO(3)%20Equivariant%20Representations) [**Code**](https://github.com/daniilidis-group/spherical-cnn)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **Spherical CNNs**  [Paper](Backbone/Spherical%20CNNs) [**Code**](https://github.com/jonkhler/s2cnn)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **Learning Spherical Convolution for Fast Features from 360&deg; Imagery**  [Paper](Backbone/SPHCONV) [**Code**](https://github.com/rbgirshick/py-faster-rcnn)

### &hearts; [Omnidirectional Vision Tasks](Tasks)

&nbsp; &nbsp; &nbsp; &nbsp; :smiley: [***Image&Video Manipulation***](Tasks/Image%26Video%20Manipulation)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Omnidirectional Image Generation (Completion)](Tasks/Image%26Video%20Manipulation/Omnidirectional%20Image%20Generation%20(Completion))

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **360 Panorama Synthesis from a Sparse Set of Images with Unknown Field of View**  [Paper](Tasks/Image%26Video%20Manipulation/Omnidirectional%20Image%20Generation%20(Completion)/360%20Panorama%20Synthesis%20from%20a%20Sparse%20Set%20of%20Images%20with%20Unknown%20Field%20of%20View) [**Code**](https://github.com/kimsoojie/lab_vcl_360panorama)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **360-Degree Image Completion by Two-Stage Conditional Gans** [Paper](Tasks/Image%26Video%20Manipulation/Omnidirectional%20Image%20Generation%20(Completion)/360-Degree%20Image%20Completion%20by%20Two-Stage%20Conditional%20Gans) [Code](Tasks/Image%26Video%20Manipulation/Omnidirectional%20Image%20Generation%20(Completion)/360-Degree%20Image%20Completion%20by%20Two-Stage%20Conditional%20Gan/Code.md)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **BIPS: Bi-modal Indoor Panorama Synthesis via Residual Depth-aided Adversarial Learning (RGB and Depth)**[Paper](Tasks/Image%26Video%20Manipulation/Omnidirectional%20Image%20Generation%20(Completion)/BIPS:%20Bi-modal%20Indoor%20Panorama%20Synthesis%20via%20Residual%20Depth-aided%20Adversarial%20Learning) [Code](Tasks/Image%26Video%20Manipulation/Omnidirectional%20Image%20Generation%20(Completion)/BIPS:%20Bi-modal%20Indoor%20Panorama%20Synthesis%20via%20Residual%20Depth-aided%20Adversarial%20Learning/Code.md)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **Diverse Plausible 360-Degree Image Outpainting for Efficient 3DCG Background Creation** [Paper](Tasks/Image%26Video%20Manipulation/Omnidirectional%20Image%20Generation%20(Completion)/Diverse%20Plausible%20360-Degree%20Image%20Outpainting%20for%20Efficient%203DCG%20Background%20Creation) [**Code**](https://github.com/akmtn/OmniDreamer) 

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **Spherical Image Generation from a Single Normal Field of View Image by Considering Scene Symmetry** [Paper](Tasks/Image%26Video%20Manipulation/Omnidirectional%20Image%20Generation%20(Completion)/Spherical%20Image%20Generation%20from%20a%20Single%20Normal%20Field%20of%20View%20Image%20by%20Considering%20Scene%20Symmetry) [Code](Tasks/Image%26Video%20Manipulation/Omnidirectional%20Image%20Generation%20(Completion)/Spherical%20Image%20Generation%20from%20a%20Single%20Normal%20Field%20of%20View%20Image%20by%20Considering%20Scene%20Symmetry/Code.md)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **Text2Light: Zero-Shot Text-Driven HDR Panorama GenerationText2Light: Zero-Shot Text-Driven HDR Panorama Generation** [Paper](Tasks/Image%26Video%20Manipulation/Omnidirectional%20Image%20Generation%20(Completion)/Text2Light:%20Zero-Shot%20Text-Driven%20HDR%20Panorama%20Generation/Paper.md) [**Code**](https://github.com/FrozenBurning/Text2Light)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Omnidirectional Image&Video Compression](Tasks/Image&Video%20Manipulation/Omnidirectional%20Image&Video%20Compression)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Omnidirectional Image&Video Cross-View Synthesis](Tasks/Image&Video%20Manipulation/Omnidirectional%20Image&Video%20Cross-View%20Synthesis)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Omnidirectional Image&Video Lighting Estimation](Tasks/Image%26Video%20Manipulation/Omnidirectional%20Image%20Generation%20(Completion))

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Omnidirectional Image&Video Super-Resolution](Tasks/Image%26Video%20Manipulation/Omnidirectional%20Image%26Video%20Super-Resolution)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Omnidirectional Image&Video Upright Adjustment](Tasks/Image&Video%20Manipulation/Omnidirectional%20Image&Video%20Upright%20Adjustment)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Omnidirectional Image&Video Visual Quality Assessment](Tasks/Image%26Video%20Manipulation/Omnidirectional%20Image%26Video%20Visual%20Quality%20Assessment)

&nbsp; &nbsp; &nbsp; &nbsp; :smiley: [***Scene Understanding***](Tasks/Scene%20Understanding)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Object Detection](Tasks/Scene%20Understanding/Object%20Detection)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Semantic Segmentation](Tasks/Scene%20Understanding/Semantic%20Segmentation)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Optical Flow Estimation](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Video Summraization](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Monocular Depth Estimation](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **Distortion-Aware Convolutional Filters for Dense Prediction in Panoramic Images
(2018)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/DAC) [**Code**](https://github.com/tdsuper/Distortion-aware-CNNs)

 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **OmniDepth: Dense Depth Estimation for Indoors Spherical Panoramas (2018)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/OmniDepth) [**Code**](https://github.com/meder411/OmniDepth-PyTorch)
 
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **Spherical View Synthesis for Self-Supervised 360-degree Depth Estimation (2019)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/SphericalVS) [**Code**](https://github.com/VCL3D/SphericalViewSynthesis)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **Pano Popups: Indoor 3D Reconstruction with a Plane-Aware Network. (2019)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/PanoPopups) [Code](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/PanoPopups/Code.md)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **BiFuse: Monocular 360-degree Depth Estimation via Bi-Projection Fusion (2020)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/BiFuse) [**Code**](https://github.com/Yeh-yu-hsuan/BiFuse)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **Geometric Structure Based and Regularized Depth Estimation From 360-degree Indoor Imagery
 (2020)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/GSOMDE) [Code](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/GSOMDE/Code.md)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **PADENet: An Efficient and Robust Panoramic Monocular Depth Estimation Network for Outdoor Scenes (2020)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/PADENet) [Code](https://github.com/zzzkkkyyy/PADENet))

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **UniFuse: Unidirectional Fusion for 360° Panorama Depth Estimation
 (2021)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/UniFuse) [**Code**](https://github.com/alibaba/UniFuse-Unidirectional-Fusion)
 
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **Improving 360 Monocular Depth Estimation via Non-local Dense Prediction Transformer and Joint Supervised and Self-supervised Learning (2021)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/IMDE) [**Code**](https://github.com/yuniw18/Joint_360depth)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **SliceNet: deep dense depth estimation from a single indoor panorama using a slice-based representation (2021)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/SliceNet) [**Code**](https://github.com/crs4/SliceNet)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **PanoDepth: A Two-Stage Approach for Monocular Omnidirectional Depth Estimation
(2021)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/PanoDepth) [**Code**](https://github.com/yuyanli0831/PanoDepth)

 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **Depth360: Self-supervised Learning for Monocular Depth Estimation
using Learnable Camera Distortion Model (2021)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/Depth360) [Code](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/Depth360/Code.md)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **OmniFusion : 360 Monocular Depth Estimation via Geometry-Aware Fusion (2022)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/OmniFusion) [**Code**](https://github.com/yuyanli0831/OmniFusion)
  
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **360MonoDepth: High-Resolution 360° Monocular Depth Estimation (2022)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/360MonoDepth) [**Code**](https://github.com/manurare/360monodepth)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **ACDNet: Adaptively Combined Dilated Convolution for Monocular Panorama Depth Estimation (2022)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/ACDNet) [**Code**](https://github.com/zcq15/ACDNet)
 
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **GLPanoDepth: Global-to-Local Panoramic Depth Estimation (2022)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/GLPanoDepth) [Code](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/GLPanoDepth/Code.md)
 
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **360 Depth Estimation in the Wild: The Depth360 Dataset and the SegFuse Network (2022)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/SegFuse) [**Code**](https://github.com/HAL-lucination/segfuse)
 
&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **Deep Depth Estimation on 360° Images with a Double Quaternion Loss (2022)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/DQL) [Code](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/DQL/Code.md)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **PanoFormer: Panorama Transformer for Indoor 360 Depth Estimation (2022)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/PanoPopups) [**Code**](https://github.com/zhijieshen-bjtu/PanoFormer)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **Multi-Modal Masked Pre-Training for Monocular Panoramic Depth Completion (2022)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/M3PT) [Code](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/M3PT/Code.md)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **Self-supervised indoor 360- degree depth estimation via structural regularization (2022)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/SSIDE) [Code](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/SSIDE/Code.md)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **Variational Depth Estimation on Hypersphere for Panorama (2022)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/OmniVAE) [Code](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/OmniVAE/Code.md)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; - **SphereDepth: Panorama Depth Estimation from Spherical Domain (2022)**  [Paper](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/SphereDepth) [Code](Tasks/Scene%20Understanding/Monocular%20Depth%20Estimation/SphereDepth/Code.md)

&nbsp; &nbsp; &nbsp; &nbsp; :smiley: [***3D Vision***](Tasks/3D%20Vision)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [SLAM](Tasks/3D%20Vision/SLAM)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Stereo Matching](Tasks/3D%20Vision/Stereo%20Matching)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Room Layout estimation and Reconstruction](Tasks/3D%20Vision/Room%20Layout%20estimation%20and%20Reconstruction)

&nbsp; &nbsp; &nbsp; &nbsp; :smiley: [***Human-Machine Interaction***](Tasks/Human-Machine%20Interaction)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Saliency Prediction](Tasks/Human-Machine%20Interaction/Saliency%20Prediction)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Visual Question Answering](Tasks/Human-Machine%20Interaction/Visual%20Question%20Answering)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Gaze Behavior](Tasks/Human-Machine%20Interaction/Gaze%20Behavior)

&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; :wink: [Audio-Visual Scene Understanding](Tasks/Human-Machine%20Interaction/Audio-Visual%20Scene%20Understanding)

### &hearts; [Novel Learning Strategies](Novel%Learning%20Strategies)
### &hearts; [Applications](Applications)
### &hearts; [Disscussion and New Perspectives](New%20Perspectives)

## [3D reconstruction](3D%20reconstruction)

- Efficient 3D Room Shape Recovery **(traditional)**
- MVLayoutNet: 3D layout reconstruction with multi-view panoramas
- HeadFusion: 360◦Head Pose tracking combining3D Morphable Model and 3D Reconstruction
- Manhattan Room Layout Reconstruction from a Single 360◦ image: A Comparative Study of State-of-the-art Methods
- Pano Popups: Indoor 3D Reconstruction with a Plane-Aware Network
- Robust 3D reconstruction with omni-directional camera based on structure from motion
- CAN WE USE LOW-COST 360 DEGREE CAMERAS TO CREATE ACCURATE 3D MODELS

## [CNN](CNN)

- Learning Spherical Convolution for Fast Features from 360°Imagery
- Learning SO(3) Equivariant Representationswith Spherical CNNs (点云数据集)
- SpherePHD: Applying CNNs on a Spherical PolyHeDron Representation of 360-degree Images
- CONCENTRIC SPHERICAL GNN FOR 3D REPRESENTATION LEARNING
- SPHERICAL CNNS
- Rotation Equivariant Graph Convolutional Network for Spherical Image Classification
- Self-supervised Representation Learning Using 360◦ Data
- SphereNet: Learning Spherical Representations for Detection and Classification in Omnidirectional Images

## [Data Synthesis](Data%20Synthesis)
- BIPS: Bi-modal Indoor Panorama Synthesis via Residual Depth-aided Adversarial Learning
- Sat2Vid: Street-view Panoramic Video Synthesis from a Single Satellite Image
- Snap Angle Prediction for 360◦ Panoramas


## [Dataset](Dataset)

- Omnidata: A Scalable Pipeline for Making Multi-Task Mid-Level Vision Datasets from 3D Scans
- Refer360-degree: A Referring Expression Recognition Dataset in 360-degree Images
- 360-Indoor: Towards Learning Real-World Objects in 360◦ Indoor Equirectangular Images
- Recognizing Scene Viewpoint using Panoramic Place Representation
- Zillow Indoor Dataset: Annotated Floor Plans With 360o Panoramas and 3D Room Layouts
- Matterport3D: Learning from RGB-D Data in Indoor Environments
- A Saliency Dataset for 360-Degree Videos
- 360-degree Video Gaze Behaviour: A Ground-Truth Data Set and a Classification Algorithm for Eye Movements
- AVTrack360: An open Dataset and Soware recording people’sHead Rotations watching 360◦Videos on an HMD
- A Large-scale Compressed 360-Degree Spherical Image database: from Subjective Quality Evaluation to Objective Model Comparison
- A Dataset of Head and Eye Movements for 360 Degree Images

## [Depth Estimation](Depth%20Estimation)
- 360 Depth Estimation in the Wild -- The Depth360 Dataset and the SegFuse Network
- 360MonoDepth: High-Resolution 360° Monocular Depth Estimation
- ACDNet: Adaptively Combined Dilated Convolution for Monocular Panorama Depth Estimation
- BiFuse: Monocular 360-degree Depth Estimation via Bi-Projection Fusion
- Improving 360◦ Monocular Depth Estimation via Non-local Dense Prediction Transformer and Joint Supervised and Self-supervised Learning
- Distortion-Aware Convolutional Filters for Dense Prediction in Panoramic Images
- GLPanoDepth: Global-to-Local Panoramic Depth Estimation
- Geometric Structure Based and Regularized Depth Estimation From 360-degree Indoor Imagery
- OmniFusion : 360 Monocular Depth Estimation via Geometry-Aware Fusion
- PanoDepth: A Two-Stage Approach for Monocular Omnidirectional Depth Estimation
- SliceNet: deep dense depth estimation from a single indoor panorama using a slice-based representation
- OmniDepth: Dense Depth Estimation for Indoors Spherical Panoramas
- Spherical View Synthesis for Self-Supervised 360-degree Depth Estimation

## [Gaze following/Gaze estimation](Gaze%20following)
- Looking here or there? Gaze Following in 360-Degree Images
- Gaze Prediction in Dynamic 360◦ Immersive Videos
- Self-view Grounding Given a Narrated 360◦ Video
- Gaze360: Physically Unconstrained Gaze Estimation in the Wild

## [Highlight detection](Highlight%20detection)
- See360: Novel Panoramic View Interpolation
- A Deep Ranking Model for Spatio-Temporal Highlight Detection from a 360-degree Video

## [Image Compression](Image%20Compression)
- Pseudocylindrical Convolutions for LearnedOmnidirectional Image Compression

## [Image Super-resolution](Image%20Super-resolution)
- LAU-Net: Latitude Adaptive Upscaling Network for Omnidirectional Image Super-resolution
- SphereSR: 360-degree Image Super-Resolution with Arbitrary Projection via Continuous Spherical Image Representation

## [Inpainting](Inpainting)
- Panoramic Image Reflection Removal
- Privacy Protection in Street-View Panoramas using Depth and Multi-View Imagery

## [Object Detetction](Object%20Detetction)
- Field-of-View IoU for Object Detection in 360{%20deg} Images
- Deep 360 Pilot: Learning a Deep Agent for Piloting through 360◦ Sports Videos
- Spherical Criteria for Fast and Accurate 360-degree Object Detection
- Kernel Transformer Networks for Compact Spherical Convolution

## [Omnidirectional Localization](Omnidirectional%20Localization)
- PICCOLO: Point Cloud-Centric Omnidirectional Localization **(traditional)**
- OmniSLAM: Omnidirectional Localization and Dense Mapping for Wide-baseline Multi-camera Systems

## [Orientation Estimation](Orientation%20Estimation)
- Rotation Equivariant Orientation Estimation for Omnidirectional Localization

## [Outdoor Lighting Estimation](Outdoor%20Lighting%20Estimation)
- Learning High Dynamic Range from Outdoor Panoramas
- Spatially-Varying Outdoor Lighting Estimation from Intrinsics

## [Panoramic Stitching](Panoramic%20Stitching)
- Minimal Solutions for Panoramic Stitching Given Gravity Prior **(traditional)**

## [Room Layout Estimation](Room%20Layout%20Estimation)
- AtlantaNet: Inferring the 3D Indoor Layout from a Single 360◦ Image beyond the Manhattan World Assumption
- Deep3DLayout: 3D Reconstruction of an Indoor Layout from a Spherical Panoramic Image
- Pano2CAD: Room Layout From A Single Panorama Image
- DuLa-Net: A Dual-Projection Network for Estimating Room Layouts from a Single RGB Panorama
- HorizonNet: Learning Room Layout with 1D Representation and Pano Stretch Data Augmentation
- OmniLayout: Room Layout Reconstruction from Indoor Spherical Panoramas
- SSLayout360: Semi-Supervised Indoor Layout Estimation from 360◦ Panorama
- Joint 3D Layout and Depth Prediction from a Single Indoor Panorama Image
- Corners for Layout: End-to-End Layout Recovery From 360 Images
- LED2-Net: Monocular 360◦ Layout Estimation via Differentiable Depth Rendering
- Manhattan Room Layout Reconstruction from a Single 360 image: A Comparative Study of State-of-the-art Methods


## [Saliency Prediction](Saliency%20Prediction)
- Cube Padding for Weakly-Supervised Saliency Prediction in 360◦Videos
- SalGCN: Saliency Prediction for 360-Degree Images Based on Spherical Graph Convolutional Networks
- Rethinking 360° Image Visual Attention Modelling with Unsupervised Learning
- Saliency Detection in 360◦Videos
- Your Attention is Unique: Detecting 360-Degree Video Saliency in Head-Mounted Display for Head Movement Prediction
- 360-aware saliency estimation with conventional image saliency predictors **(traditional)


## [Scene Understanding](Scene%20Understanding)
- DeepPanoContext: Panoramic 3D Scene Understanding with Holistic Scene Context Graph and Relation-based Optimization
- PanoContext: A Whole-Room 3D Context Model for Panoramic Scene Understanding **(traditional)**
- Lighting, Reflectance and Geometry Estimation from 360◦ Panoramic Stereo
- HoHoNet: 360 Indoor Holistic Understanding with Latent Horizontal Features
- Automatic 3D Indoor Scene Modeling from Single Panorama
- Im2Pano3D: Extrapolating 360° Structure and Semantics Beyond the Field of View
- Eliminating the Blind Spot: Adapting 3D Object Detection and Monocular Depth Estimation to 360◦ Panoramic Imagery
- Recovering 3D existing-conditions of indoor structures from spherical images (traditional)


## [Stereo Matching](Stereo%20Matching)
- OmniMVS: End-to-End Learning for Omnidirectional Stereo Matching

## [Structure from Motion](Structure%20from%20Motion)
- Extreme Structure from Motion for Indoor Panoramas without Visual Overlaps

## [Survey](Survey)
- State-of-the-Art in 360° Video/Image Processing: Perception, Assessment and Compression
- A Survey on Adaptive 360◦ Video Streaming: Solutions, Challenges and Opportunities
- Annotated 360-Degree Image and Video Databases: A Comprehensive Survey
- 3D Scene Geometry Estimation from 360◦ Imagery: A Survey

## [Upright Adjustment](Upright%20Adjustment)
- 360o Camera Alignment via Segmentation
- Deep Upright Adjustment of 360 Panoramas Using Multiple Roll Estimations

## [VR Sickness Assessment](VR%20Sickness%20Assessment)
- VRSA Net: VR Sickness Assessment Considering Exceptional Motion for 360° VR Video
- Advanced Spherical Motion Model and Local Padding for 360° Video Compression **(traditional)**

## [Video Compression](Video%20Compression)
- Learning Compressible 360◦Video Isomers
- 

## [Video Summarization](Video%20Summarization)
- A Memory Network Approach for Story-Based Temporal Summarization of 360° Videos
- Pano2Vid: Automatic Cinematography for Watching 360-degree Videos

## [View Synthesis](View%20Synthesis)
- Automatic Content-aware Projection for 360◦ Videos **(traditional)**
- Deep Multi Depth Panoramas for View Synthesis

## [Visual Quality Assessment](Visual%20Quality%20Assessment)
- Viewport Proposal CNN for 360° Video Quality Assessment
- Cross-Reference Stitching Quality Assessmentfor 360◦Omnidirectional Images
- Cubemap-Based Perception-Driven Blind Quality Assessment for 360-degree Images
- MC360IQA: A Multi-channel CNN for Blind360-Degree Image Quality Assessment



## [Visual Question Answering](Visual%20Question%20Answering)
- Visual Question Answering on 360{%20deg} Images
- Pano-AVQA: Grounded Audio-Visual Question Answering on 360-degree Videos


## [semantic segmentation](semantic%20segmentation)
- Transfer beyond the Field of View: Dense Panoramic Semantic Segmentation via Unsupervised Domain Adaptation
- What’s in my Room? Object Recognition on Indoor Panoramic Images
- Bending Reality: Distortion-aware Transformers for Adapting to Panoramic Semantic Segmentation
- Omnisupervised Omnidirectional Semantic Segmentation
- DensePASS: Dense Panoramic Semantic Segmentation via UnsupervisedDomain Adaptation with Attention-Augmented Context Exchange
- DS-PASS: Detail-Sensitive Panoramic Annular Semantic Segmentation
- Capturing Omni-Range Context for Omnidirectional Segmentation
- Orientation-Aware Semantic Segmentation on Icosahedron Spheres

## Citation
If you found our survey helpful for your research, please cite our paper as:

```
@article{Ai2022DeepLF,
  title={Deep Learning for Omnidirectional Vision: A Survey and New Perspectives},
  author={Hao Ai and Zidong Cao and Jin Zhu and Haotian Bai and Yucheng Chen and Ling Wang},
  journal={ArXiv},
  year={2022},
  volume={abs/2205.10468}
}
```

