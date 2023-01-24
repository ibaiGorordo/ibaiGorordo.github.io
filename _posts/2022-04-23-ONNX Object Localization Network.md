---
layout: post
title: ONNX Object Localization Network
date: 2022-04-23 14:00:54 
last_modified_at: 2022-10-14 03:56:29 
url: https://github.com/ibaiGorordo/ONNX-Object-Localization-Network
image:
  path: https://github.com/ibaiGorordo/ONNX-Object-Localization-Network/raw/main/doc/img/output.jpg
  alt: !Object-Localization-Network
tags: [class-agnostic-detection, computer-vision, object-detection, onnx, onnxruntime, opencv, python, object-localization]
categories: ["Repository", Python]
---
 Python scripts performing class agnostic object localization using the Object Localization Network model in ONNX.

![!Object-Localization-Network](https://github.com/ibaiGorordo/ONNX-Object-Localization-Network/raw/main/doc/img/output.jpg)
*Original image: [https://en.wikipedia.org/wiki/File:Interior_design_865875.jpg](https://en.wikipedia.org/wiki/File:Interior_design_865875.jpg)*

# Important
- I added a bit of logic to the box color selection to make it look nicer. Since it performs K-Means for each box, it might be slow. If you only care about speed, you can either set all the boxes to the same color or use random colors.

# Requirements

 * Check the **requirements.txt** file. 
 * For ONNX, if you have a NVIDIA GPU, then install the **onnxruntime-gpu**, otherwise use the **onnxruntime** library.
 * Additionally, **pafy** and **youtube-dl** are required for youtube video inference.
 
# Installation
```
git clone https://github.com/ibaiGorordo/ONNX-Object-Localization-Network.git
cd ONNX-Object-Localization-Network
pip install -r requirements.txt
```
### ONNX Runtime
For Nvidia GPU computers:
`pip install onnxruntime-gpu`

Otherwise:
`pip install onnxruntime`

### For youtube video inference
```
pip install youtube_dl
pip install git+[https://github.com/zizo-pro/pafy@b8976f22c19e4ab5515cacbfae0a3970370c102b](https://github.com/zizo-pro/pafy@b8976f22c19e4ab5515cacbfae0a3970370c102b)
```

# ONNX model
The original model was converted to ONNX by [PINTO0309](https://github.com/PINTO0309), download the models from the download script in [his repository](https://github.com/PINTO0309/PINTO_model_zoo/tree/main/264_object_localization_network) and save them into the **[models](https://github.com/ibaiGorordo/ONNX-Object-Localization-Network/tree/main/models)** folder. 
- The License of the models is Apache-2.0 License: [https://github.com/mcahny/object_localization_network/blob/main/LICENSE](https://github.com/mcahny/object_localization_network/blob/main/LICENSE)

# Pytorch model
The original Pytorch model can be found in this repository: [https://github.com/mcahny/object_localization_network](https://github.com/mcahny/object_localization_network)
 
# Examples

 * **Image inference**:
 ```
 python image_object_localization.py
 ```
 
 * **Webcam inference**:
 ```
 python webcam_object_localization.py
 ```

 * **Video inference**: [https://youtu.be/n9qhQJXYUWo](https://youtu.be/n9qhQJXYUWo)
 ```
 python video_object_localization.py
 ```
 ![!Object-Localization-Network video](https://github.com/ibaiGorordo/ONNX-Object-Localization-Network/raw/main/doc/img/oln_box.gif)
  
 *Original video: [https://youtu.be/vgJUXvkdS78](https://youtu.be/vgJUXvkdS78)*

# References:
* Object-Localization-Network model: [https://github.com/mcahny/object_localization_network](https://github.com/mcahny/object_localization_network)
* PINTO0309's model zoo: [https://github.com/PINTO0309/PINTO_model_zoo](https://github.com/PINTO0309/PINTO_model_zoo)
* Original paper: [https://arxiv.org/abs/2108.06753](https://arxiv.org/abs/2108.06753)
