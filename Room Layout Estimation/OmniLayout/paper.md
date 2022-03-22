## OmniLayout: Room Layout Reconstruction from Indoor Spherical Panoramas

- year: 2021

- dataset：  **(PanoContext and Stanford 2D-3D)**  

- abstract: We propose to use spherical convolutions. The resulting network, which we call OmniLayout performs convolutions directly on the sphere surface, sampling according to inverse equirectangular projection and hence invariant to equirectangular distortions. 
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/OmniLayoutabstract.png)

- Contributions:

We build our network on top of HorizonNet and replace standard convolution operation with spherical convolution for enhanced representation and reduce computational complexity by replacing Bi-LSTM with Bi-GRU.

- structure:

The proposed architecture consists of a ResNet-50 encoder with proposed spherical convolutions. We remove the final fully-connected layer and concatenate the features from different levels and pass it to a Bi-Directional Gated Recurrent Unit (Bi-GRU) that predicts the layout floor-wall boundary (yf), ceiling-wall boundary (yc), and wall-wall boundary (yw).

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/OmniLayoutstructure.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/OmniLayoutstructure1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/OmniLayoutstructure2.png)

- results：

metrics: **(Pixel Error (%);  Corner Error (%) ;3D IoU  Error (%))**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/OmniLayoutresult.png)


- analysis: In our knowledge this is the first work in room layout estimation that uses the equirectangular projection function to reduce the distortions. The proposed method, OmniLayout is computationally efficient and can also recover both cuboid shaped layouts as well non-cuboid shaped layouts (“L-shaped”).
