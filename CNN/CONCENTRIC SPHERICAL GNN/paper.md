## CONCENTRIC SPHERICAL GNN FOR 3D REPRESENTATION LEARNING

- year: 2021

- dataset: ModelNet40 dataset

- Abstract: We propose a novel multi-resolution convolutional architecture for learning over concentric spherical feature maps, of which the single sphere representation is a special case. Our hierarchical architecture is based on alternatively learning to incorporate both intra-sphere and inter-sphere information.
- Contributions:
(1) We propose a new multi-sphere icosahedral discretization for representation of 3D data, and show that incorporating the radial dimension can greatly enhance representation ability over single-sphere representations.
(2) We also introduce a novel convolutional architecture for multi-sphere discretization by introducing two
different types of convolutions, graph convolution and radial convolutions, for incorporating intra-sphere and inter-sphere information. Their combined use leads to an expressive architecture that is also rotationally equivariant. Our proposed convolutions are also scalable, being linear with respect to the discretization size.
(3) We design mappings of both 3D mesh objects and general point clouds to the proposed representation. We achieve new state-of-the-art performance on ModelNet40 point cloud classification, using the proposed model and an input data mapping based on radial basis functions. We also outperform existing Spherical CNN performance in SHREC17 3D mesh classification.


- Structure: GNN

<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/CONCENTRIC_1.png" width="70%" height="70%">
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/CONCENTRIC_2.png" width="70%" height="70%">


-Analysis: This paper proposes an effective learning representation of 3D data (point clouds/meshes) using a spherical GNN architecture over concentric spherical maps. Evaluation is done through 3D classification tasks.
