# TadGAN: Time Series Anomaly Detection Using Generative Adversarial Networks

This is a Python3 / [Tensorflow](https://www.tensorflow.org/) implementation 
of [TadGAN](https://arxiv.org/abs/2009.07769) paper.

## Data:

The model has been trained on `Exhange 2 - CPC Results` signal from [NAB real ad exhange](https://github.com/numenta/NAB/tree/master/data/realAdExchange) dataset. The anomaly labels for the signal can be found in the [labels folder](https://github.com/numenta/NAB/tree/master/labels).

## Architecture:

The model implements an encoder and decoder as generator and two critics as discriminators as described in the paper. The loss function is wasserstein loss with gradient penalty.

## Pretrained Model:

The trained model is saved in the `Model` directory. The model has to be retrained for other datasets.