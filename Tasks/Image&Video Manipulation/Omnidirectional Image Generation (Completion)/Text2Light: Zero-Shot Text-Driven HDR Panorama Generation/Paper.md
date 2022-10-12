## Diverse Plausible 360-Degree Image Outpainting for Efficient 3DCG Background Creation

- **year**: 2022

- **Publication Conference**: SIGGRAPH Asia

- **Experimental Dataset**:  HDR360-UHD DATASET (the authors combined the existing datasets and newly collected panoramas, and the dataset contains 4392 HDR panoramas with resolutions ranging from 4096 × 2048 (4K) to 8192 × 4096 (8K)).

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; Given the difficulty of capturing HDRIs, a versatile and controllable generative model is highly desired, where layman users can intuitively control the generation process. However, existing state-of-the-art methods still struggle to synthesize high-quality panoramas for complex scenes. 

- **Contribution**:


&nbsp; &nbsp; &nbsp; &nbsp; Specifically, to achieve **zero-shot text-driven panorama generation**, the authors first built **dual codebooks** as the discrete representation for diverse environmental textures. Then, driven by the pre-trained Contrastive Language-Image Pre-training (CLIP) model, a **text-conditioned global sampler** learns to *sample holistic semantics from the global codebook according to the input text*. Furthermore, a **structure-aware local sampler** learns to synthesize LDR panoramas patch-by-patch, guided by holistic semantics. To achieve super-resolution inverse tone mapping, we derive a *continuous representation of 360-degree imaging from the LDR panorama* as a set of structured latent codes anchored to the sphere. This continuous representation enables a versatile module to upscale the resolution and dynamic range simultaneously. 

- **Proposing Framework**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/ae989ab649b766168fd807bfafc09c81cb68fe00/Images/text2pano1.png" width="1000" height="250">
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
