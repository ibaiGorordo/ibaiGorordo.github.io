---
layout: post
title: Pytorch SAGENet Driver Attention Estimation
date: 2022-02-19 08:10:54 
last_modified_at: 2022-02-21 01:38:16 
url: https://github.com/ibaiGorordo/Pytorch-SAGENet-Driver-Attention-Estimation
image:
  path: https://github.com/ibaiGorordo/Pytorch-SAGENet-Driver-Attention-Estimation/raw/main/doc/img/output.jpg
  alt: SAGENet Driver Attention Estimation Pytorch
categories: ["Repository", Python]
---

## [Open In Github](https://github.com/ibaiGorordo/Pytorch-SAGENet-Driver-Attention-Estimation)[![Open In Github](https://icons-for-free.com/download-icon-part+1+github-1320568339880199515_0.svg)](https://github.com/ibaiGorordo/Pytorch-SAGENet-Driver-Attention-Estimation)

 Python scripts for performing driver attention estimation using the SAGENet model in Pytorch
 
![SAGENet Driver Attention Estimation Pytorch](https://github.com/ibaiGorordo/Pytorch-SAGENet-Driver-Attention-Estimation/raw/main/doc/img/output.jpg)
*Original image:[https://en.wikipedia.org/wiki/File:Axis_axis_crossing_the_road.JPG](https://en.wikipedia.org/wiki/File:Axis_axis_crossing_the_road.JPG)*

# Requirements

 * Check the **requirements.txt** file. 
 * For Pytorch, check the official website to install the version matching your machine: [https://pytorch.org/](https://pytorch.org/)
 * Additionally, **pafy** and **youtube-dl** are required for youtube video inference.
 
# Installation (Except Pytorch)
```
pip install -r requirements.txt
pip install pafy youtube_dl=>2021.12.17
```

# Pretrained model
Download the original model (https://drive.google.com/file/d/1GBCxIwAtuaC8EjMmQo4d9kVaGQzZaUZr/view?usp=sharing) and save it into the **[models](https://github.com/ibaiGorordo/Pytorch-SAGENet-Driver-Attention-Estimation/tree/main/models)** folder. 

# Original Repository
The [original repository](https://github.com/anwesanpal/SAGENet_demo) also contains code for estimating the driver's attention in Pytorch. This repository uses part of that code to make it easier to use the model in videos, images and webcamera.
 
# Examples

 * **Image inference**:
 
 ```
 python image_attention_estimation.py
 ```
 
  * **Video inference**:
 
 ```
 python video_attention_estimation.py
 ```
 
 * **Webcam inference**:
 
 ```
 python webcam_attention_estimation.py
 ```
 
# Inference video Example: [https://youtu.be/I-tZNb7tBBw](https://youtu.be/I-tZNb7tBBw)
 ![SAGENet Driver Attention Estimation Pytorch](https://github.com/ibaiGorordo/Pytorch-SAGENet-Driver-Attention-Estimation/raw/main/doc/img/sagenet-attention-heatmap.gif)

*Original video: [https://youtu.be/bUhFfunT2ds](https://youtu.be/bUhFfunT2ds)*

# References:
* SAGENet Demo example: [https://github.com/anwesanpal/SAGENet_demo](https://github.com/anwesanpal/SAGENet_demo)
* Original paper: [https://arxiv.org/abs/1911.10455](https://arxiv.org/abs/1911.10455)
 
