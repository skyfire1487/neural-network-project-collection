# Neural Network Project Collection

This repository contains three neural network and deep learning projects focused on model implementation, image classification, and object detection training. The topics cover neural network training from first principles, CNN-based image classification, and YOLOv8-based face detection.

本專案集合三個神經網路與深度學習實作主題，內容涵蓋從基礎原理實作神經網路、使用 CNN 進行影像分類，以及使用 YOLOv8 進行臉部偵測訓練。

## Projects

| Project | Topic | Main focus | Public materials |
| --- | --- | --- | --- |
| [Neural Network From Scratch](projects/neural-network-from-scratch/) | Handwritten digit classification | Forward pass, back propagation, weight updates, validation tracking | Notebook, architecture diagram, forward-pass diagram |
| [CNN Image Classification](projects/cnn-image-classification/) | CIFAR-style image classification | Convolution blocks, BatchNormalization, Dropout, Data Augmentation, training comparison | Notebook, model architecture, training curves |
| [YOLOv8 Face Detection Training](projects/yolov8-face-detection-training/) | Face detection model training | YOLOv8 training setup, validation metrics, prediction output inspection | Training config, result curves, confusion matrix, validation sample |

## Repository Notes

- The first project uses NumPy-based neural network logic and does not rely on deep learning libraries for back propagation.
- The second project uses TensorFlow/Keras to build and compare CNN image classification models.
- The third project uses Ultralytics YOLOv8 as the training framework and focuses on training configuration, validation metrics, and result interpretation.
- Dataset paths and training artifacts can be configured locally when rerunning the notebooks.

## Results Summary

- The from-scratch neural network records validation accuracy improving through training experiments, with the best recorded run reaching about 0.96 validation accuracy.
- The CNN image classification experiment records validation accuracy around 0.79 in the selected run, with additional comparisons for convolution depth, normalization, dropout, and augmentation.
- The YOLOv8 face detection selected run `yolov8x_e10+66` records final validation metrics around precision 0.871, recall 0.649, mAP50 0.743, and mAP50-95 0.427.

These numbers summarize the observed training records in this project. The focus is on the implementation process, model design choices, and experiment documentation.

## How to Read This Repository

Start with each topic folder's README. The notebooks preserve the main code structure and implementation flow for each experiment.

Each topic folder under `projects/` contains its own diagrams, result images, notebook, and configuration files where applicable.

## Suggested Environment

The projects were developed with Python notebooks. A modern environment can be prepared with:

```bash
pip install -r requirements.txt
```

The notebooks may require dataset paths to be adjusted before rerunning.
