# Neural Network Project Collection

This repository collects three course projects from the 2023 fall semester course on artificial intelligence, neural networks, and deep learning. The materials were reorganized for portfolio review, with the original course submission labels, identifier-based filenames, local datasets, model weights, and third-party framework source files removed.

本專案整理自 2023 上學期「人工智慧、神經網路與深度學習」課程中的三個實作主題。整理後的版本以履歷展示為目標，保留方法、流程、結果圖與可讀程式碼，移除原始課程提交標籤、識別碼檔名、本機資料集、模型權重與第三方框架原始碼。

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

These numbers are included as course experiment records, not as benchmark claims. The focus of this repository is to show the implementation process, model design choices, and experiment documentation.

## How to Read This Repository

Start with each topic folder's README. The notebooks are included as cleaned portfolio copies: outputs and local path traces were removed, while the main code structure and implementation flow were preserved.

Each topic folder under `projects/` contains its own selected diagrams, result images, notebook, and configuration files where applicable. Local-only course materials remain on the original machine but are excluded from Git tracking.

## Suggested Environment

The original projects were developed with Python notebooks. A modern environment can be prepared with:

```bash
pip install -r requirements.txt
```

The notebooks may still require dataset paths to be adjusted before rerunning, because the raw course datasets are not included in this public repository.
