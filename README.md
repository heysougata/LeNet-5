# LeNet-5
LeNet-5 Total seven layer , does not comprise an input, each containing a trainable parameters; each layer has a plurality of the Map the Feature , a characteristic of each of the input FeatureMap extracted by means of a convolution filter, and then each FeatureMap There are multiple neurons.
# Architecture Details
* The first layer is the input layer with feature map size 32X32X1.

* Then we have the first convolution layer with 6 filters of size 5X5 and stride is 1. The activation function used at his layer is tanh. The output feature map is 28X28X6.

* Next, we have an average pooling layer with filter size 2X2 and stride 1. The resulting feature map is 14X14X6. Since the pooling layer doesn’t affect the number of channels.

* After this comes the second convolution layer with 16 filters of 5X5 and stride 1. Also, the activation function is tanh. Now the output size is 10X10X16.

* Again comes the other average pooling layer of 2X2 with stride 2. As a result, the size of the feature map reduced to 5X5X16.

* The final pooling layer has 120 filters of 5X5  with stride 1 and activation function tanh. Now the output size is 120.

* The next is a fully connected layer with 84 neurons that result in the output to 84 values and the activation function used here is again tanh.

* The last layer is the output layer with 10 neurons and  Softmax function. The Softmax gives the probability that a data point belongs to a particular class. The highest value is then predicted.

* This is the entire architecture of the Lenet-5 model. The number of trainable parameters of this architecture is around sixty thousand.

![arch](https://user-images.githubusercontent.com/120707085/225368061-b4d37b0c-4f35-433a-97ed-7fcfa98ffda6.jpg)

# Summary
* LeNet-5 is a very efficient convolutional neural network for handwritten character recognition.
* Convolutional neural networks can make good use of the structural information of images.
* The convolutional layer has fewer parameters, which is also determined by the main characteristics of the convolutional layer, that is, local connection and shared weights.
