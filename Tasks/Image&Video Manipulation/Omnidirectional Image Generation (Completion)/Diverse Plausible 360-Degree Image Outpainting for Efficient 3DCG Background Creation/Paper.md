## Diverse Plausible 360-Degree Image Outpainting for Efficient 3DCG Background Creation

- **year**: 2022

- **Publication Conference**: CVPR

- **Experimental Dataset**:  Sun360 Dataset (Not avaliable Now) and Laval Indoor dataset (avaliable Now).

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; (1) Previous methods, for generating a 360&deg; image from a single image with a narrow field of view (NFoV), suffered from **overfitting to the training resolution and deterministic generation**.

&nbsp; &nbsp; &nbsp; &nbsp;  For example, as shown in following figure, existing method 360IC (*360-Degree Image Completion by Two-Stage Conditional Gans*), trained at 512×256, produces many artifacts at 1024×512. The authors believe that **this is due to distortions caused by the equirectangular projection (ERP)**. 
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/93f9be7c54566b5c359ed4fa135431bf3272f672/Images/Task/Image&Video%20Manipulation/Diverse%20Plausible%20360%20Image%20Outpainting_comparison.png" width="400" height="380">
</div>

- **Goal**:


&nbsp; &nbsp; &nbsp; &nbsp; First, this paper addresses the problem of converting an NFoV image into a 360&deg; image by complementing its surroundings to obtain a 360-degree environment consistent with the image given as a partial background.


&nbsp; &nbsp; &nbsp; &nbsp; More specially, The goal of this paper is to realize the outpainting of 360&deg; images with the following two properties:

&nbsp; &nbsp; &nbsp; &nbsp;  (1) Sample diverse outputs for a single input.

&nbsp; &nbsp; &nbsp; &nbsp;  (2) infer arbitrary resolutions.

- **Contribution**:

&nbsp; &nbsp; &nbsp; &nbsp; (1)   The authors proposed AdjustmentNet to introduce a transformer into 360&deg; image outpainting, which enables diverse and arbitrary-resolution outputs

&nbsp; &nbsp; &nbsp; &nbsp; (2)   The authors proposed two novel techniques for acquiring the properties of 360&deg; images: **WS-perceptual loss for the training of CompletionNets** and **circular inference for the transformer**. 

- **Proposing Framework**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/8718eaa56d626e2d048182ba41fe27c33e45e1e3/Images/Task/Image&Video%20Manipulation/Diverse%20Plausible%20360%20Image%20Outpainting_framework.png" width="1000" height="250">
</div>

&nbsp; &nbsp; &nbsp; &nbsp; The authors present a framework comprising *CompletionNets* and *AdjustmentNet*. (1) CompletionNets is an image completion module that uses the same networks as TT (*Taming Transformers for High-Resolution Image Synthesis*) and two novel techniques to be proposed later. (2) AdjustmentNet improves the consistency of color, stitching, and resolution between the output result of CompletionNets and the input image.  Because AdjustmentNet adjusts the fixed-size output of CompletionNets to the size of the input image, we can obtain completion results for any image resolution.

Furthermore, considering the unique properties of 360-degree images, the authors proposed two novel techniques : (1)  to achieve continuity at both ends of an image,  **circular inference** is proposed as a new auto-regressive order for a transformer. (2)  to further improve the perceptual quality, a **WS-perceptual loss** function is provided for training of CompletionNets

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/d2c861440347ac12c79a9bd5134be3300b80ea28/Images/Task/Image&Video%20Manipulation/Diverse%20Plausible%20360%20Image%20Outpainting_circular.png" width="400" height="300">
</div>

- **Experimental Results**：

&nbsp; &nbsp; &nbsp; &nbsp; As a quantitative metric, Fr ́echet inception distance (FID) is employed to evaluate the quality and diversity of the generated images

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/e236f65832229c48b85c23ce1e35680bdc4bcbc4/Images/Task/Image&Video%20Manipulation/360%20Image%20Generation%20with%20Gans%20results1.png" width="750" height="300">
</div>

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/e236f65832229c48b85c23ce1e35680bdc4bcbc4/Images/Task/Image&Video%20Manipulation/360%20Image%20Generation%20with%20Gans%20results2.png" width="450" height="240">
</div>

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/e236f65832229c48b85c23ce1e35680bdc4bcbc4/Images/Task/Image&Video%20Manipulation/360%20Image%20Generation%20with%20Gans%20results3.png" width="450" height="200">
</div>
 
- **Limitations (provided in the paper)**：

&nbsp; &nbsp; &nbsp; &nbsp; (1) **Inference time and computational memory**. Our method takes approximately 30 s for one completion on a single 2080Ti, mainly because of a transformer. However, since 3DCG designers, the subject of our work, are likely to use PCs and servers with high-end GPUs, the performance of our method may be sufficient for practical use.

&nbsp; &nbsp; &nbsp; &nbsp; (2) **Controllability**. The proposed method does not control what is generated in the completion region. One possible solution is to paste an object that appears directly in the completion region and complete it so that it is smoothly connected.
