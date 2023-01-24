---
layout: post
title: PyTorch High Res Stereo Depth Estimation
date: 2021-09-09 15:11:18 
last_modified_at: 2023-01-15 20:04:55 
url: https://github.com/ibaiGorordo/PyTorch-High-Res-Stereo-Depth-Estimation
image:
  path: https://github.com/ibaiGorordo/PyTorch-High-Res-Stereo-Depth-Estimation/raw/main/docs/img/out.jpg
  alt: High res stereo depth estimation Pytorch
tags: [pytorch, python, stereo-vision, stereo-matching, stereo-depth-estimation, depth-estimation]
categories: ["Repository", Python]
---
Python scripts form performing stereo depth estimation using the high res stereo model in PyTorch.

![High res stereo depth estimation Pytorch](https://github.com/ibaiGorordo/PyTorch-High-Res-Stereo-Depth-Estimation/raw/main/docs/img/out.jpg)
*Stereo depth estimation on the cones images from the Middlebury dataset (https://vision.middlebury.edu/stereo/data/scenes2003/)*

# Requirements

 * **OpenCV**, **imread-from-url** and **pytorch**. Also, **pafy** and **youtube-dl** are required for youtube video inference. 
 
# Installation
```
pip install -r requirements.txt
pip install pafy youtube-dl
```

**Pytorch:** Check the [Pytorch website](https://pytorch.org/) to find the best method to install Pytorch in your computer.

# Pretrained model
Download the pretrained model from the [original repository](https://github.com/gengshan-y/high-res-stereo) and save it into the **[models](https://github.com/ibaiGorordo/PyTorch-High-Res-Stereo-Depth-Estimation/tree/main/models)** folder. 
 
# Examples

 * **Image inference**:
 
 ```
 python imageDepthEstimation.py 
 ```
 
  * **Video inference**:
 
 ```
 python videoDepthEstimation.py
 ```
 
 * **DrivingStereo dataset inference**:
 
 ```
 python drivingStereoTest.py
 ```
 
# [Inference video Example](https://youtu.be/kG_c32pFRR8) 
 ![High res stereo depth estimation Pytorch](https://github.com/ibaiGorordo/PyTorch-High-Res-Stereo-Depth-Estimation/raw/main/docs/img/highresStereoDepthEstimation.gif)

# References:
* High Res Stereo model: [https://github.com/gengshan-y/high-res-stereo](https://github.com/gengshan-y/high-res-stereo)
* DrivingStereo dataset: [https://drivingstereo-dataset.github.io/](https://drivingstereo-dataset.github.io/)
* Original paper: [https://arxiv.org/abs/1912.06704](https://arxiv.org/abs/1912.06704)
 
