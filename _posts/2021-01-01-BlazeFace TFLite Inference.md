---
layout: post
title: BlazeFace TFLite Inference
date: 2021-01-01 01:31:58 
last_modified_at: 2022-11-17 11:38:13 
url: https://github.com/ibaiGorordo/BlazeFace-TFLite-Inference
image:
  path: https://github.com/ibaiGorordo/BlazeFace-TFLite-Inference/raw/main/doc/img/output.jpg
  alt: !BlazeFace detection tflite
tags: [blazeface, tensorflow2, python, facedetection, face-detection, tflite, tensorflow-lite]
categories: ["Repository", Python]
---
 Python scripts to detect faces using Python with the BlazeFace Tensorflow Lite models. Tested on Windows 10, Tensorflow 2.4.0 (Python 3.8).

![!BlazeFace detection tflite](https://github.com/ibaiGorordo/BlazeFace-TFLite-Inference/raw/main/doc/img/output.jpg)

# Requirements

 * **OpenCV**, **Numpy** and **tensorflow 2**. **pafy** and **youtube-dl** are required for youtube video inference. 
 
# Installation
```
conda create -n blazeFace python=3.8 -y
conda activate blazeFace
conda install numpy opencv tensorflow -y
pip install pafy youtube-dl

```

# Model types

 * **Front**: Input size 128 x 128, faster but lower accuracy.
 * **Back**: Input size 256 x 256, higher accuracy but slower.
 
# Examples

 * **Image inference**:
 
 ```
 python imageFaceDetection.py 
 ```
 
  * **Webcam inference**:
 
 ```
 python webcamFaceDetection.py
 ```
 
  * **Video inference**:
 
 ```
 python videoFaceDetection.py
 ```
 
 ![!BlazeFace detection tflite video](https://github.com/ibaiGorordo/BlazeFace-TFLite-Inference/raw/main/doc/img/video%20output.gif)

 
 
