# Mars Crater Detection and Segmentation with MaskRCNN

![](/gitex.PNG)


Detection of craters on planetary surface is very crucial for the better understanding of planet topography. It is also important for the selection of landing sites of various lander mission, path planning for rover missions. This project is about application of deep learning method for detection and semantic segmentation of craters in an image. Model trained using transfer learning on pretrained MaskRCNN model. Overall project can be devided into four parts as follow:-    


1. [Data Preparation](https://github.com/sandipanrakshit34/Mars-Crater-Detection-and-Segmentation-with-MaskRCNN)

2. [Data Inspection](inspect_crater_data.ipynb)

3. [Training](train.ipynb)

4. [Testing](inspect_crater_model.ipynb)


Mars                       |  Moon
:-------------------------:|:-------------------------:
[![](mars.jpg)]() |                                           [![](moon.jpg)]()

#### Data Collection and Training-Validation data preparation 

Image data collected from the [sources](Dataset-Sources) and annotated with [VIA](http://www.robots.ox.ac.uk/~vgg/software/via/via.html) tool to get json file. Which looks like:- 

![](https://github.com/mymultiverse/Mask_RCNN/blob/master/samples/crater/viaex.PNG)

The Labeled dataset can be downloaded from [dropbox](https://www.dropbox.com/scl/fo/zm7m1cua71erhhf5rh9d9/AEfjYBAom80h84CaM33lKC8?rlkey=y6klkk1zrfptffhkx0yefm2b3&st=uwmps9fm&dl=0).
Dataset directory looks like:-
```bash

├── train
│   ├── img1.jpg
|   ├── :
|   ├── imgn.jpg
│   └── via_region_data.json
└── val
    ├── img.jpg
    ├── :
    ├── imgq.jpg
    └── via_region_data.json
```
train and val folder should be inside datasets directory(which is place at root directory)

Trained model mask_rcnn_crater_new.h5 [dropbox](https://www.dropbox.com/scl/fi/0hk0m92ru6rthsgiqnluy/mask_rcnn_crater_new.h5?rlkey=z2i4ijotx5prjcv6kf4ld5l57&st=askv6lf5&dl=0)

## Author

- [@sandipanrakshit34](https://github.com/sandipanrakshit34)

##

Dataset Sources:

1. [High Resolution Imaging Science Experiment](https://www.uahirise.org/)
2. [Mars Science](https://mars.nasa.gov/multimedia/images/)
3. [ASU](https://jmars.mars.asu.edu/)
4. [USGS](https://webgis2.wr.usgs.gov/Mars_Global_GIS/)

