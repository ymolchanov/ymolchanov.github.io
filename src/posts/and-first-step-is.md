---
title: And here is the Kaggle's Deep Learning Course 0.1.3
description: Here I will write about my experience of Deep Learning first impression.
date: "2021-02-07"
tags: []
---

## What is the Deep Learning?

It is the field inside Machine Learning. Which mostly connected with neural network method.

## Why is this so important?

Quote:

> Some of the most impressive advances in artificial intelligence in recent years have been in the field of deep learning.

## What are Learning Rate and Batch size?

You probably saw that smaller batch sizes gave noisier weight updates and loss curves. This is because each batch is a small sample of data and smaller samples tend to give noisier estimates. Smaller batches can have an "averaging" effect though which can be beneficial.

Smaller learning rates make the updates smaller and the training takes longer to converge. Large learning rates can speed up training, but don't "settle in" to a minimum as well. When the learning rate is too large, the training can fail completely. (Try setting the learning rate to a large value like 0.99 to see this.)

## Underfitting or overfitting?

![](/images/hokey_stick.png)
Here we see the "hokey stick" plot.  
The gap between these curves is quite small and the validation loss never increases, so it's **more likely that the network is underfitting than overfitting**. It would be worth experimenting with more capacity to see if that's the case.

## Data preparation

With neural networks, it's generally a good idea to put all of your data on a common scale.  
Before we put data in Neural Network we need to do some actions around a data set. One of this actions is **put data to common scale**.

## Questions:

Why we need a bias in our neurons?

## New words:

**regression** - machine learning problem that we solving (operate with continuous data)

**classification** - machine learngin problem (operating with discrete data)

**dense layer** - most simple neural network layer, we work with it in [Lesson 2](https://www.kaggle.com/ymolchanov/exercise-deep-neural-networks/edit).  
A Dense layer feeds all outputs from the previous layer to all its neurons, each neuron providing one output to the next layer. It's the **most basic layer** in neural networks.  
In general, they (dense layers) have the same formulas as the _linear layers_ `wx+b`, but the end result is passed through a non-linear function called Activation function.  
Dense layers can be reduced back to linear layers if we use a linear activation!  
[About Dense layer in simple words](https://medium.com/datathings/dense-layers-explained-in-a-simple-way-62fe1db0ed75)  
[About Linear layer](https://medium.com/datathings/linear-layers-explained-in-a-simple-way-2319a9c2d1aa)

**TPU** - [Tensor Processing Unit](https://en.wikipedia.org/wiki/Tensor_Processing_Unit)

**activation functions** - activation function is simply some function we apply to each of a layer's outputs (its activations). It gives us more power, without it we can't move out of the world of lines and planes.

**rectifier function** - one of the activation function ( `max(0, x)` )

**rectified linear unit or ReLU** - is the neuron with rectifier function as activation function

**loss function** - function that measures the disparity between the the target's true value and the value the model predicts.

**optimizer** - The optimizer is an algorithm that adjusts the weights to minimize the loss

signal  
noise
**Dropout** - is an idea of layer transformation. We drop some neurons to remove model's overfitting.
batch normalization

## Map:

[First lesson of Kaggle's Deep Learning Course](https://www.kaggle.com/ryanholbrook/a-single-neuron)  
[First excercise](https://www.kaggle.com/ymolchanov/exercise-a-single-neuron/edit)  
[Pandas DataFrame head method](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.head.html#pandas.DataFrame.head)  
[Keras Dense Layer doc](https://www.tensorflow.org/api_docs/python/tf/keras/layers/Dense)  
[Keras Sequential doc](https://www.tensorflow.org/api_docs/python/tf/keras/Sequential)  
[Second lesson](https://www.kaggle.com/ryanholbrook/deep-neural-networks)  
[Second excercise](https://www.kaggle.com/ymolchanov/exercise-deep-neural-networks/edit)  
[Lesson 3: Stochastic Gradient Descent](https://www.kaggle.com/ryanholbrook/stochastic-gradient-descent)  
[Stochastic gradient descent](https://www.kaggle.com/ymolchanov/exercise-stochastic-gradient-descent/edit)  
[model.compile](https://www.tensorflow.org/api_docs/python/tf/keras/Model#compile)  
[model.fit](https://www.tensorflow.org/api_docs/python/tf/keras/Model#fit)  
[Lesson 4: overfitting and underfitting](https://www.kaggle.com/ryanholbrook/overfitting-and-underfitting)
[Excercise for Lesson 4: here I found good examples of data preparation](https://www.kaggle.com/ymolchanov/exercise-overfitting-and-underfitting/edit)  
[pandas.DataFrame.dropna](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.dropna.html)  
[keras.callbacks.EarlyStopping](https://www.tensorflow.org/api_docs/python/tf/keras/callbacks/EarlyStopping)  
[Lesson 5: Dropout and Batch Normalization](https://www.kaggle.com/ryanholbrook/dropout-and-batch-normalization)
