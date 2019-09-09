# [CNN](https://github.com/tfzoo/CNN) 
## [简介](https://github.com/tfzoo/CNN/wiki) 

[CNN = Convolutional Neural Networks](https://en.wikipedia.org/wiki/Convolutional_neural_network) . A convolutional neural network consists of an input and an output layer, as well as multiple hidden layers. The hidden layers of a CNN typically consist of convolutional layers, RELU layer i.e. activation function, pooling layers, fully connected layers and normalization layers.


卷积(convolution) 相关知识点：卷积核、滤波器、通道

输入图像： n×n
滤波器： f×f
paddig(填充)： p
stride(步长): s

滤波器需要四个参数确定：宽度×高度×通道数×过滤器个数，每个滤波器实际上是卷积核的集合，通道数与上一层图像输入的通道数相同，个数与本层输出图像的通道数相同，滤波器的卷积核各自产生一个对应通道的输出，最后整个滤波器产生一个总的输出通道。偏置的作用是对每个输出滤波器增加偏置项以便产生最终输出通道。

padding（填充）操作在卷积操作之前先在图像边缘进行像素填充，像素值可以是0也可以是图像边缘像素，填充宽度为p

Stride 的想法是改变卷积核的移动步长跳过一些像素。Stride 是 1 表示卷积核滑过每一个相距是 1 的像素，是最基本的单步滑动，作为标准卷积模式。Stride 是 2 表示卷积核的移动步长是 2，跳过相邻像素，图像缩小为原来的 1/2。Stride 是 3 表示卷积核的移动步长是 3，跳过 2 个相邻像素，图像缩小为原来的 1/3。越来越多的新网络结构，比如 ResNet，已经抛弃了池化层采用 Stride 方法对图像进行缩小。

###  [天府动物园 tfzoo：tensorflow models zoo](http://www.tfzoo.com)
####   qitas@qitas.cn
[![sites](tfzoo/tfzoo.png)](http://www.tfzoo.com)