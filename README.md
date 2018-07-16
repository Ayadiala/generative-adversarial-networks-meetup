# Generative adversarial network with tensorflow 

we will see how we can train a network that does not depend on the mean squared error or any related loss function — instead, it will learn all by itself what a real image should look like. The architecture we will get to know is called Deep Convolutional Generative Adversarial Network (DCGAN). I got inspired to complete this project by an awesome article written by Rowel Atienza in late March, where he taught us how to apply the same technique in keras. For being able to draw comparisons to the last VAE-based model, we will firstly see how to implement a DCGAN which is able to draw MNIST characters. Afterwards, we will apply our knowledge in an even cooler project — with only a few minor tweaks, our network will learn how to draw (semi-)realistic human faces!

TensorFlow / TensorLayer implementation of Deep Convolutional Generative Adversarial Networks which is a stabilize Generative Adversarial Networks.

## Deep Convolutional Generative Adversarial Networks

Like the VAE, the DCGAN is an architecture for learning to generate new content. And just like the VAE, a DCGAN consists of two parts. In this case, these are:

* The discriminator, which learns how to distinguish fake from real objects of the type we’d like to create
* The generator, which creates new content and tries to fool the discriminator

The basic idea is that both network parts compete with each other. When the discriminator becomes better, the generator needs to become better too, otherwise it can’t fool the discriminator any longer. Similarly, when the generator becomes better, the discriminator has to become better also, else it will lose the ability to distinguish fake from real content.

TensorFlow / TensorLayer implementation of [Deep Convolutional Generative Adversarial Networks](http://arxiv.org/abs/1511.06434) which is a stabilize Generative Adversarial Networks.

![alt tag](https://user-images.githubusercontent.com/10371630/33244947-c882506e-d2f8-11e7-89e4-611fdc7dacd9.png)


Prerequisites
========================
* Python 2.7 or Python 3.3+
* TensorFlow==1.0+
* TensorLayer==1.4+

Usage
========================
Choose between mnist or celib dataset in the `main` function.
