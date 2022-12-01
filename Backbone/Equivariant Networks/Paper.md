## Equivariant Networks for Pixelized Spheres

- **year**: 2021

- **Publication Conference**: ICML

- **Experimental Dataset**:  spherical MNIST, Stanford 2D3DS, and HAPPI20 climate data.

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) Various pixelizations or tilings of the sphere, often based on Platonic solids, have been used. Here, each face of the solid is refined using a triangular, hexagonal, or square grid and further recursive refinements can bring the resulting polyhedron closer and closer to a sphere, enabling an accurate projection from the surface of a sphere;

&nbsp; &nbsp; &nbsp; &nbsp; (2) While Platonic solids have well-known symmetries, their pixelization does not simply extend these symmetries.

&nbsp; &nbsp; &nbsp; &nbsp; (3) A natural improvement is to use the symmetry of the solid to dictate valid permutations of faces instead of assuming complete exchangeability.

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1)  Using the idea of block systems from permutation group theory, we are able to enforce inter-relations across different levels of the hierarchy, composed of the solid and face tilings. After identifying this symmetry transformation, we identify the family of equivariant maps for different choices of Platonic solid.

&nbsp; &nbsp; &nbsp; &nbsp; (2)  We also introduce an equivariant padding procedure to further improve the feed-forward layer.

- **Proposing Framework**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Equivariantnet.png" width="400" height="600">
</div>


- **Experimental Results**：

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Equivariantnet_result.png" width="300" height="250"><img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Equivariantnet_result1.png" width="300" height="300"><img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Equivariantnet_result2.png" width="300" height="300">
</div>


