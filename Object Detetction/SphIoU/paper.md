## Spherical Criteria for Fast and Accurate 360-degree Object Detection

- year: 2020

- dataset: VOC360 dataset (self-collected), COCO-Men dataset (self-collected), and SUN360 dataset

- Abstract: In this paper, we introduce a novel spherical criteria for fast and accurate 360 object detection, including both spherical bounding boxes and spherical IoU (SphIoU). Based on the spherical criteria, we propose a novel two-stage 360-degree detector, i.e., Reprojection R-CNN, by combining the advantages of both ERP and PSP, yielding efficient and accurate 360◦ object de- tection. 

- Contributions:
(1) We introduce spherical criteria as an efficient and accurate approximation of unbiased measurement, including both spherical BB (SphBB) and spherical IoU (SphIoU).
(2) We propose a novel two-stage object detector, i.e., Reprojection R-CNN (Rep R-CNN), by taking full advantage of both ERP and PSP.
(3) Due to the lack of unbiased dataset for 360◦ object detection, we construct two datasets, i.e., VOC360 and COCO-Men.

- Structure: R-CNN

<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphIoU.png" width="70%" height="70%">

- Results：
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SphIoU_exp1.png" width="50%" height="50%">

-Analysis: This work proposes a new 360 citeria for object detection. They also provide a R-CNN architecture which performs best in experiments. In addition, they also provide two self-collected datasets.




