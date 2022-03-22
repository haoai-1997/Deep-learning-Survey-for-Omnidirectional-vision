## Pano-AVQA: Grounded Audio-Visual Question Answering on 360-degree Videos

- year: 2021

- dataset: Pano-AVQA (self-collected)

- Abstract: We propose a novel benchmark named Pano-AVQA as a large- scale grounded audio-visual question answering dataset on panoramic videos. We train several transformer-based models from Pano-AVQA, where the results suggest that our proposed spherical spatial embeddings and multimodal training objectives fairly contribute to a better semantic understanding of the panoramic surroundings on the dataset.
- Contributions:
 1. We propose novel benchmark tasks on spatial and audio-visual question answering on 360◦ videos towards a holistic semantic understanding of omnidirec- tional surroundings.
2. Since there is no existing dataset for this objective to the best of our knowledge, we contribute Pano-AVQA as the first large-scale spatial and audio-visual question answering dataset on 360◦ videos, consisting of 51.7K question-answer pairs with bounding box grounding.
3. We design an audio-visual question answering model for 360◦ videos that effectively fuses multimodal cues from the panoramic sphere. We incorporate this model with several baseline systems and evaluate them on the Pano-AVQA dataset.

- Structure: Transformer

<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/panoavqa_1.png" width="70%" height="70%">
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/panoavqa_2.png" width="70%" height="70%">

- Results：
  <img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/BiFuse_exp1.png" width="50%" height="50%">

-Analysis: Utilize two projection formats of 360-degree images to better extracting and fusing information.
