---
layout: post
title: ONNX YOLOv6 Object Detection
date: 2022-06-25 11:32:25 
last_modified_at: 2022-12-13 13:23:38 
url: https://github.com/ibaiGorordo/ONNX-YOLOv6-Object-Detection
image:
  path: https://github.com/ibaiGorordo/ONNX-YOLOv6-Object-Detection/raw/main/doc/img/detected_objects.jpg
  alt:  ONNX YOLOv6 Object Detection
categories: ["Repository", Python]
---
 Python scripts performing object detection using the YOLOv6 model in ONNX.

![! ONNX YOLOv6 Object Detection](https://github.com/ibaiGorordo/ONNX-YOLOv6-Object-Detection/raw/main/doc/img/detected_objects.jpg)
*Original image: [https://commons.wikimedia.org/wiki/File:Motorcyclists_lane_splitting_in_Bangkok,_Thailand.jpg](https://commons.wikimedia.org/wiki/File:Motorcyclists_lane_splitting_in_Bangkok,_Thailand.jpg)*

# Important
- About the YOLOv6 name: [https://github.com/meituan/YOLOv6/blob/main/docs/About_naming_yolov6.md](https://github.com/meituan/YOLOv6/blob/main/docs/About_naming_yolov6.md)
- The input images are directly resized to match the input size of the model. I skipped adding the pad to the input image, it might affect the accuracy of the model if the input image has a different aspect ratio compared to the input size of the model. Always try to get an input size with a ratio close to the input images you will use.
- The original YOLOv6 repository is still in development, so things might not work in the future.

# Requirements

 * Check the **requirements.txt** file. 
 * For ONNX, if you have a NVIDIA GPU, then install the **onnxruntime-gpu**, otherwise use the **onnxruntime** library.
 
# Installation
```
git clone https://github.com/ibaiGorordo/ONNX-YOLOv6-Object-Detection.git
cd ONNX-YOLOv6-Object-Detection
pip install -r requirements.txt
```
### ONNX Runtime
For Nvidia GPU computers:
`pip install onnxruntime-gpu`

Otherwise:
`pip install onnxruntime`

# ONNX model 
~~The original model was converted to ONNX using the following Colab notebook from the original repository, run the notebook and save the download model into the [models  folder](https://github.com/ibaiGorordo/ONNX-YOLOv6-Object-Detection/tree/main/models):~~
- ~~**Convert YOLOv6 ONNX for Inference** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1pke1ffMeI2dXkIAbzp6IHWdQ0u8S6I0n?usp=sharing)~~

You can find the ONNX models in the Assets section of the official repository Releases (e.g. [Release 2.1](https://github.com/meituan/YOLOv6/releases/tag/0.2.1)). Download the ONNX file and save the download model into the [models  folder](https://github.com/ibaiGorordo/ONNX-YOLOv6-Object-Detection/tree/main/models):
- Additionally, if you want to convert the model to ONNX yourself, you can follow the instructions in: [https://github.com/meituan/YOLOv6/tree/main/deploy/ONNX](https://github.com/meituan/YOLOv6/tree/main/deploy/ONNX)
- The License of the models is GPL-3.0 license: [License](https://github.com/meituan/YOLOv6/blob/main/LICENSE)

# Pytorch model
The original Pytorch model can be found in this repository: [YOLOv6 Repository](https://github.com/meituan/YOLOv6)
 
# Examples

 * **Image inference**:
 ```
 python image_object_detection.py
 ```
 
 * **Webcam inference**:
 ```
 python webcam_object_detection.py
 ```

 * **Video inference**: [https://youtu.be/yYo0XQp97vo](https://youtu.be/yYo0XQp97vo)
 ```
 python video_object_detection.py
 ```
 ![!YOLOv6 detection video](https://github.com/ibaiGorordo/ONNX-YOLOv6-Object-Detection/raw/main/doc/img/yolov6s_video.gif)
 
  *Original video: [https://youtu.be/yXEb0fWLJIY](https://youtu.be/yXEb0fWLJIY)*

 * **Comparison with YOLOv5**: [https://youtu.be/yd1DhOf8mW4](https://youtu.be/yd1DhOf8mW4)
 ```
 python comparison_with_yolov5.py
 ```
Convert YOLOv5 model to ONNX: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1V-F3erKkPun-vNn28BoOc6ENKmfo8kDh?usp=sharing)

# References:
* YOLOv6 model: [https://github.com/meituan/YOLOv6](https://github.com/meituan/YOLOv6)
* YOLOv5 model: [https://github.com/ultralytics/yolov5](https://github.com/ultralytics/yolov5)
