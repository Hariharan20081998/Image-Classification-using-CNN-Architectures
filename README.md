# Image Classification

## Datasets
### CALTECH 101
This Dataset contains pictures of objects belonging to 101 categories. About 40 to 800 images are present per category. Most categories have about 50 images. Collected in September 2003 by Fei-Fei Li, Marco Andreetto, and Marc 'Aurelio Ranzato.  The size of each image is roughly 300 x 200 pixels.

### COIL100
COIL-100 was collected by the Center for Research on Intelligent Systems at the Department of Computer Science, Columbia University. The database contains color images of 100 objects. The objects were placed on a motorized turntable against a black background and images were taken at pose internals of 5 degrees. This dataset was used in a real-time 100 object recognition system whereby a system sensor could identify the object and display its angular pose. There are 7,200 images of 100 objects. Each object was turned on a turnable through 360 degrees to vary object pose with respect to a fixed color camera. Images of the objects were taken at pose intervals of 5 degrees. This corresponds to 72 poses per object. There images were then size normalized. Objects have a wide variety of complex geometric and reflectance characteristics.

### Wang
This dataset contains 1000 images in 10 categories. Every 100 image belongs to a category.

## Architectures
### VGGNet
VGG stands for Visual Geometric Group. It takes a 224x224x3 image as input. VGG Net consists of architectures ranging from VGG11 to Vgg22. The Convolutions layers use a 3x3 filter and also use 1x1 filters for linear transformation with the stride of 1. It uses ReLu transformation function.

#### VGG16
VGG 16 consists of 16 weighted layers consisting of 13 Convolutional Layers and 3 Dense Layers (Configuration D)

#### VGG19
VGG 19 consists of 19 weighted layers consisting of 16 Convolutional Layers and 3 Dense Layers (Configuration E)

![alt text](https://github.com/niranjana98/Image-Classification/blob/main/VGGNet.png)
Figure: Different VGGNet Architectures

### Inception
The main idea behind the Inception Architecture is to effectively detect and classify images which have large variations insize of the region of interest. Since deep networks have a problem of overfitting and are computationally complex, it is more efficient to make a wider network with different convolutional nets with different filter sizes such as 3x3, 5x5 at the same level. And the outputs from each level is concatenated. There are 4 versions of Inception. 

#### Inception V3
Inception V3 consists of inception blocks which contains 4 braches which process the inputs: a 1x1 CONV layer, a pooling layer followed by a 1x1 layer, a 1x1 layer and a 3x3 layer and finally a 1x1 layer followed by 2 3x3 layers (which is equivalent to 5x5 layer). Since such architectures have the problem of "Vanishing Gradients", the technique of auxillary loss is used, in which output is obtained from 2 inception modules and loss is computed. The total loss function is a weighted sum of the auxiliary loss and the real loss. In such Auxillary classifiers, Batch Normalisation is used. Inception V3 uses a RMSPropOptimiser.

![alt text](https://github.com/niranjana98/Image-Classification/blob/main/Inception%20Module.png)
Figure: Representation of a Inception Module


## References
1. http://www.vision.caltech.edu/Image_Datasets/Caltech101/
2. http://www1.cs.columbia.edu/CAVE/software/softlib/coil-100.php
3. http://wang.ist.psu.edu/docs/related/
4. https://arxiv.org/abs/1409.1556
5. https://arxiv.org/pdf/1512.00567v3.pdf

