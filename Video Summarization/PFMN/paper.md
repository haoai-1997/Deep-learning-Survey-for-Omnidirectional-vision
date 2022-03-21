## A Memory Network Approach for Story-Based Temporal Summarization of 360° Videos


- year: 2018

- dataset：  **( Pano2Vid dataset,  image-based storytelling VIST dataset )**  

- abstract: We address the problem of **(story-based temporal summarization of long 360◦ videos)**. We propose a novel memory network model named Past-Future Memory Network (PFMN), in which we first compute the scores of 81 normal field of view (NFOV) region proposals cropped from the input 360◦ video, and then recover a latent, collective summary using the network with two external memories that store the embeddings of previously selected subshots and future candidate subshots.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PFMNabstract.png)
- Contributions:

i) our work is the first to address story-based temporal summarization of 360◦ videos
ii) our model is the first attempt to leverage memory networks for video summarization tasks

- structure:
The unique updates of PFMN include (i) exploiting an additional memory for future context, and (ii) correlating the future context and previously selected subshots to select the next summary subshot at each iteration.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PFMNstructure1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PFMNstructure.png)
- results：

view selection capability on Pano2Vid dataset; the temporal summarization with a newly
collected 360◦ video dataset, another domain, with image-based storytelling VIST dataset
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PFMNresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PFMNresult1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/PFMNresult2.png)

- analysis: **(Two external memories)** to store the embeddings of previously selected subshots
and future candidate subshots.
