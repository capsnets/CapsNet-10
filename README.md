# CapsNet (Code Added for MNIST, Cifer10 and Cat and Dog Datasets)
We want to implement the CapsNet model based on @XifengGo implementation: Here is a pipline of CapsNet, the neural network architecture using Capsules. 

| ![1*0NxktTeAhqNyRa411M3LXA.jpeg](https://cdn-images-1.medium.com/max/1600/1*0NxktTeAhqNyRa411M3LXA.jpeg) | 
|:--:| 
| *Source: Capsule Network paper: https://arxiv.org/abs/1710.09829*|


NIPS 2017 Paper:
* Dynamic Routing Between Capsules,
* by Sara Sabour, Nicholas Frosst, Geoffrey E. Hinton
* https://arxiv.org/abs/1710.09829

The 2011 paper:
* Transforming Autoencoders
* by Geoffrey E. Hinton, Alex Krizhevsky and Sida D. Wang
* https://goo.gl/ARSWM6

CapsNet implementations:
* Keras w/ TensorFlow backend: https://github.com/XifengGuo/CapsNet-...
* TensorFlow: https://github.com/naturomics/CapsNet...
* PyTorch: https://github.com/gram-ai/capsule-ne...

CapsNet Videos:
* What is wrong with convolutional neural network: https://www.youtube.com/watch?v=rTawFwUvnLE
* Understanding Hinton’s Capsule Networks. Part I: Intuition: https://medium.com/ai%C2%B3-theory-practice...
* Understanding Hinton’s Capsule Networks. Part II: How Capsules Work: https://medium.com/ai%C2%B3...

# Cifer10

| ![Cnn.PNG](https://github.com/sulaimanvesal/CapsNet/blob/master/images/Cnn.PNG) | 
|:--:| 
| *fchollet CNN: "It gets to 75% validation accuracy in 25 epochs, and 79% after 50 epochs.
(it's still underfitting at that point, though)." https://github.com/fchollet/keras/blob/master/examples/cifar10_cnn.py|

| ![Cifer10.png](https://github.com/sulaimanvesal/CapsNet/blob/master/images/Cifer10.png) | 
|:--:| 
| *CapsNet model implemented in keras with the same architecture in the paper: https://arxiv.org/abs/1710.09829|

We trained the CapsNet model through @XifengGo implementation in keras with slight changes, the hyperparameters set as following:

```batch_size =32
epochs = 300
lam_recon = 1.563
num_routing = 3
lr = 0.0001
Optimizer = Adam 
```

It can be seen that the model is still underfitting and there should be space for improvement in the classification.

| ![Cifer102.png](https://github.com/sulaimanvesal/CapsNet/blob/master/images/Cifer102.png) | 
|:--:|
| *Validation CapsNet and Validation loss for Cifer10 Dataset|
