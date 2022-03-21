## Viewport Proposal CNN for 360° Video Quality Assessment

- year: 2019

- dataset：  **( VQA-ODV dataset(largest VQA dataset for 360° video))**  

- abstract: this paper proposes a viewportbased convolutional neural network (V-CNN) approach for VQA on 360° video, considering both auxiliary tasks of viewport proposal and viewport saliency prediction
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VCNNabstract.png)

- Contributions:

1) We propose a viewport-based approach for VQA on 360° video, on the basis of real human behaviors when watching 360° video.
2) We embed auxiliary tasks to boost VQA, by predicting the HM(potential viewport) and EM(saliency within viewport) of subjects
3) Our approach outperforms the state-of-the-art approaches in VQA, and achieves comparable performance in the auxiliary tasks, i.e., viewport proposal and viewport saliency prediction.


- structure:
Our V-CNN approach is composed of two stages, i.e., viewport proposal and VQA. In the first stage, the viewport proposal network (VP-net) is developed to yield several potential viewports, seen as the first auxiliary task. In the second stage, a viewport quality network (VQ-net) is designed to rate the VQA score for each proposed viewport, in which the saliency map of the viewport is predicted and then utilized in VQA score rating. Consequently, another auxiliary task of viewport saliency prediction can be achieved.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VCNNstructure.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VCNNstructure1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VCNNstructure2.png)

- results：

view selection capability on Pano2Vid dataset; the temporal summarization with a newly
collected 360◦ video dataset, another domain, with image-based storytelling VIST dataset
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VCNNresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/VCNNresult1.png)


- analysis: Our approach is in accordance with the human’s way of watching 360° video, since the observers can only see viewports. 

Our VCNN approach consists of two stages, i.e., viewport proposal and VQA. 

In the **(first stage)**, the VP-net was developed with a viewport softer NMS for proposing potential viewports. In this stage, the first auxiliary task of viewport proposal is achieved. 

In the **(second stage)**, we designed a VQnet to rate the VQA score of each proposed viewport. In the VQ-net, the saliency map of each proposed viewport is predicted, as the second auxiliary task; then it is used for VQA of the viewport. **(Subsequently, the main task of VQA on 360° video is accomplished by integrating the VQA scores of all proposed viewports.)**
