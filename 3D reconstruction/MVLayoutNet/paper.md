## MVLayoutNet: 3D layout reconstruction with multi-view panoramas

- conference: Arxiv, 2021

- dataset: 2D-3D-S, ZInD

- abstract: The proposed MVS module
takes a newly-proposed layout cost volume, which aggregates multi-view 
costs at the same depth layer into cor-responding layout elements. We additionally provide an
attention-based scheme that guides the MVS module to fo-cus on structural regions. 
Such a design considers both lo-cal pixel-level costs and global holistic information for bet-ter reconstruction.

- contributions: 
(1) We present an end-to-end network that seamlessly combines layout estimation and multiview stereo for large-scale scene layout reconstruction.
(2) We propose a layout cost volume with a novel MVS module that performs 1D probability regression on ab- stract layout elements.
(3) We use explicit semantics and weakly supervised self- attention to enforce structural analysis.
(4) Experiments highlight contributions of our key designs and significant quality improvement from the state-of- the-arts.

- Framework:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/layout%20reconstruction/MVLayoutNet_Framwork.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/layout%20reconstruction/MVLayoutNet_framework2.png)

- results:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/layout%20reconstruction/MVLayoutNet_result.png)
