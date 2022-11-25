## Geometry Aware Convolutional Filters for Omnidirectional Images Representation

- **year**: 2019

- **Publication Conference**: ICML

- **Experimental Dataset**: Image classifcation (Spherical dataset, Mod-spherical dataset, Fish-eye dataset, Cube-map dataset); Image Compression (the modified version of the dataset (Recognizing scene viewpoint using panoramic place representation)).

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) The images captured by 360&deg; cameras, are often analyzed and classified with techniques designed for planar images that unfortunately fail to properly handle the native geometry of such images and therefore results in suboptimal performance.

&nbsp; &nbsp; &nbsp; &nbsp; (2) In the context of omnidirectional cameras, CNNs are typically applied directly to the unwrapped and distorted spherical images. This approach, however, is suboptimal: due to specific geometry of these images, and, in particular, the change in the image statistics with the position in the image. The latter forces the network to learn different filters for different locations in the omnidirectional images

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) Replace ordinary convolutional filters with the graph-based ones that can adapt their size and shape depending on the position in the omnidirectional image thanks to the flexible graph structure.

&nbsp; &nbsp; &nbsp; &nbsp; (2)  In order to overcome the common limitation of these graph-based filters being isotropic (i.e. invariant to the changes in the objects orientation in the image) we suggest to use multiple directed graphs instead of a single undirected one. This permits our method to encode the orientation of the objects that appear in the images and, therefore, extract more meaningful features from them.

- **Proposing Framework**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/GAFilters.png" width="500" height="400">
</div>
