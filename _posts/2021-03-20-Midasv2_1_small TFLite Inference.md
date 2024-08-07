---
layout: post
title: Midasv2_1_small TFLite Inference
date: 2021-03-20 12:27:35 +0000
last_modified_at: 2024-06-02 17:30:56 +0000
url: https://github.com/ibaiGorordo/Midasv2_1_small-TFLite-Inference
image:
  path: https://github.com/ibaiGorordo/Midasv2_1_small-TFLite-Inference/raw/main/doc/img/output.jpg
  alt: Midas v2.1 small TFLite Inference
tags: [tflite, tensorflow, monocular-depth-estimation, deeplearning, python, midasv2]
categories: ["Repository", Python]
---

## [Open In Github](https://github.com/ibaiGorordo/Midasv2_1_small-TFLite-Inference)

 Python scripts to perform monocular depth estimation using Python with the Midas v2.1 small Tensorflow Lite model. Tested on Windows 10, Tensorflow 2.4.0 (Python 3.8).

![!Midas v2.1 small TFLite Inference](https://github.com/ibaiGorordo/Midasv2_1_small-TFLite-Inference/raw/main/doc/img/output.jpg)

# Requirements

 * **OpenCV**, **Numpy** and **tflite (or tensorflow)**. **pafy** and **youtube-dl** are required for youtube video inference. 
 
# Installation
```
pip install numpy opencv-python tflite tensorflow
pip install pafy youtube-dl
```

# Midas v2.1 small ([link](https://tfhub.dev/intel/lite-model/midas/v2_1_small/1/lite/1))

 * **Input**: RGB image of size 256 x 256 pixels.
 * **Output**: Inverse relative depth map with 256 x256 pixels.
 * **Inference speed**: - 30 FPS on Iphone 11 NPU and 22 FPS on OnePlus8 GPU (Snapdragon 865).
 
# Examples

 * **Image inference**:
 
 ```
 python imageDepthEstimation.py 
 ```
 
  * **Webcam inference**:
 
 ```
 python webcamDepthEstimation.py
 ```
 
  * **Video inference**:
 
 ```
 python videoDepthEstimation.py
 ```
 
 # [Inference video Example](https://youtu.be/e161_lZps9c)
 ![!Midas v2.1 small TFLite Inference on video](https://github.com/ibaiGorordo/Midasv2_1_small-TFLite-Inference/raw/main/doc/img/Midasv2_1_small-TFLite-InferenceVideo.gif)
 
 Original video: https://youtu.be/TGadVbd-C-E (by Nagasaki Biopark)
 
 
