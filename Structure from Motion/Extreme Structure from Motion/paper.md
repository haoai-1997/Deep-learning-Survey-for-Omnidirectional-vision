## Extreme Structure from Motion for Indoor Panoramas without Visual Overlaps


- year: 2021

- dataset：**( a dataset of 1029 panorama images with 286 houses)**  

- abstract: This paper proposes an extreme Structure from Motion (SfM) algorithm for residential indoor panoramas that have little to no visual overlaps.  Our idea is to learn to evaluate the realism of room/door/window arrangements in the topdown semantic space. After using heuristics to enumerate possible arrangements based on door detections, we evaluate their realism scores, pick the most realistic arrangement, and return the corresponding camera poses.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ESFMabstract.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ESFMdataset.png)
- Contributions:

1) A new extreme indoor SfM problem with the new dataset for the exploding market;
2) One-of-a-kind SfM algorithm which learns to evaluate the arrangement of semantic information;
3) State-of-the-art performance where existing techniques fail

- structure: We extract the architectural semantic information from each panorama and re-project into a “Nadir semantic representation”, which cuts the flow of raw pixel information and avoids network over-fitting. After generating arrangement candidates by aligning doors in the semantic images, a convolutional message passing neural network learns to evaluate the realism of the arrangements.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ESFMstructure.png)


- results：
metrics: **(success-rate (where a method is defined to be a success if top-K reconstructions contain a solution, whose mean positional error is below δ meters.))**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ESFMresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ESFMresult1.png)

- analysis: This paper introduces a new extreme SfM problem for indoor panoramas and proposes a unique SfM algorithm, which learns to evaluate the arrangement of rooms/doors/windows without solving a correspondence problem. Our algorithm makes significant improvements over the current state-of-the-art, which completely fails for every single example.

- **future**: the running time is exponential in the number of panoramas and the algorithm highly depends on the door detection, in particular, is not able to recover from missing doors.
