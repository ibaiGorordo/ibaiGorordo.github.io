---
layout: post
title: ONNX PackNet SfM
date: 2022-02-13 07:26:28 +0000
last_modified_at: 2024-02-22 06:31:18 +0000
url: https://github.com/ibaiGorordo/ONNX-PackNet-SfM
image:
  path: https://github.com/ibaiGorordo/ONNX-PackNet-SfM/raw/main/doc/img/out.jpg
  alt: GLPDepth monocular depth estimation ONNX
tags: [python, opencv, depth-estimation, monocular-depth-estimation, packnet-sfm, onnx, onnxruntime]
categories: ["Repository", Python]
---

## [Open In Github](https://github.com/ibaiGorordo/ONNX-PackNet-SfM)

Python scripts for performing monocular depth estimation using the PackNet-SfM model in ONNX

![GLPDepth monocular depth estimation ONNX](https://github.com/ibaiGorordo/ONNX-PackNet-SfM/raw/main/doc/img/out.jpg)
*Original image:[https://commons.wikimedia.org/wiki/File:HydeStreetSF.JPG](https://commons.wikimedia.org/wiki/File:HydeStreetSF.JPG)*

# Requirements

 * Check the **requirements.txt** file. Additionally, **pafy** and **youtube-dl** are required for youtube video inference.

# Installation
```
pip install -r requirements.txt
pip install pafy youtube_dl>=2021.12.17
```

# ONNX model
The original models were converted to different formats (including .onnx) by [PINTO0309](https://github.com/PINTO0309), download the models from [his repository](https://github.com/PINTO0309/PINTO_model_zoo/tree/main/147_PackNet-SfM) and save them into the **[models](https://github.com/ibaiGorordo/ONNX-PackNet-SfM/tree/main/models)** folder. 

# Original Pytorch model
The Pytorch pretrained models were taken from the [original repository](https://github.com/TRI-ML/packnet-sfm).
 
# Examples

 * **Image inference**:
 
 ```
 python image_depth_estimation.py 
 ```
 
  * **Video inference**:
 
 ```
 python video_depth_estimation.py
 ```
 
 * **Webcam inference**:
 
 ```
 python webcam_depth_estimation.py
 ```
 
# [Inference video Example](https://youtu.be/YNqGT5jgbeQ) 
 ![GLPDepth monocular depth estimation ONNX](https://github.com/ibaiGorordo/ONNX-PackNet-SfM/raw/main/doc/img/packnet_sfm_test.gif)

*Original video: [https://www.youtube.com/watch?v=z_9GiRz12-4](https://www.youtube.com/watch?v=z_9GiRz12-4)*

# References:
* PackNet-SfM model: [https://github.com/TRI-ML/packnet-sfm](https://github.com/TRI-ML/packnet-sfm)
* PINTO0309's model zoo: [https://github.com/PINTO0309/PINTO_model_zoo](https://github.com/PINTO0309/PINTO_model_zoo)
* PINTO0309's model conversion tool: [https://github.com/PINTO0309/openvino2tensorflow](https://github.com/PINTO0309/openvino2tensorflow)
* Original papers: [https://arxiv.org/abs/1905.02693](https://arxiv.org/abs/1905.02693) and [https://arxiv.org/abs/2008.06630](https://arxiv.org/abs/2008.06630)
