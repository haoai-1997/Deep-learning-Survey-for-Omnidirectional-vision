## Self-view Grounding Given a Narrated 360◦ Video

- year: 2018

- dataset：  **360 Videos Dataset: self-collected the first narrated 360◦ videos dataset**  

- we aim at automatically grounding the Normal Field of View (NFoVs) of a 360◦ video given subtitles of the narrative (referred to as “NFoV-grounding”). We propose a novel Visual Grounding Model (VGM) to implicitly and efficiently predict the NFoVs given the video content and subtitles. 
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VGMabstract.png)

- Contributions:

1) We define a new ”NFoV-grounding” task which is essential to automatic assist watching 360◦ videos
2) We propose a novel Visual Grounding Model (VGM) to implicitly and efficiently infer NFoV.
3) We introduce a novel irrelevant loss and a 360◦ data augmentation technique to robustly train our model.
4) We collect the first narrated 360◦ video dataset and achieve the best performance.

- structure:

1) at each frame, we efficiently encode the panorama into feature map of candidate NFoVs using a Convolutional Neural Network (CNN) and the subtitles to the same hidden space using a RNN with Gated Recurrent Units (GRU). 
2) Then, we apply soft-attention on candidate NFoVs to trigger sentence decoder aiming to minimize the reconstruct loss between the generated and given sentence. 
3) we obtain the NFoV as the candidate NFoV with the maximum attention without any human supervision.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VGMstructure.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VGMdataset.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VGMdataset1.png)



- results：

metrics: **(avg. Recall (%) avg. Precision (%))**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VGMresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VGMresult1.png)

- analysis: We introduce a new NFoV grounding task which aims to ground subtitles (i.e., natural language phrases) into corresponding views in each 360◦ video. To tackle this task, we propose a novel model with two main innovations: (1) train the network with both of relevant and irrelevant softattention visual features, and (2) apply NFoV proposal in feature space for saving time-consuming, memory usage, and making end-to-end training feasible.
