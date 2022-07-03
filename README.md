# Image Classification
This repo is about image classification using feature extraction with VGG16 pretrained model
## Transfer Learning
Transfer learning is the reuse of a pre-trained model on a new problem. It's currently very popular in deep learning because it can train deep neural networks with comparatively little data.

![image](https://user-images.githubusercontent.com/63583210/177046093-8d73bd6c-7939-4090-8ef2-3ec193cdfd78.png)

## VGG16
VGG16 is a convolutional neural network trained on a subset of the ImageNet dataset, a collection of over 14 million images belonging to 22,000 categories. K. Simonyan and A. Zisserman proposed this model in the 2014 paper, Very Deep Convolutional Networks for Large-Scale Image Recognition (https://arxiv.org/abs/1409.1556).

![image](https://user-images.githubusercontent.com/63583210/177045413-1ec915e9-8b43-49b9-b129-85180cc40b32.png)
VGG16 arcitecture

## steps
1. Downloaded the dataset for image classification. Here, I have used Multi-class weather Dataset. (https://data.mendeley.com/datasets/4drtyfjtfy/1)
   <br/>Convert into the folder structure as shown in dataset folder.
2. Preparing the dataset to train and test.
<br/>i) Convert the images into shape of 224x224x3 (as input of VGG16)
<br/>ii) Have unique label for each classes. Such as Sunrise - 0, Shine - 1, Rain - 2, Cloudy -3.
<br/>iii) Split the datapoint into train (90%) and test (10%) datapoints.
3. Download the pretrained model VGG16 imagenet and use it for feature extraction.
4. Training the multilayer preceptron and using it after 7x7x512 max pooling layer.
5. Train the model with an adam optimizer.
6. Evaluate the model with test datapoints.
