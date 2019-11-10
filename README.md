# CNN-Architectures
Some of the most powerful and famous Convolution Neural Network Architectures

The main idea is to get familiar with state-of-the-art CNN architectures by actually creating them. 

This will build and improve our intuition and understanding about CNN’s and how to and when to use them.


# AlexNet — Architecture
Well that figure certainly looks scary. This is because the network was split into two halves, each trained simultaneously on two different GPUs. Let’s make this a little bit easy for us and bring a simpler version into the picture:


![1 5r9uLOsKYE6Tfq0qsGubdQ](https://user-images.githubusercontent.com/19469956/68547112-a6ea3000-0403-11ea-997a-e2d006a82712.jpeg)



The architecture consists of 5 Convolutional Layers and 3 Fully Connected Layers. These 8 layers combined with two new concepts at 
that time — MaxPooling and ReLU activation gave their model an edge.
You can see the various layers and their configuration in the figure above. The layers are described in the table below:


![2](https://user-images.githubusercontent.com/19469956/68547139-eca6f880-0403-11ea-97b1-6090823b9c30.jpeg)



ReLU activation is applied to the output of every Convolution and Fully Connected layer except the last softmax layer.




# LeNet-5 Architecture


LeNet-5, a 7 layer Convolutional Neural Network, was deployed in many banking systems to recognize hand-written numbers on cheques.


![3](https://user-images.githubusercontent.com/19469956/68547193-af8f3600-0404-11ea-980b-7503a18bc453.jpeg)





# Xception Net


![5](https://user-images.githubusercontent.com/19469956/68547317-0c3f2080-0406-11ea-9c37-0a32b5bffaba.png)




Xception Net is an improvisation of InceptionNet in terms of computational efficiency. Xception means Extreme Inception
Xception Net outperforms Inception Net v3.

The difference between Inception Net and Xception Net is that, in Inception Net normal convolutional operations are performed whereas 

in Xception Net, Depthwise Separable Convolutional operations are performed. Depthwise Separable Convolutions are different from normal convolutions in a way that, in normal Conv2D layer, for an input of (32, 32, 3) image we can use any number of filters in the Convlayer. Each of those filters will be operated over all three channels and the output is the sum of all corresponding values. 

But in Depthwise separable convolutions, each channel have only one kernel to do convolution. Hence, by performing Depthwise Separable Convolutions, we can reduce the computational complexity as every kernel is of two dimensional only and is convoluting only over one channel. In Keras, we can implement this by using DepthwiseConv2D layer.
