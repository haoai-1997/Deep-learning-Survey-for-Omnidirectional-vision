## Cube Padding for Weakly-Supervised Saliency Prediction in 360◦Videos

- year: 2018

- dataset: Wild-360(Wild-360 contains 85 360◦video clips, totally about 55k frames.
60 clips within our dataset are for training and the rest 25 clips are for testing. 
All the clips are cleaned and trimmed from 45 raw videos obtained from YouTube.)

- abstract:
we propose a simple and effective Cube Padding (CP) technique as follows.
Firstly, we render the 360◦view on six faces of a cube using perspective projection.
Then, we concatenate all six faces while utilizing the connectivity between faces on the cube for image padding (i.e., Cube Padding) in convolution, pooling, convolutional LSTM layers

- structure

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Cube_Padding_system.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Cube_Padding.png)

- loss function

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Cube_padding_motion_loss.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Cude_Padding_loss_recons.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Cude_padding_smooth_loss.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Cude_Padding_total_loss.png)

- result

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/Cube_Padding_result.png)
