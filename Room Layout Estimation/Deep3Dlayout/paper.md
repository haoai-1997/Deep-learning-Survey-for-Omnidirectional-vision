## Deep3DLayout: 3D Reconstruction of an Indoor Layout from a Spherical Panoramic Image


- year: 2021

- dataset：  **(AtlantaLayout dataset (non-MWM(Manhattan World Model)) and Pano3DLayout dataset)**  

- abstract: In this article, we introduce a novel deep learning technique capable to produce, at interactive rates, a tessellated bounding 3D surface from a single 360◦ image. A graph convolutional network directly infers the room structure as a 3D mesh by progressively deforming a graph-encoded tessellated sphere mapped to the spherical panorama, leveraging perceptual features extracted from the input image.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Deep3Dlayoutabstract.png)

- Contributions:

We build our network on top of HorizonNet and replace standard convolution operation with spherical convolution for enhanced representation and reduce computational complexity by replacing Bi-LSTM with Bi-GRU.

- structure:

Our network recovers the room structure by progressively deforming a 3D mesh so that its shape matches the environment seen by the viewer. **We can initialize the mesh to a 3D sphere, and then initialize
the sphere to a geodesic polyhedron obtained by regular subdivision of an icosahedron. Mesh deformation is
then driven by associating image features to mesh vertices.** we extract gravity-aligned features (GAF) and refine the association with vertices by exploiting long- and short-range relations, 

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Deep3Dlayoutstructure.png)


- results：

metrics: **(IoU3D;IoU2D;CD;𝐹𝜏0.1;𝐹𝜏0.3;𝐹𝜏0.5)**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Deep3Dlayoutresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Deep3Dlayoutresult1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Deep3Dlayoutresult2.png)
- analysis: Differently from prior solutions, all the components of our method address the problem in 3D, without resorting to 1D or 2D projections, and we produce as output a closed 3D mesh rather than a 2.5D model with strong planarity or surfaceorientation priors. In particular, inference times are well within interactivity constraints. **Failure: our spherical mesh topology is far from being sufficient to represent all sorts of architectural environments, since several elements of the architectural structure, such as pillars, stairs, septal walls or openings cannot be represented with a single closed surface.**
