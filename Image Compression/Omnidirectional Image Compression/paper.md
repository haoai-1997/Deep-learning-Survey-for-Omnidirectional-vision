## Pseudocylindrical Convolutions for LearnedOmnidirectional Image Compression

- year: 2021

- dataset: ERP images from Flickr that carry Creative Commons licenses and save them losslessly.

- abstract: In this paper, we make one of the first attempts to learn deep neural networksfor omnidirectional image compression.
We thenpropose pseudocylindrical convolutions for 360° image compression. 
To demonstrate the feasibility of our idea, we implement an end-to-end 360° image compression system, consisting of the learned pseudocylindrical representation, an analysis transform, a non-uniform quantizer, a synthesis transform, and an entropy model.

- contribution:
(1) We propose a computationally tractable greedy algorithm to determine the (sub)-optimal parameter configuration in terms of the rate-distortion performance, estimated by a novel proxy objective.
Interestingly, we find that the optimized representation does not correspond to pseudocylindrical projections with the equal-area property(e.g., sinusoidal projection). 
(2) We propose pseudocylindrical convolutions that work seamlessly with the parametric pseudocylindrical representation for 360° image compression.
(3) We build an end-to-end 360° image compression system, which is composed of the optimized pseudocylindrical representation, an analysis transform, a non-uniform quantizer, a synthesis transform, and a context-based entropy model.


- structure:
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/spherical_representation.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Pseudocylindrical_Convolutions_framework.png)




