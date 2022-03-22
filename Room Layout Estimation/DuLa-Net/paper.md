## DuLa-Net: A Dual-Projection Network for Estimating Room Layouts from a Single RGB Panorama

- year: 2019

- dataset: PanoContext dataset, and Realtor360 dataset (self-collected)

- Abstract: We present a deep learning framework, called DuLa-Net, to predict Manhattan-world 3D room layouts from a single RGB panorama. To achieve better prediction accuracy, our method leverages two projections of the panorama at once, namely the equirectangular panorama-view and the perspective ceiling-view, that each contains different clues about the room layouts. To learn more complex room layouts, we introduce the Realtor360 dataset.
- Contributions:
(1) We propose a novel network architecture that con- tains two encoder-decoder branches to analyze the in- put panorama in two different projections. These two branches are further connected through a feature fusion scheme. This dual-projection architecture can infer room layouts with more complex shapes beyond cuboids and L-shapes.
(2) Our neural network is an important step towards build- ing an end-to-end architecture. Our network directly outputs a probability map of the 2D floor plan. This output requires significantly less post-processing to obtain the final 3D room layout than the output of the current state of the art.
(3) We introduce a new data set, called Realtor360, that contains 2573 panoramas depicting rooms with 4 to 12 corners. To the best of our knowledge, this is largest data set of indoor images with room layout annotations currently available.

- Structure: Dual-branch (panorama-view and ceiling-view)

<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/dualnet.png" width="70%" height="70%">

- Results：
  <img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/dualnet_exp1.png" width="50%" height="50%">

-Analysis: Utilize two projection views (panorama-view and ceiling-view) at once to achieve better performance.
