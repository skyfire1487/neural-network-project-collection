# Neural Network From Scratch

## Overview

This project implements a small feedforward neural network for handwritten digit classification. The main purpose is to show the forward pass, back propagation, gradient calculation, weight update process, and validation tracking without using a Python deep learning framework for the neural network training logic.

本專案以手寫數字分類為主題，重點是自行實作神經網路的 forward pass、back propagation、權重更新與驗證流程。此部分的核心訓練邏輯以 NumPy 實作，不依靠 TensorFlow、PyTorch 或 Keras 這類深度學習框架。

## Method

- Input images are flattened into 784-dimensional vectors.
- Pixel values are normalized before training.
- The network uses hidden-layer weights and output-layer weights with sigmoid activation.
- The backward pass computes output-layer and hidden-layer error terms, then updates weights with gradient-based correction.
- Validation accuracy and mean squared error are tracked during training.

## Materials

- Notebook: `train_digit_classifier_from_scratch.ipynb`
- Architecture diagram: `network-architecture.png`
- Forward-pass diagram: `forward-pass.svg`

## Result Notes

The experiment records show validation accuracy improving over training. The strongest recorded run reached about 0.96 validation accuracy.

## Limitations

- The notebook may need dataset path updates before rerunning.
- The goal is to document the learning process of neural network training, not to provide a production digit-recognition system.
