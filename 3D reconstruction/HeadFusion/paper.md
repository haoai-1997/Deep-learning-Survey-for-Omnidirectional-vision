## HeadFusion: 360◦Head Pose tracking combining3D Morphable Model and 3D Reconstruction

- year: 2018

- dataset: BIWI dataset, UBImpressed Dataset

- abstract:
3DMM models usually only cover the face region，so that we require frontal or mid-profile poses to do Head pose estimation, which peclude a large set of applications where such conditions can not be garanteed,
In this paper, we present a famework which combines the strengths of a 3DMM model fitted online with a prior-free reconstruction of a 3D full head model providing support for pose estimation from any viewpoint. 
In addition, we also proposes a symmetry regularizer for accurate 3DMM fitting under partial observations, and exploit visual tracking to address natural head dynamics with fast accelerations.

- contribution
(1) A 3D head representation combining the semantic and the precision of a 3DMM fitting and tracking under restricted poses with the robustness of a full head representation reconstructed from depth data.
(2) A  symmetry regularizer for robust online  3DMM adaptation
(3) A framework exploiting both visual motion trackingand 3D model semantics for frame-to-frame pose initialization
(4) Extensive experiments and results beyond the state-of-the-art on both a public benchmark dataset(BIWI) and videos from natural role played inter-actions.

- structure:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/HeadFusion_framework.png)

- result:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/UBImpressed_result.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/UBimpressed_landmark_position_result.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/BIWI_result.png)

- future work
Our work can also be expanded to other tasks, by serving as a preprocessing step for head gesture recognition, eye gaze tracking,or facial expression estimation
