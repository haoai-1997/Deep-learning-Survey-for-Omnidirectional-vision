## 360 Depth Estimation in the Wild -- The Depth360 Dataset and the SegFuse Network

- year: 2022

- dataset: Depth360 (achieved by exploring the use of a plenteous source of data, 360 videos from the internet, using a test-time training method that leverages unique information in each omnidirectional sequence.)

- abstract: In this work, we first establish a large-scale dataset with varied settings called Depth360 to tackle the training data problem.
We then propose an end-to-end two-branch multi-task learning network, SegFuse, that mimics the human eye to effectively learn from the dataset and estimate high-quality depth maps from diverse monocular RGB images.
Our method predicts consistent global depth while maintaining sharp details at local regions.

- contributions:
(1) The paper proposes to utilize omni-directional video in the wild to generate a large-scale dataset, Depth360.
(2) The paper proposes an end-to-end two-branch multi-task architecture called SegFuse that estimates depth from a single-view 360 im-age input by mimicking the human eye.
(3) We perform an extensive evaluation against state-of-the-art omnidirectional datasets and methods and present a better quantitative and qualitative performance.

- structure:
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Depth360Gen.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SegFuse.png)

- loss function

inverse Huber loss

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Huber_Loss_func_1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Huber_loss_func_2.png)

- result:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/360DataGen.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SegFuse_result.png)


