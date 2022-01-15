# Ship-Size-Feature-Estimation-in-SAR-data-using-Inertia-Tensors
The repository consists code for finding size of ships detected in synthetic aperture radar data using inertia tensors. 

Recently, ship detection and classification using synthetic aperture radar (SAR) data have gained lot of attention from researches. To detect and classify ships, it is essential to calculate ship features such as length, width, mass, and area. Provided ipynb file helps us to calculate 13 different features from ship chips collected from Sentinel-1 SAR data.

The features are: 
1. Length
2. Width
3. Significance
4. Significance mean
5. Total Pixels
6. Mass
7. Area
8. 7 Hu momemnts

To understand meaning of different features, please refer - [link](https://doi.org/10.1016/j.asr.2021.08.042)

Note that calculation of minimum bounding box around ship is done using inertia tensors. For detailed methodology, please refer - [link](https://doi.org/10.3390/proceedings2020097)

To demonstrate proposed method, 50 sample images of ship chips are taken from OpenSARShip dataset in VH-VV polarization. Refer - [link](https://opensar.sjtu.edu.cn/). The pixel spacing of images are 10 * 10. Hence, output values are considered in same unit. To get actual values such as length and width of ships, multiply (code) output values by 10. 

#### Sample results

##### Original ship chip image: 

![alt text](Images/Original.PNG?raw=true "Title")

##### Binary ship chip image: 

![alt text](Images/Binary.PNG?raw=true "Title")

##### Minimum Bounding Rectangle: 

![alt text](Images/MBR.PNG?raw=true "Title")


Please cite below research paper while using above material. 

Hrishikesh Relekar, Palanisamy Shanmugam,
Transfer learning based ship classification in Sentinel-1 images incorporating scale variant features,
Advances in Space Research,
Volume 68, Issue 11,
2021,
Pages 4594-4615,
ISSN 0273-1177,
https://doi.org/10.1016/j.asr.2021.08.042.





