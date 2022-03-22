## Zillow Indoor Dataset: Annotated Floor Plans With 360o Panoramas and 3D Room Layouts

- year: 2021

- dataset：  **( PanoContext dataset and Stanford-2D3D dataset, MatterportLayout test dataset)**  

- abstract: We present Zillow Indoor Dataset (ZInD): A large indoor dataset with 71,474 panoramas from 1,524 real unfurnished homes. ZInD provides annotations of 3D room layouts, 2D and 3D floor plans, panorama location in the floor plan, and locations of windows and doors.
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ZInDabstract.png)

- Contributions:

1) ZInD is the **(largest)** real dataset with layout annotations.
2) A unique property is the room layout data, which follows a real world distribution (cuboid, more general Manhattan, and non-Manhattan layouts) as opposed to the mostly cuboid or Manhattan layouts in current publicly available datasets.

- structure:
ZInD contains 1,524 homes, with a total of 71,474 panoramas, 21,596 room layouts, and 2,564 floor plans

![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ZInDstructure.png)
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ZInDdataset.png)


- results：
To demonstrate ZInD’s benefits, we benchmark with **(HorizonNet)** on room layout estimation from single panoramas and multi-view registration.
metrics: **(3D IoU, Corner Error, Pixel Error, 2D IoU, δ1, RMSE)**
![image](https://github.com/VLISLAB/360-DL-Survey/blob/main/Images/ZInDresult.png)


- analysis: The dataset reflects a realistic distribution of layout complexities that include a significant number that are noncuboid and non-Manhattan. While the featured homes are unfurnished, we have shown that mapping the (sparse) panoramas to floor plans remains a research challenge.
