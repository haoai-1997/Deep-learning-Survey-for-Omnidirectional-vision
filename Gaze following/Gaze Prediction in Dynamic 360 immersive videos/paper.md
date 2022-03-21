## Gaze Prediction in Dynamic 360◦ Immersive Videos

- year: 2018

- dataset：  **(208 360◦ videos captured in dynamic scenes)**  

- abstract: This paper explores gaze prediction in dynamic 360◦ immersive videos, i.e., based on the history scan path and VR contents, we predict where a viewer will look at an upcoming time. Our analysis shows that gaze prediction depends on its history scan path and image contents.

- Contributions:

i) to our knowledge, it is the **(first)** work that specifically tackles the gaze prediction task in dynamic 360◦ video
ii) we construct the first large-scale eye tracking database on 360◦ videos with a gaze tracker deployed in an HMD in a real immersive VR setting; 
iii) we employ a saliency-driven solution for gaze prediction, and extensive experiments validate the effectiveness of our method.

- structure:
Considering that the saliency measured at different scales is different, we propose to compute saliency maps at different spatial scales: the sub-image patch centered at current gaze point, the sub-image corresponding to the Field of View (FoV), and the panorama image. Then we feed both the saliency maps and the corresponding images into a Convolutional Neural Network (CNN) for feature extraction. Meanwhile, we also use a Long-Short-Term-Memory (LSTM) to encode the history scan path. Then we combine the CNN features and LSTM features for gaze displacement prediction between gaze point at a current time and gaze point at an upcoming time.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/GPin360degstructure.png)
- results：
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/GPin360degresult1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/GPin360degresult2.png)



- analysis: built **(the first large-scale eye-tracking dataset for dynamic 360◦ immersive videos)**, and analyze the dataset in details. Our analysis shows that **(temporal and spatial saliency, as well as history gaze path)**, are three important factors for gaze prediction.
