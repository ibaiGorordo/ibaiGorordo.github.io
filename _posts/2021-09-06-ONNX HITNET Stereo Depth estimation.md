---
layout: post
title: ONNX HITNET Stereo Depth estimation
date: 2021-09-06 11:53:53 
last_modified_at: 2022-11-08 01:36:23 
url: https://github.com/ibaiGorordo/ONNX-HITNET-Stereo-Depth-estimation
image:
  path: https://github.com/ibaiGorordo/ONNX-HITNET-Stereo-Depth-estimation/raw/main/doc/img/out.jpg
  alt: Hitnet stereo depth estimation ONNX
tags: [onnx, deep-learning, depth-estimation, stereo-vision, stereo-matching, stereo-depth-estimation, python, onnxruntime]
categories: ["Repository", Python]
---
Python scripts form performing stereo depth estimation using the HITNET model in ONNX.

![Hitnet stereo depth estimation ONNX](https://github.com/ibaiGorordo/ONNX-HITNET-Stereo-Depth-estimation/raw/main/doc/img/out.jpg)
*Stereo depth estimation on the cones images from the Middlebury dataset (https://vision.middlebury.edu/stereo/data/scenes2003/)*

# Requirements

 * **OpenCV**, **imread-from-url**, **onnx** and **onnxruntime**. Also, **pafy** and **youtube-dl** are required for youtube video inference. The depthai library is also necessary in the case of the OAK-D boards (https://docs.luxonis.com/projects/api/en/latest/install/)
 
# Installation
```
pip install -r requirements.txt
pip install pafy youtube-dl
```

# ONNX model
The original models were converted to different formats (including .onnx) by [PINTO0309](https://github.com/PINTO0309), download the models from [his repository](https://github.com/PINTO0309/PINTO_model_zoo/tree/main/142_HITNET) and save them into the **[models](https://github.com/ibaiGorordo/ONNX-HITNET-Stereo-Depth-estimation/tree/main/models)** folder. 

# Original Tensorflow model
The Tensorflow pretrained model was taken from the [original repository](https://github.com/google-research/google-research/tree/master/hitnet).
 
# Examples

 * **Depthai OAK-D series inference on the host**:
 
 ```
 python depthai_host_depth_estimation.py
 ```

 * **Image inference**:
 
 ```
 python image_depth_estimation.py 
 ```
 
  * **Video inference**:
 
 ```
 python video_depth_estimation.py
 ```
 
 * **DrivingStereo dataset inference**:
 
 ```
 python driving_stereo_test.py
 ```
  

# Pytorch inference
For performing the inference in Tensorflow, check my other repository **[HITNET Stereo Depth estimation](https://github.com/ibaiGorordo/HITNET-Stereo-Depth-estimation)**.

# TFLite inference
For performing the inference in TFLite, check my other repository **[TFLite HITNET Stereo Depth estimation](https://github.com/ibaiGorordo/TFLite-HITNET-Stereo-depth-estimation)**.

# [Inference video Example](https://youtu.be/BRQ_oaCRj3M) 
 ![Hitnet stereo depth estimation ONNX](https://github.com/ibaiGorordo/ONNX-HITNET-Stereo-Depth-estimation/raw/main/doc/img/onnxHitnetDepthEstimation.gif)

# References:
* Hitnet model: [https://github.com/google-research/google-research/tree/master/hitnet](https://github.com/google-research/google-research/tree/master/hitnet)
* PINTO0309's model zoo: [https://github.com/PINTO0309/PINTO_model_zoo](https://github.com/PINTO0309/PINTO_model_zoo)
* PINTO0309's model conversion tool: [https://github.com/PINTO0309/openvino2tensorflow](https://github.com/PINTO0309/openvino2tensorflow)
* DrivingStereo dataset: [https://drivingstereo-dataset.github.io/](https://drivingstereo-dataset.github.io/)
* Original paper: [https://arxiv.org/abs/2007.12140](https://arxiv.org/abs/2007.12140)
* Depthai Python library: [https://github.com/luxonis/depthai-python](https://github.com/luxonis/depthai-python)
 

