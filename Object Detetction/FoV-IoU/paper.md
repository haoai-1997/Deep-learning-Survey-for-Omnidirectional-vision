## Field-of-View IoU for Object Detection in 360{\deg} Images

- year: 2022

- dataset: 360 indoor dataset

- abstract: The paper proposes two fundamental techniques -- Field-of-View IoU and 360 Augmentation for object detection in 360 images.The FoV-IoU  computes the intersection-over-union of two Field-of-View bounding boxes in a spherical imagewhich could be used for training, inference, and evaluation while 360Augmentation is a data augmentation technique specific to 360° object detection task which randomly rotates a spherical image and solves the bias due to the sphere-to-plane projection.

- contributions:
(1) we propose a novel IoU computation method, namely FoV-IoU which better approximates the exact computation ofIoU between two FoV-BBs.
(2) we also propose 360Augmentation, a 360° image augmentation technique that can increase the diversity of training data while maintaining the spherical  coordinate mapping of the ERP image.
(3) The proposed method is compared with various 360-degree object detection methods on the 360-Indoor dataset, and is shown to perform well in combination with various existing perspective object detectors.

- structure:
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/FoV-IoU.png)

- result:
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/FoV-IoU_exp_1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/FoV-IoU_exp_2.png)

- analysis:
The limitation is, however, both FoV-IoU and Sph-IoU arestill an approximation of the spherical polygons and inevitably misevaluate the exact intersection areas. Our future work is toimprove the approximation accuracy for better object detectionin 360° images
