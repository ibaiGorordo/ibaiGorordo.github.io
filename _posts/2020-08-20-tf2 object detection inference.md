---
layout: post
title: tf2 object detection inference
date: 2020-08-20 10:45:51 +0000
last_modified_at: 2023-04-23 11:07:34 +0000
url: https://github.com/ibaiGorordo/tf2-object-detection-inference
image:
  path: https://github.com/ibaiGorordo/tf2-object-detection-inference/raw/master/doc/img/Inference%20Output%20Example.gif
  alt: TF2 Object Detection Inference
tags: [tensorflow2, object-detection, inference, webcam-capture, opencv, deep-learning, tensorflow]
categories: ["Repository", Python]
---

## [Open In Github](https://github.com/ibaiGorordo/tf2-object-detection-inference)

![TF2 Object Detection Inference](https://github.com/ibaiGorordo/tf2-object-detection-inference/raw/master/doc/img/Inference%20Output%20Example.gif)

# TF2.0 Object Detection Inference
Python program to perform object detection inference with Tensorflow 2.0.

# Installation
* Follow the steps as in: [https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/install.html](https://tensorflow-object-detection-api-tutorial.readthedocs.io/en/latest/install.html)

# Usage
* Modify the model name (**model_name**) with the desired model from the [Object Detection Model Zoo (TF2)](https://github.com/tensorflow/models/blob/master/research/object_detection/g3doc/tf2_detection_zoo.md). Note: The name should be the one in the link, for example, in the case of the *SSD MobileNet v2 320x320* model, **model_name** should be 'ssd_mobilenet_v2_fpnlite_320x320_coco17_tpu-8'.

* Modify the relative path to the labels folder (**PATH_TO_LABELS**). The current program works only if the Python program is in the same directory where the models directory is located.
