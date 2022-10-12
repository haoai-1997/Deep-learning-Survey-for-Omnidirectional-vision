## Text2Light: Zero-Shot Text-Driven HDR Panorama Generatio

- **year**: 2022

- **Publication Conference**: SIGGRAPH Asia

- **Experimental Dataset**:  HDR360-UHD DATASET (the authors combined the existing datasets and newly collected panoramas, and the dataset contains 4392 HDR panoramas with resolutions ranging from 4096 × 2048 (4K) to 8192 × 4096 (8K)).

- **Motivation**:

&nbsp; &nbsp; &nbsp; &nbsp; Given the difficulty of capturing HDRIs, a versatile and controllable generative model is highly desired, where layman users can intuitively control the generation process. However, existing state-of-the-art methods still struggle to synthesize high-quality panoramas for complex scenes. 

- **Contribution**:
<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/ae989ab649b766168fd807bfafc09c81cb68fe00/Images/text2pano1.png" width="1000" height="500">
</div>

&nbsp; &nbsp; &nbsp; &nbsp; Specifically, to achieve **zero-shot text-driven panorama generation**, the authors first built **dual codebooks** as the discrete representation for diverse environmental textures. Then, driven by the pre-trained Contrastive Language-Image Pre-training (CLIP) model, a **text-conditioned global sampler** learns to *sample holistic semantics from the global codebook according to the input text*. Furthermore, a **structure-aware local sampler** learns to synthesize LDR panoramas patch-by-patch, guided by holistic semantics. To achieve super-resolution inverse tone mapping, we derive a *continuous representation of 360-degree imaging from the LDR panorama* as a set of structured latent codes anchored to the sphere. This continuous representation enables a versatile module to upscale the resolution and dynamic range simultaneously. 

- **Proposing Framework**:

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/e1c2300ccfdabebdd2bf414e3d3a6b701c28f746/Images/text2pano2.png" width="1000" height="650">
</div>

&nbsp; &nbsp; &nbsp; &nbsp; The authors presented Text2Light, the first framework for zero-shot text-driven HDR panorama generation. Due to the complexity of HDR panorama in detailed textures, spherical structure, and high dynamic range, the authors decomposed the generation process into two dedicated stages. 1) Stage I generates a 360-degree panorama in low dynamic range (LDR) and low resolution (LR) given a description of the scene as the input. 2) Stage II upscales the result of Stage I both in resolution and dynamic range by a super-resolution inverse tone mapping operator (SR-iTMO).


- **Experimental Results**：

&nbsp; &nbsp; &nbsp; &nbsp; As a quantitative metric, Fr ́echet inception distance (FID), Inception Score (IS), perceptual quality (PQ) and structural integrity (SI) are employed to evaluate the quality and diversity of the generated images

<div align=center>
<img src="https://github.com/VLISLAB/360-DL-Survey/blob/0b5649bbe1131424c944d0cad8bd3001d10a1846/Images/text2pano3.png" width="500" height="900">
</div>


 
- **Limitations (provided in the paper)**：

&nbsp; &nbsp; &nbsp; &nbsp; (1) **Text Bias.**. Since authors did not use any paired data for text-driven synthesis, the performance relies on CLIP model. Interestingly, authors observed that CLIP tends to be **biased on some word-image pairs** in our framework.

&nbsp; &nbsp; &nbsp; &nbsp; (2) **Uncommon Scenery**. Text2Light cannot synthesize scene-level contents that are uncommon in the dataset.
