In this lab, you will create and train a computer vision model to recognize different items of clothing using TensorFlow on Google Cloud Compute Engine.

# Introduction to TensorFlow
TensorFlow provides a computational framework for building ML models. TensorFlow provides a variety of different toolkits that allow you to construct models at your preferred level of abstraction. In this lab you'll use tf.keras, a high-level API to build and train a neural network for classifying images in TensorFlow.

### Neural networks
A neural network is a model inspired from the brain. It is composed of layers, at least one of which is [hidden](https://developers.google.com/machine-learning/glossary/#hidden_layer), that consists of simple connected units or neurons followed by nonlinearities.

A node in a neural network typically takes multiple input values and generates one output value. The neuron applies an [activation function](https://developers.google.com/machine-learning/glossary/#activation_function) (nonlinear transformation) to a weighted sum of input values to calculate the output value.

For more information about neural networks, see [Neural Networks: Structure](https://developers.google.com/machine-learning/crash-course/introduction-to-neural-networks/anatomy).

## About Data 

You will train a neural network to classify images of clothing from a dataset called [Fashion MNIST](https://github.com/zalandoresearch/fashion-mnist).
  
This dataset contains 70,000 items of clothing belonging to 10 different categories of clothing. The images show individual articles of clothing at low resolution (28 by 28 pixels), as seen here:

![img data](https://cdn.qwiklabs.com/YPBhHbZOxbtfyeaVsai9H2bgpNqt9JJtO9ZhsYTcbas%3D)

In this lab, 60,000 images will be used to train the network and 10,000 images will be used to evaluate how accurately the network learned to classify images.

The Fashion MNIST data is available in [tensorflow datasets(tfds)](https://www.tensorflow.org/datasets/catalog/fashion_mnist).


## Objectives
In this lab, you will learn how to:

- Set up the development environment in the IDE
- Design, compile, train and evaluate your model
- Save and load models
- Write your own callbacks to customize behavior during training
- Complete a series of exercises to guide you through experimenting with the different layers of the network
