## Learning Compressible 360◦Video Isomers

- year: 2015

- dataset：  **360◦video dataset (self prposed)** 

- abstract: We introduce an approach to predict the sphere rotation that will yield the maximal compression rate. Given video clips in their original encoding, a convolutional neural network learns the association between a clip’s visual content and its compressibility at different rotations of a cubemap projection. Given a novel video, our learning-based approach efficiently infers the most compressible direction in one shot, without repeated rendering and compression of the source video.

- structure：learn spherical convolutions in equirectangular projection given a target networktrained on perspective images
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/360Isomers_structure.png)

- analysis: his work studies how to improve 360◦video compression by selecting a proper orientation for cubemap projec-tion. Our analysis across 3 popular codecs shows scope for reducing video sizes by up to 77% through rotation, with an average of more than 8% over all videos. We propose an approach that predicts the optimal orientation given the video in a single orientation. It achieves 82% the compres-sion rate of the optimal orientation while requiring less than 0.3%of the computation of a non-learned solution (fraction of a second vs. 1.5 hours per GOP).
