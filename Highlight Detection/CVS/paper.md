## A Deep Ranking Model for Spatio-Temporal Highlight Detection from a 360-degree Video

- year: 2018

- dataset: Pano2Vid dataset and 360-degree video highlight dataset (self-collected)

- Abstract: We address the problem of highlight detection from a 360-degree video by summarizing it both spatially and temporally. Given a long 360-degree video, we spatially select pleasantly-looking normal field-of-view (NFOV) segments from unlimited field of views (FOV) of the 360-degree video, and temporally summarize it into a concise and informative highlight as a selected subset of subshots.
- Contributions:
(1) Our work is the first attempt to summarize 360-degree videos both spatially and temporally for highlight detection. To this end, we develop a novel deep ranking model and collect a new dataset of 360-degree videos from YouTube and Vimeo.
(2) We propose Composition View Score (CVS) model, which produces a spherical composition score map of composition per video segment of 360-degree videos, and determines which view is suitable for highlight via a sliding window kernel at inference.

- Structure: CVS model

<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/CVS.png" width="70%" height="70%">

- Results：
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/CVS_exp1.png" width="50%" height="50%">
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/CVS_exp2.png" width="50%" height="50%">

-analysis: 将room layout工作进行拆分成，surface normal estimation, 2D object detection and 3D object pose estimation,利用生成模型和概率论进行参数推理。

