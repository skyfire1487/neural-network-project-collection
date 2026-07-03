# CNN Image Classification

## Overview

This project builds CNN image classification experiments with TensorFlow/Keras. The work focuses on model architecture choices and training behavior, including convolution depth, filter count, BatchNormalization, Dropout, Data Augmentation, learning rate settings, and validation metrics.

本專案使用 TensorFlow/Keras 進行影像分類模型訓練，重點是比較 CNN 架構設計與訓練調整方式。內容包含卷積層數量、filter 數量、BatchNormalization、Dropout、Data Augmentation 與 learning rate 設定。

## Method

- Load image data and labels into NumPy arrays.
- Split the dataset into training and validation subsets.
- Build CNN models with Conv2D, pooling layers, BatchNormalization, Dropout, and dense output layers.
- Compare training curves and validation accuracy across model settings.
- Use accuracy, precision, recall, and confusion-matrix concepts to interpret results.

## Materials

- Notebook: `train_cifar_cnn.ipynb`
- Model architecture: `model-architecture.png`
- Selected training curves: `training-curves-final.png`
- Ranking summary: `ranking-summary.png`

## Result Notes

The selected notebook records a validation accuracy around 0.79 in the final comparison. The result is presented as a course experiment record. It is useful for showing the effect of architecture and training-setting changes, not as a benchmark against current image-classification models.

## Limitations

- The image dataset and trained model checkpoint files are not included.
- Some original experiment checkpoints were excluded because they are large binary files.
- The notebook may require local dataset paths to be set before rerunning.
