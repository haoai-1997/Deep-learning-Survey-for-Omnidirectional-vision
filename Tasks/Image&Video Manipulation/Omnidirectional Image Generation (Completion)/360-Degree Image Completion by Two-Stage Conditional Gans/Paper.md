## 360-Degree Image Completion by Two-Stage Conditional Gans

- **year**: 2019

- **Publication Conference**: ICIP

- **Experimental Dataset**:   the "Street"category from Sun360 Dataset (Not avaliable Now)

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) To the best of our knowledge, there are no GANs for generating 360-degree images. 

&nbsp; &nbsp; &nbsp; &nbsp; (2) This is a challenging problem because it is both an inverse problem that GANs convert incomplete images into complete 360-degree images and an ill-posed problem that the correct output is not only one and the relatively large area should be generated. 

&nbsp; &nbsp; &nbsp; &nbsp; (3) Head-mounted displays (HMD) are one of the most suitable devices for displaying a 360&deg; image. However,the images frequently used do not cover 360&deg; but have a narrower angle of view.

- **Challenge**:

&nbsp; &nbsp; &nbsp; &nbsp; (1)  This problem (360&deg; Image Completion) is related to inpainting, which involves recovering image content due to scratches or weathering, or removing unnecessary objects in an image.

&nbsp; &nbsp; &nbsp; &nbsp; (2)  This paper proposes the novel problem setting that by *using a known area from the 360-degree image as an input*, the remainder of the image can be completed with the GANs.

There are specific distortions in 360&deg; images of equirectangular projections. Therefore, one of the goals of this paper is to generate the distortion in outlines of the buildings and roads. Another goal is to generate content consistent with the input.

- **Proposing Framework**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Task/Image&Video Manipulation/360 Image Generation with Gans.png" width="1000" height="350">
</div>

&nbsp; &nbsp; &nbsp; &nbsp; The proposed approach has the following three points: (1) *to simplify the problem, they solve an inside completion problem instead of an outside completion problem by rearranging images*; (2) *In order to recognize the distortion that exists over a wide range of a 360-degree image and to generate distortions that are consistent between the input and output, we use dilated convolution layers*; (3) *They performtwo-stage generation to improve the quality of the final outputs*. 

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/51b78fc42016c5bbb34dee078edcea964d9b2808/Images/Task/Image&Video%20Manipulation/360%20Image%20Generation%20with%20Gans%20dilated.png" width="340" height="280"><img src="https://github.com/VLISLAB/360-DL-Survey/blob/51b78fc42016c5bbb34dee078edcea964d9b2808/Images/Task/Image&Video%20Manipulation/360%20Image%20Generation%20with%20Gans%20rearranging.png" width="460" height=280">
</div>

- **Experimental Results**：
  
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/0d1e83e40dda330c46157a5fff8c708665fc9213/Images/Task/Image&Video%20Manipulation/360%20Image%20Generation%20with%20Gans%20results1.png" width="800" height="400">
</div>
  
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/0d1e83e40dda330c46157a5fff8c708665fc9213/Images/Task/Image&Video%20Manipulation/360%20Image%20Generation%20with%20Gans%20results2.png" width="500" height="250"><img src="https://github.com/VLISLAB/360-DL-Survey/blob/0d1e83e40dda330c46157a5fff8c708665fc9213/Images/Task/Image&Video%20Manipulation/360%20Image%20Generation%20with%20Gans%20results3.png" width="500" height=250"><img src="https://github.com/VLISLAB/360-DL-Survey/blob/0d1e83e40dda330c46157a5fff8c708665fc9213/Images/Task/Image&Video%20Manipulation/360%20Image%20Generation%20with%20Gans%20results4.png" width="500" height=250">
</div>

&nbsp; &nbsp; &nbsp; &nbsp; Experimental results showed that the proposed methods are more effective to solve the problem than the baseline.

