# DNLD-Project3-Generate-TV-Scripts

This is my submission to the Udacity Deep Learning Nanodegree Projec 3, this is an example RNN to generate TV scripts from pre-labeled data.

## Backgound

Recurant Neural Networks are differnet from standard neural networks as they have "memory" cells allowing them to remember a context

The data set provided by Udacity is a subset of data from the below kaggle competiton, this repo contains two main ipython notebooks

### dlnd_tv_script_generation

This is the origional RNN as required to meet the DLND course - it's a standrd RNN (single layer) using Tensorflow trained on a GPU instance in AWS and achived a Final Traing Loss of 0.061 after 10,000 Epochs and a dropout out layer of 0.8

### dlnd_tv_script_generation-extra

This is the same basic network as above but with a few additions, as the network was still showing (albeit small) a ongoing reduction in training loss I upped the epochs to double. I also included Tensboard outputs showing the embeddings and what the graph looks like (visually).

I also downloaded the larger data set from the origional kaggle competition (~10mb) and trained the network on this (TODO post updated network stats)

## Recurant Neural Networks

RNN's work well where we need to remember previous words in order to predict which word comes next


* In order for RNN's to be used with text data steps need to be taken to preprocess;
* Convert word to Int and convert Int to word
* Tokenize Punctuation


Tokenize Punctuation

## Links

[Origional Kaggle competition data](https://www.kaggle.com/wcukierski/the-simpsons-by-the-data)
[Explination on RNN's](http://colah.github.io/posts/2015-08-Understanding-LSTMs/)