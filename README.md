#Neural Image Caption Generator
## Model Overview

### Introduction

The model is a deep neural network that learns how to describe
the content of images.

### Architecture

The model is an example of an *encoder-decoder* neural network.
It works by first "encoding" an image into a fixed-length vector representation,
and then "decoding" the representation into a natural language description.

The image encoder is a deep convolutional neural network. This type of
network is widely used for image tasks and is currently state-of-the-art for
object recognition and detection.

The decoder is a long short-term memory (LSTM) network. This type of network is
commonly used for sequence modeling tasks such as language modeling and machine
translation. In the model, the LSTM network is trained as a
language model conditioned on the image encoding.

Words in the captions are represented with an embedding model. Each word in the
vocabulary is associated with a fixed-length vector representation that is
learned during training.

### Packages Used.

* **Bazel** ([instructions](http://bazel.io/docs/install.html)).
* **TensorFlow** ([instructions](https://www.tensorflow.org/versions/master/get_started/os_setup.html)).
* **NumPy** ([instructions](http://www.scipy.org/install.html)).
* **Natural Language Toolkit (NLTK)**:(http://www.nltk.org/data.html) 
Dataset:
MSCOCO
(http://mscoco.org/) 
