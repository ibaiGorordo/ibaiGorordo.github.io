---
layout: post
title: ONNX MobileStereoNet
date: 2021-11-27 15:40:38 
last_modified_at: 2022-11-29 09:41:53 
url: https://github.com/ibaiGorordo/ONNX-MobileStereoNet
image:
  path: https://github.com/ibaiGorordo/ONNX-MobileStereoNet/raw/main/doc/img/out.jpg
  alt: MobileStereoNet depth estimation ONNX
---
Python scripts for performing stereo depth estimation using the MobileStereoNet model in ONNX

![MobileStereoNet depth estimation ONNX](https://github.com/ibaiGorordo/ONNX-MobileStereoNet/raw/main/doc/img/out.jpg)
*Stereo depth estimation on the cones images from the Middlebury dataset (https://vision.middlebury.edu/stereo/data/scenes2003/)*

# Requirements

 * Check the **requirements.txt** file. Additionally, **pafy** and **youtube-dl** are required for youtube video inference.
 * DrivingStereo dataset, **ONLY** for the `driving_sereo_test.py`script. Link: [https://drivingstereo-dataset.github.io/](https://drivingstereo-dataset.github.io/)
 
# Installation
```
pip install -r requirements.txt
pip install pafy youtube-dl
```

# ONNX model
Download the ONNX model from [Google Drive](https://drive.google.com/file/d/1Dkyrg5Fu554gqxfclkHC6zJBCYrdzOO0/view?usp=sharing) and save it into the [models folder](https://github.com/ibaiGorordo/ONNX-MobileStereoNet/tree/main/models).

# Original Pytorch model
The Pytorch pretrained model was taken from the [original repository](https://github.com/cogsys-tuebingen/mobilestereonet).
 
# Examples

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
 python driving_sereo_test.py
 ```
 
# [Inference video Example](https://youtu.be/AueQdkU70io) 
 ![MobileStereoNet depth estimation ONNX](https://github.com/ibaiGorordo/ONNX-MobileStereoNet/raw/main/doc/img/video_stereo_depth.gif)

# References:
* MobileStereoNet model: [https://github.com/cogsys-tuebingen/mobilestereonet](https://github.com/cogsys-tuebingen/mobilestereonet)
* PINTO0309's model zoo: [https://github.com/PINTO0309/PINTO_model_zoo](https://github.com/PINTO0309/PINTO_model_zoo)
* PINTO0309's model conversion tool: [https://github.com/PINTO0309/openvino2tensorflow](https://github.com/PINTO0309/openvino2tensorflow)
* DrivingStereo dataset: [https://drivingstereo-dataset.github.io/](https://drivingstereo-dataset.github.io/)
* Original paper: [https://arxiv.org/pdf/2108.09770.pdf](https://arxiv.org/pdf/2108.09770.pdf)
 
