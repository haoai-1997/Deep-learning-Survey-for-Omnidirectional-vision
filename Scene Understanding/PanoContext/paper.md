## PanoContext: A Whole-room 3D Context Modelfor Panoramic Scene Understanding
- year: 2020

- dataset：  **(Annotated 3D panorama dataset : PanoContext)**  

- abstract: For an input panorama, our method outputs 3D bounding boxes ofthe room and all major objects inside, together with their semantic categories. Ourmethod generates 3D hypotheses based on contextual constraints and ranks thehypotheses holistically, combining both bottom-up and top-down context infor-mation.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PanoContextabstract.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PanoContextdataset.png)

- analysis: We construct an annotated panorama dataset and re-construct the 3D model from single-view using manual annotation. Experiments show that solely based on 3D context without any image-based object detector,we can achieve a comparable performance with the state-of-the-art object detec-tor. **(This demonstrates that when the FOV is large, context is as powerful as object appearance)**
