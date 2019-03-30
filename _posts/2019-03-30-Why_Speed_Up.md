---
layout: post
title: 神经网络为什么要加速
tag: 模型加速
---

### 为什么要加速？
神经网络为什么要加速，以下是各个相关文章的说法。

###### MobileNets

__In many real world applications__ such as robotics, self-driving car and augmented reality, __the recognition tasks __need to be carried out in a timely fashion on __a computationally limited platform__.



###### SqueezeNet

A CNN architecture with __fewer parameters__ has several advantages:

* More efficient distributed training.
* Less overhead when exporting new models to clients.
* Feasible FPGA and embedded deployment.



###### ShuffleNet

We introduce an extremely computation-efficient CNN architecture named ShuffleNet, __which is designed specially for mobile devices with very limited computing power__.



###### Inception

__With the ongoing traction of mobile and embedded computing__, __the efficiency of our algorithms__-especially their power and memory use - __gains importance__.



######DenseNet: Implementing Efficient ConvNet Descriptor Pyramids
__Extending__ a current state of the art __CNN-based classifier into an object detector__ using a naive dense sliding window set of region proposals would be __prohibitively slow__.



###### Exploiting Linear Structure Within Convolutional Networks for Efficient Evaluation

大模型部署时会存在以下问题：

* 移动平台资源（CPU speed, memory and battery life）受限，难以部署
* 互联网规模的部署会耗费服务器大量的资源（electrical and cooling costs）



###### Speeding-up convolutional neural networks using fine-tuned CP-decomposition
CNN在低端设备上的应用及单独训练的计算代价是个问题，尤其在一些实时应用中



###### Sparse convolutional neural networks

神经网络的结构中存在大量的冗余



###### Efficient and accurate approximations of nonlinear convolutional networks

高昂的测试代价使得模型在实际中不实用

* 云服务器每秒需处理上千次请求
* 便携设备大多仅有CPU或低端的GPU
* 某些识别任务即便在高端GPU上仍然很耗时



###### Accelerating very deep convolutional networks for classification and detection

Real-world systems may suffer from the low speed of these networks.

* 云服务器每秒需处理上千次的请求
* 便携设备不支持慢的模型
* 某些识别任务需处理高分辨率的图片



###### Coordinating Filters for Faster Deep Neural Networks

The high computation intensity of DNNs makes it challenging to deploy these models on __resource-limited systems__.