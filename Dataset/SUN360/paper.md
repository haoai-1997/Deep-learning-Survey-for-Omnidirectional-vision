## Recognizing Scene Viewpoint using Panoramic Place Representation

- year: 2012

- dataset：  **( self-construct SUN360 dataset)**  The final dataset contains 80 categories and 67,583 panoramas, all of which have a resolution of 9104 × 4552 pixels and cover a full 360◦ × 180◦ visual angle using equirectangular projection
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SUN360dataset1.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SUN360datasetw.png)
- abstract: We introduce the problem of scene viewpoint recognition, the goal of which is to classify the type of place shown in a photo, and also recognize the observer’s viewpoint within that category of place
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SUN360abstract.png)

- Contributions:

The goal of this paper is to study the viewpoint recognition problem in scenes. We aim to design a model which, given a photo, can classify the place category to which it belongs (e.g., a theater), and predict the direction in which the observer is facing within that place (e.g., towards the stage).
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SUN360contribution.png)

- structure:

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SUN360structure.png)


- results：

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/SUN360result.png)


- analysis: We study a new problem of recognizing place category and viewpoint in scenes. We construct a new panorama dataset, and design a new algorithm for automatic panorama alignment. Since this is a first attempt at a new problem, we are simplifying the question by considering only viewpoint and ignoring the observer’s position within a place.
