# YOLOv8 Face Detection Training

## Overview

This project documents a YOLOv8 face detection training experiment. The focus is on configuring training, observing validation behavior, and reviewing detection output. The project uses Ultralytics YOLOv8 as the framework, so the original contribution is the training setup, experiment process, and result interpretation rather than the YOLOv8 framework implementation itself.

本專案整理 YOLOv8 臉部偵測訓練流程，重點是訓練設定、驗證曲線、混淆矩陣與預測結果檢查。此專案使用 Ultralytics YOLOv8 作為訓練框架，因此公開內容以訓練流程與結果整理為主，不把 YOLOv8 框架原始碼視為自己的實作成果。

## Method

- Use YOLOv8 detection mode for a single class: `face`.
- Train with image size 640 and batch size 4.
- Continue training from an earlier run for the selected `yolov8x_e10+66` experiment.
- Review precision, recall, mAP50, mAP50-95, F1 curve, PR curve, confusion matrix, and prediction samples.

## Materials

- Training config: `training-args.yaml`
- Training curves: `training-results.png`
- Confusion matrix: `confusion-matrix.png`
- F1 curve: `f1-curve.png`
- Precision-recall curve: `precision-recall-curve.png`
- Validation prediction sample: `validation-predictions-sample.jpg`

## Selected Run

The selected public run is `yolov8x_e10+66`.

| Setting | Value |
| --- | --- |
| Task | Detection |
| Class | face |
| Image size | 640 |
| Batch size | 4 |
| Epochs in selected continuation run | 66 |
| Final precision | about 0.871 |
| Final recall | about 0.649 |
| Final mAP50 | about 0.743 |
| Final mAP50-95 | about 0.427 |

## Limitations

- The dataset is not included.
- The trained `.pt` weights are not included.
- The Ultralytics source tree is not included because it is a third-party framework and is not needed for portfolio review.
