# Image Classification

## Datasets
### CALTECH 101
This Dataset contains pictures of objects belonging to 101 categories. About 40 to 800 images are present per category. Most categories have about 50 images. Collected in September 2003 by Fei-Fei Li, Marco Andreetto, and Marc 'Aurelio Ranzato.  The size of each image is roughly 300 x 200 pixels.

### COIL100
COIL-100 was collected by the Center for Research on Intelligent Systems at the Department of Computer Science, Columbia University. The database contains color images of 100 objects. The objects were placed on a motorized turntable against a black background and images were taken at pose internals of 5 degrees. This dataset was used in a real-time 100 object recognition system whereby a system sensor could identify the object and display its angular pose. There are 7,200 images of 100 objects. Each object was turned on a turnable through 360 degrees to vary object pose with respect to a fixed color camera. Images of the objects were taken at pose intervals of 5 degrees. This corresponds to 72 poses per object. There images were then size normalized. Objects have a wide variety of complex geometric and reflectance characteristics.

### Wang
This dataset contains 1000 images in 10 categories. Every 100 image belongs to a category.

## Architectures
## VGGNet
VGG stands for Visual Geometric Group. It takes a 224x224x3 image as input. VGG Net consists of architectures ranging from VGG11 to Vgg22. The Convolutions layers use a 3x3 filter and also use 1x1 filters for linear transformation with the stride of 1. It uses ReLu transformation function.

## VGG16
VGG 16 consists of 16 weighted layers consisting of 13 Convolutional Layers and 3 Dense Layers (Configuration D)

# VGG19
VGG 16 consists of 19 weighted layers consisting of 16 Convolutional Layers and 3 Dense Layers (Configuration E)

![alt text](https://github.com/niranjana98/Image-Classification/blob/main/VGGNet.png)

## References
1. http://www.vision.caltech.edu/Image_Datasets/Caltech101/
2. http://www1.cs.columbia.edu/CAVE/software/softlib/coil-100.php
3. http://wang.ist.psu.edu/docs/related/
4. https://arxiv.org/abs/1409.1556

