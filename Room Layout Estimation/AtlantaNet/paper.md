## AtlantaNet: Inferring the 3D Indoor Layout from a Single 360◦ Image beyond the Manhattan World Assumption

- year: 2020

- dataset：**(PanoContext; Stanford 2D-3D; Matterport3D;  a specific testing set of a hundred images: AtlantaLayout)**  

- abstract:  Compared to recent stateof-the-art works, our method is not limited to Manhattan World environments, and can reconstruct rooms bounded by vertical walls that do not form right angles or are curved – i.e., Atlanta World models. To predict the 3D layout, we propose an encoder-decoder neural network architecture, leveraging Recurrent Neural Networks (RNNs) to capture long-range geometric patterns, and exploiting a customized training strategy based on domain-specific knowledge.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/AtlantaNetabstract.png)

- Contributions:
1) We introduce a data encoding based on the Atlanta World indoor model, that allows layout prediction on planar projections free from spherical image deformations, unlike previous approaches that are predominantly based on features extracted from the equirectangular view.
2) We reconstruct the 3D layout, in terms of 2D footprint and room height, by inferring the 2D layout from the contour of a solid segmentation masks and the room height from the geometric analysis of the correlation between two contours.
3) We propose an end-to-end network that does not require heavy pre-processing and a training strategy based on feeding both ceiling and floor view on the same network instance.

- structure: The network takes as an input a transform of size 3×w×w and produces a segmentation mask of size 1×w×w.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/AtlantaNetstructure.png)


- results：
metrics: **((3D IoU, Corner Error, Pixel Error, 2D IoU, δi)**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/AtlantaNetresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/AtlantaNetresult1.png)

- analysis: We have introduced a novel end-to-end approach to predict the 3D room layout from a single panoramic image. We project the original panoramic image on two horizontal planes, one above and one below the camera, and use a suitably traineddeep neural network to recover the inside-outside segmentation mask of these two images. The upper image mask, which contains less clutter, is used to determine the 2D floor plan in form of a polygonal layout, while the correlation between upper and lower mask is used to determine the room height under the Atlanta world model.

- Limitations: From the topological point-of-view, the condition that (the recovered shape does not describe the real room layout) happens where the horizontal planes are not clearly identifiable, so, in our example, when the horizontal ceiling is partially occluded by other horizontal structures.
