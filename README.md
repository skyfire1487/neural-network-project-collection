# Neural Network Project Collection

This repository contains three neural network and deep learning projects completed during the 2023 fall semester. The topics cover neural network training from first principles, CNN-based image classification, and YOLOv8-based face detection training.

本專案包含 2023 上學期「人工智慧、神經網路與深度學習」課程中的三個實作主題，內容涵蓋從基礎原理實作神經網路、使用 CNN 進行影像分類，以及使用 YOLOv8 進行臉部偵測訓練。

## Projects

| Project | Topic | Main focus | Public materials |
| --- | --- | --- | --- |
| [Neural Network From Scratch](projects/neural-network-from-scratch/) | Handwritten digit classification | Forward pass, back propagation, weight updates, validation tracking | Notebook, architecture diagram, forward-pass diagram |
| [CNN Image Classification](projects/cnn-image-classification/) | CIFAR-style image classification | Convolution blocks, BatchNormalization, Dropout, Data Augmentation, training comparison | Notebook, model architecture, training curves |
| [YOLOv8 Face Detection Training](projects/yolov8-face-detection-training/) | Face detection model training | YOLOv8 training setup, validation metrics, prediction output inspection | Training config, result curves, confusion matrix, validation sample |

## Repository Notes

- The first project uses NumPy-based neural network logic and does not rely on deep learning libraries for back propagation.
- The second project uses TensorFlow/Keras to build and compare CNN image classification models.
- The third project uses Ultralytics YOLOv8 as the training framework. This repository documents the training process and selected results; it does not include the Ultralytics source tree or trained `.pt` weights.
- Datasets and model checkpoints are intentionally excluded because they are large and are not required for reviewing the implementation approach.

## Results Summary

- The from-scratch neural network records validation accuracy improving through training experiments, with the strongest original experiment logs reaching about 0.96 validation accuracy.
- The CNN image classification experiment records validation accuracy around 0.79 in the selected run, with additional comparisons for convolution depth, normalization, dropout, and augmentation.
- The YOLOv8 face detection selected run `yolov8x_e10+66` records final validation metrics around precision 0.871, recall 0.649, mAP50 0.743, and mAP50-95 0.427.

These numbers summarize the observed training records in this project. The focus is on the implementation process, model design choices, and experiment documentation.

## How to Read This Repository

Start with each topic folder's README. The notebooks preserve the main code structure and implementation flow for each experiment.

Each topic folder under `projects/` contains its own diagrams, result images, notebook, and configuration files where applicable.

## Suggested Environment

The original projects were developed with Python notebooks. A modern environment can be prepared with:

```bash
pip install -r requirements.txt
```

The notebooks may require dataset paths to be adjusted before rerunning.
