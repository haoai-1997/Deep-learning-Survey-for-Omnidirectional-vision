## SphereNet: Learning Spherical Representations for Detection and Classification in Omnidirectional Images

- **year**: 2018

- **Publication Conference**: ECCV
- **Experimental Dataset**:  Omni-MNIST, FlyingCars, and OmPaCa Dataset

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) Standard convolutional neural networks are not well suited for this scenario as the natural projection surface is a sphere which cannot be unwrapped to a plane without introducing significant distortions, particularly in the polar regions.

&nbsp; &nbsp; &nbsp; &nbsp; (2)  While CNNs are capable of learning invariances to common object transformations and intra-class variations, they would require significantly more parameters, training samples and training time to learn invariance to these distortions from data.

&nbsp; &nbsp; &nbsp; &nbsp; (3) The equirectangular image representation suffers from heavy distortions in the polar regions which implies that an object will appear differently depending on its latitudinal position.

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) Authors introduced SphereNet, a framework for learning spherical image representations by encoding distortion invariance into convolutional filters. SphereNet retains the original spherical image connectivity and, by building on regular convolutions, enables the transfer of perspective CNN models to omnidirectional inputs.

&nbsp; &nbsp; &nbsp; &nbsp; (2)  Authors improved the computational efficiency of SphereNet using an approximately uniform sampling of the sphere which avoids oversampling in the polar regions.

&nbsp; &nbsp; &nbsp; &nbsp; (3) Authors created two novel semi-synthetic and real-world datasets for object detection in omnidirectional images.

&nbsp; &nbsp; &nbsp; &nbsp; (4) Authors demonstrated improved performance as well as SphereNet's transfer learning capabilities on the tasks of image classification and object detection and compare our results to several state-of-the-art baselines.

- **Proposing Framework**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphereNetstructure.png" width="800" height="300">
</div>

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphereNetstructure1.png" width="800" height="400">
</div>

- **Experimental Results**：

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphereNetresult.png" width="800" height="320">
</div>
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphereNetresult1.png" width="800" height="320">
</div>
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphereNetresult2.png" width="800" height="320">
</div>

- **Analysis**：

Authors expected that with the increasing availability and popularity of omnidirectional sensors in both the consumer market (e.g., action cameras) as well as in industry (e.g., autonomous cars, virtual reality), the demand for specialized models for omnidirectional images such as SphereNet will increase in the near future. Authors therefore planned to exploit the flexibility of our framework by applying it to other related computer vision tasks, including semantic (instance) segmentation, optical flow and scene flow estimation, single image depth prediction and multi-view 3D reconstruction in the future.
