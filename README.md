# Improving sementic segmentation performance using synthetic to realistic image generation using advarsarial domain transfer method

![PIC](Photos/syn.png)


## Pre-requisites

- python 2.7
- Tensorflow 
- OpenCV
- matplotlib
- jupyter notebook

We choose FCN to check the effectiveness of ynthetic to realistic image generation. We feed this realistic version of the GTA dataset along with a very popular sementic segmentation dataset([Cityscapes](https://www.cityscapes-dataset.com/)) to the FCN model. 

| Approach    | mIoU(%) | 
|:--------------- |:---------------:|
| Only Cityscapes|    34.15|  
|  Only GTA  |   25.16 | 
|  Cityscapes +  GTA | 35.13  |
|    Real GTA |   37.12   |  
| Cityscapes + Real GTA |   42.7   |  


## References

- [UNIT: UNsupervised Image-to-image Translation Networks](https://github.com/mingyuliutw/UNIT)
- [FCN8s Implementation](https://github.com/pierluigiferrari/fcn8s_tensorflow)
- [Converted version of GTA dataset](https://drive.google.com/open?id=1WRyH9buNUMvfuBXw9gH35XpY7-bf9CZR)


