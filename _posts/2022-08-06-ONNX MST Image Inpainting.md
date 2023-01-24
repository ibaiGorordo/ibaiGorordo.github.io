---
layout: post
title: ONNX MST Image Inpainting
date: 2022-08-06 14:54:59 
last_modified_at: 2023-01-23 00:31:03 
url: https://github.com/ibaiGorordo/ONNX-MST-Image-Inpainting
image:
  path: https://github.com/ibaiGorordo/ONNX-MST-Image-Inpainting/raw/main/doc/img/inpainted.png
  alt: ONNX MST Image Inpainting
tags: [onnx, image-inpainting, inpainting, onnxruntime, onnxruntime-gpu, opencv, python]
categories: ["Repository", Python]
---

## [Open In Github](https://github.com/ibaiGorordo/ONNX-MST-Image-Inpainting)[![Open In Github](https://icons-for-free.com/download-icon-part+1+github-1320568339880199515_0.svg)](https://github.com/ibaiGorordo/ONNX-MST-Image-Inpainting)

Python scripts for performing Image Inpainting using the MST model in ONNX

![!ONNX MST Image Inpainting](https://github.com/ibaiGorordo/ONNX-MST-Image-Inpainting/raw/main/doc/img/inpainted.png)

*Original image: [https://es.wikipedia.org/wiki/Archivo:Perro_Pipper_en_Merida_-_Pipperontour.jpg](https://es.wikipedia.org/wiki/Archivo:Perro_Pipper_en_Merida_-_Pipperontour.jpg)*

# Requirements

 * Check the **requirements.txt** file. 
 * For ONNX, if you have a NVIDIA GPU, then install the **onnxruntime-gpu**, otherwise use the **onnxruntime** library.
 
# Installation
:warning: Make sure to add the recursive when cloning
```
git clone https://github.com/ibaiGorordo/ONNX-MST-Image-Inpainting.git --recursive
cd ONNX-MST-Image-Inpainting
pip install -r requirements.txt
```
### ONNX Runtime
For Nvidia GPU computers:
`pip install onnxruntime-gpu`

Otherwise:
`pip install onnxruntime`

# ONNX model 
Convert the model to ONNX using the Colab repository below and save it into the [models folder](https://github.com/ibaiGorordo/ONNX-MST-Image-Inpainting/tree/main/models)
- **Convert MST Inpainting to ONNX** [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1Nm2Ci423z6jd7XHoh8BTE6rQbTCdJRnU?usp=sharing)
- The License of the models is MIT: [License](https://github.com/ewrfcas/MST_inpainting/blob/main/LICENSE)

# Examples

 * **Image Inpainting (mask already available)**:
 ```
 python image_inpaint.py.py
 ```

   * **Sketch mask and Inpaint**:
 ```
 python sketch_and_inpaint.py.py
 ``` 
![!ONNX MST Image Inpainting with mask sketch](https://github.com/ibaiGorordo/ONNX-MST-Image-Inpainting/raw/main/doc/img/inpaint_image.gif)

# Mask Sketcher Usage
- **Left Mouse Button:** Draw Mask
- **Middle/Wheel Mouse Button:** Remove Mask
- **Bottom slider:** Control mask drawing tool size
- **Press any key to stop sketching**

 [https://user-images.githubusercontent.com/43162939/185775748-de6232e9-518a-45df-8de4-99902f1733c7.mp4](https://user-images.githubusercontent.com/43162939/185775748-de6232e9-518a-45df-8de4-99902f1733c7.mp4)
  
# References:
* MST_inpainting: [https://github.com/ewrfcas/MST_inpainting](https://github.com/ewrfcas/MST_inpainting)
* HAWP: [https://github.com/cherubicXN/hawp](https://github.com/cherubicXN/hawp)
* PINTO0309's model zoo: [https://github.com/PINTO0309/PINTO_model_zoo](https://github.com/PINTO0309/PINTO_model_zoo)
* PINTO0309's model conversion tool: [https://github.com/PINTO0309/openvino2tensorflow](https://github.com/PINTO0309/openvino2tensorflow)
* MST Original paper: [https://arxiv.org/abs/2103.15087](https://arxiv.org/abs/2103.15087)




