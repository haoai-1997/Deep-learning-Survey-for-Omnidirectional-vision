## Rethinking 360° Image Visual Attention Modelling with Unsupervised Learning
- year: ICCV 2021
- dataset: Salient360!, VR-EyeTracking and Sitzman.

- abstract:  We extend recent advances in contrastive learning to learn latent representations that are sufficiently invariant to be highly effective for spherical
saliency prediction as a downstream task. We argue that omni-directional images are particularly suited to such an approach due to the geometry of the data domain. To ver-ify this hypothesis, we design an unsupervised framework
that effectively maximizes the mutual information between the different views from both the equator and the poles. We show that the decoder is able to learn good quality saliency
distributions from the encoder embeddings.

- contributions: 
(1) We propose a framework to extend the idea of contrastive/self-supervised learning to a new data domain, specifically 360° images.
(2) The proposed method performs on par with fully supervised methods.
(3) Our approach addresses one of the key challenges encountered when predicting 360° saliency
by excluding any use of CMP.
(4) A single subsequent stream of learning on the equirectangular projection images significantly reduces the computational cost.

- Framework:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/saliency%20prediction/Rethinking%20360_%20framework.png)

- results:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/saliency%20prediction/Rethinking%20360_result.png)
