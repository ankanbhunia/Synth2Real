# Improving sementic segmentation performance using synthetic to realistic image generation using advarsarial doamin transfer method

![Alt text](Photos/syn.png)


## Pre-requisites

- python 2.7
- Tensorflow 
- OpenCV
- matplotlib
- jupyter notebook

The use of synthetic data in semantic segmentation task have already proven to be effective. But, direct use of synthetic data may degrade the results. Here, we employed a style transfer technique to convert the synthetic images to realistic images. For the synthetic dataset we choose ![GTA](https://download.visinf.tu-darmstadt.de/data/from_games/) game dataset. It has dense pixel-level semantic annotations for 25 thousand images synthesized by a photorealistic open-world computer game. We generate a realistic version of this dataset using GAN model. 
We choose FCN to check the effectiveness of ynthetic to realistic image generation. We feed this realistic version of the GTA dataset along with a very popular sementic segmentation dataset (![Cityscapes](https://www.cityscapes-dataset.com/)) to the FCN model. 

| Approch    | mIoU(%) | 
|:--------------- |:---------------:|
| Only Cityscapes|    34.15|  
|  Only GTA  |   25.16 | 
|  Cityscapes +  GTA | 35.13  |
|    Real GTA |   37.12   |  
| Cityscapes + Real GTA |   42.7   |  


