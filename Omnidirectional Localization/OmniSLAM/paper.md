## OmniSLAM: Omnidirectional Localization and Dense Mapping for Wide-baseline Multi-camera Systems

- year: 2020

- dataset：  **(real data: IT/BT and Wangsimni; the synthetic datasets: Sunny, Cloudy, Sunset, and Garage)**  

- abstract:  In this paper, we present an omnidirectional localization and dense mapping system for a wide-baseline multiview stereo setup with ultra-wide field-of-view (FOV) fisheye cameras, which has a 360◦ coverage of stereo observations of the environment.

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/OmniSLAMabstract.png)


- Contributions:
1) We propose light-weighted and improved networks for the omnidirectional depth estimation from the widebaseline stereo setup. The accuracy, the number of parameters, and the running time of our network have become better than the previous versions, which makes our system more practical
2) We build a robust omnidirectional visual SLAM system by integrating the depth map into ROVO and addinga loop closing module. The accuracy of the estimatedtrajectory is improved than the previous versions inboth challenging indoor and large scale outdoor environments. 
3) We present an integrated omnidirectional localization and dense mapping system, and the extensive experiments on synthetic, and real-world indoor and outdoor environments show that our proposed system generateswell reconstructed 3D dense maps for various scenes.

- structure:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/OmniSLAMstructure.png)

- results：
metrics: **( mean absolute error, )**

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/OmniSLAMresult.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/OmniSLAMresult1.png)


- analysis: In this paper, we propose an integrated omnidirectional localization and dense mapping system for a wide-baseline multi-camera rig with wide FOV fisheye lenses.


