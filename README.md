# CNN-Architectures
Some of the most powerful and famous Convolution Neural Network Architectures

# AlexNet — Architecture
Well that figure certainly looks scary. This is because the network was split into two halves, each trained simultaneously on two different GPUs. Let’s make this a little bit easy for us and bring a simpler version into the picture:



The architecture consists of 5 Convolutional Layers and 3 Fully Connected Layers. These 8 layers combined with two new concepts at 
that time — MaxPooling and ReLU activation gave their model an edge.
You can see the various layers and their configuration in the figure above. The layers are described in the table below:




ReLU activation is applied to the output of every Convolution and Fully Connected layer except the last softmax layer.
