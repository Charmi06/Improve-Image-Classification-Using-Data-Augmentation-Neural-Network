## Improve Image Classification Using Data Augmentation & Neural Network
## Keras Vgg 16

### Pre-requisites
* Python 2.7
* Keras

### Models
M0   | M DA | Vgg 16
------------- | ------------- | ------
The shapes of 3D feature maps are passed between ayers and their connections. Conv1 and Conv2 have the same space size of 32x32x32, while the pooling layer has the space size of 16x16x32 after dimensionality reduction. The flatten layer is used to adjust the feature maps to the dense layer. The output layer has ten neurons with one for each target | This model pattern is three stacks of two convolutional layers followed by three max-pooling layer. The 3 filter numbers applied in the stacking convolutional layers slide from 32,64, 128 separately. The flatten layer is used to adjust the feature maps to the dense layer with the probability output for ten classes. We also added Batch Normalization layers. | There are two stacks of two convolutional layers and three stacks of three convolutional layers followed by one pooling layer after every stack along with batch normalization before activation  layer. The filter numbers slide from 64 to 128, 256 and 512 separately in the stacked convolutional layers.
![ 2 layer convolutional neural network](/Images/2layer.PNG) |![ 6 layer convolutional neural network](/Images/6layer.PNG) | ![ 13 layer convolutional neural network](/Images/13layer.PNG) 


## File & Code Details
File Name | Description
----------|------------
M0.ipynb | Model with 2 layer
M DA-0.ipynb | Model with 6 Convolutional Layer
M DA-1.ipynb | Model with 6 Conv Layer and Data Augmentation
M DA-2.ipynb | Model with 6 Convolutional Layer and Data Augmentation + Gaussian Noise
M DA-3.ipynb | Model with 6 Convolutional Layer and Extreme Data Augmentation
VGG16-0.ipynb | Model with 13 Convolutional Layer
VGG16-1.ipynb | Model with 13 Conv Layer and Data Augmentation
VGG16-2.ipynb | Model with 6 Convolutional Layer and Data Augmentation + Gaussian Noise
