---
layout: post
title: ONNX YOLOv10 Object Detection
date: 2024-08-26 01:43:20 +0000
last_modified_at: 2024-08-26 04:15:50 +0000
url: https://github.com/ibaiGorordo/ONNX-YOLOv10-Object-Detection
image:
  path: https://github.com/user-attachments/assets/a926d7d7-7ee5-474d-b90f-310ef874f0cb
  alt: ONNX YOLOv10 Object Detection
tags: [computer-vision, object-detection, onnx, onnxruntime, opencv, python, yolo, yolov10]
categories: ["Repository", Python]
---

## [Open In Github](https://github.com/ibaiGorordo/ONNX-YOLOv10-Object-Detection)

 Python scripts performing object detection using the YOLOv10 model in ONNX.
 
![!ONNX YOLOv10 Object Detection](https://github.com/user-attachments/assets/a926d7d7-7ee5-474d-b90f-310ef874f0cb)

> [!CAUTION]
> I skipped adding the pad to the input image when resizing, which might affect the accuracy of the model if the input image has a different aspect ratio compared to the input size of the model. Always try to get an input size with a ratio close to the input images you will use.

## Requirements

 * Check the **requirements.txt** file.
 * For ONNX, if you have a NVIDIA GPU, then install the **onnxruntime-gpu**, otherwise use the **onnxruntime** library.

## Installation [![PyPI](https://img.shields.io/pypi/v/yolov10-onnx?color=2BAF2B)](https://pypi.org/project/yolov10-onnx/)

```bash
pip install yolov10-onnx
```
Or, clone this repository:
```bash
git clone https://github.com/ibaiGorordo/ONNX-YOLOv10-Object-Detection.git
cd ONNX-YOLOv10-Object-Detection
pip install -r requirements.txt
```
### ONNX Runtime
For Nvidia GPU computers:
`pip install onnxruntime-gpu`

Otherwise:
`pip install onnxruntime`

## ONNX model
- If the model file is not found in the models directory, it will be downloaded automatically from the [Official Repo](https://github.com/THU-MIG/yolov10/releases/tag/v1.1).
- **Available models**: yolov10n.onnx, yolov10s.onnx, yolov10m.onnx, yolov10b.onnx, yolov10l.onnx, yolov10x.onnx

## Original YOLOv10 model
The original YOLOv10 model can be found in this repository: [https://github.com/THU-MIG/yolov10](https://github.com/THU-MIG/yolov10)
- The License of the models is AGPL-3.0 license: [https://github.com/THU-MIG/yolov10/blob/main/LICENSE](https://github.com/THU-MIG/yolov10/blob/main/LICENSE)

## Examples

 * **Image inference**:
 ```
 python image_object_detection.py
 ```

 * **Webcam inference**:
 ```
 python webcam_object_detection.py
 ```

 * **Video inference**: [https://youtu.be/hz9PYZF4ax4](https://youtu.be/hz9PYZF4ax4)
 ```
 python video_object_detection.py
 ```
![!yolov10_object_detection](https://github.com/user-attachments/assets/08872b1c-2009-4f8d-97a5-7b88f13ec887)


## References:
* YOLOv10 model: [https://github.com/THU-MIG/yolov10](https://github.com/THU-MIG/yolov10)
