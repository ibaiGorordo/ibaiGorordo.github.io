---
layout: post
title: ONNX msg_chn_wacv20 depth completion
date: 2021-10-03 10:13:27 +0000
last_modified_at: 2024-04-15 22:34:16 +0000
url: https://github.com/ibaiGorordo/ONNX-msg_chn_wacv20-depth-completion
image:
  path: https://github.com/ibaiGorordo/ONNX-msg_chn_wacv20-depth-completion/raw/main/doc/img/out.png
  alt: ONNX msg_chn_wacv20 depth completion
tags: [onnx, onnxruntime, depth-estimation, depth-completion, python, depth]
categories: ["Repository", Python]
---

## [Open In Github](https://github.com/ibaiGorordo/ONNX-msg_chn_wacv20-depth-completion)

Python script for performing depth completion from sparse depth and rgb images using the msg_chn_wacv20 model in ONNX. The example takes a synthetic depth map, it reduces the density (variable) of the depthmap and passes it to the depth completion map to densify the depth map.

![ONNX msg_chn_wacv20 depth completion](https://github.com/ibaiGorordo/ONNX-msg_chn_wacv20-depth-completion/raw/main/doc/img/out.png)

# Requirements

 * **OpenCV**, **onnx** and **onnxruntime**. Also, **unrealcv** is only required if you want to generate new data using unrealcv.

# UnrealCV synthethic data generation
The input images and depth are generated using the UnrealCV library (https://unrealcv.org/), you can find more information about how to generate this data in this [other repository for Unreal Synthetic depth generation](https://github.com/ibaiGorordo/UnrealCV-stereo-depth-generation).

# Installation
```
pip install -r requirements.txt
```

# ONNX model
The original models were converted to different formats (including .onnx) by [PINTO0309](https://github.com/PINTO0309), download the models from [his repository](https://github.com/PINTO0309/PINTO_model_zoo/tree/main/160_msg_chn_wacv20) and save them into the **[models](https://github.com/ibaiGorordo/ONNX-msg_chn_wacv20-depth-completion/tree/main/models)** folder.

# Original Pytorch model
The Pytorch pretrained model was taken from the [original repository](https://github.com/anglixjtu/msg_chn_wacv20).

# Examples

  * **Video inference (UnrealCV synthetic data)**:

 ```
 python video_depth_estimation.py
 ```

# Inference video Example
![ONNX msg_chn_wacv20 depth completion](https://github.com/ibaiGorordo/ONNX-msg_chn_wacv20-depth-completion/raw/main/doc/img/msg_chn_wacv20-depth-completion.gif)

# References:
* msg_chn_wacv20 model: [https://github.com/anglixjtu/msg_chn_wacv20](https://github.com/anglixjtu/msg_chn_wacv20)
* PINTO0309's model zoo: [https://github.com/PINTO0309/PINTO_model_zoo](https://github.com/PINTO0309/PINTO_model_zoo)
* PINTO0309's model conversion tool: [https://github.com/PINTO0309/openvino2tensorflow](https://github.com/PINTO0309/openvino2tensorflow)

* Original paper:
[https://openaccess.thecvf.com/content_WACV_2020/papers/Li_A_Multi-Scale_Guided_Cascade_Hourglass_Network_for_Depth_Completion_WACV_2020_paper.pdf](https://openaccess.thecvf.com/content_WACV_2020/papers/Li_A_Multi-Scale_Guided_Cascade_Hourglass_Network_for_Depth_Completion_WACV_2020_paper.pdf)


