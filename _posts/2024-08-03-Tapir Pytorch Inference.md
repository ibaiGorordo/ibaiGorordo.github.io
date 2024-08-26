---
layout: post
title: Tapir Pytorch Inference
date: 2024-08-03 06:48:51 +0000
last_modified_at: 2024-08-23 08:39:52 +0000
url: https://github.com/ibaiGorordo/Tapir-Pytorch-Inference
image:
  path: https://socialify.git.ci/ibaiGorordo/Tapir-Pytorch-Inference/image?&forks=1&issues=1&language=1&name=1&owner=1&stargazers=1&theme=Light
  alt: Tapir Pytorch Inference
tags: [computer-vision, deep-learning, point-tracking, pytorch, tracking]
categories: ["Repository", Python]
---

## [Open In Github](https://github.com/ibaiGorordo/Tapir-Pytorch-Inference)

![!vlcsnap-2024-08-26-13h58m08s098](https://github.com/user-attachments/assets/5d92851e-08fd-40f5-a486-370ca276198b)

## Important
This is a strip down version of the original Tapir repository focused on inference.
- Removed the JAX dependencies and the training code.
- Make it easy to run in real-time even with a camera feed.
- Converted tensors from 5D to 4D (only use one frame)
- ⚠️⚠️⚠️**ONNX Inference is very slow**⚠️⚠️⚠️

## Installation
```shell
git clone https://github.com/ibaiGorordo/Tapir-Pytorch-Inference.git
cd Tapir-Pytorch-Inference
pip install -r requirements.txt
```
- **Download model** from: [https://storage.googleapis.com/dm-tapnet/causal_bootstapir_checkpoint.pt](https://storage.googleapis.com/dm-tapnet/causal_bootstapir_checkpoint.pt)

## License
The License of the original model is Apache 2.0: [License](https://github.com/google-deepmind/tapnet/blob/main/LICENSE)

## ONNX Export
⚠️⚠️⚠️**ONNX Inference is very slow**⚠️⚠️⚠️
```shell    
python onnx_export.py
```

Arguments:
 - **--model**: Path to the model weights
 - **--resolution**: Input resolution (default: 640)
 - **--num_points**: Number of points (default: 1000)
 - **--dynamic**: Export with dynamic number of points (default: False)
 - **--num_iters**: Number of iterations, use 0 for faster inference, 4 for better results (default: 4)
 - **--output_dir**: Output directory (default: ./)

# Examples
[https://github.com/user-attachments/assets/457eeb57-9961-4022-9b15-55f1d9dc2260](https://github.com/user-attachments/assets/457eeb57-9961-4022-9b15-55f1d9dc2260)

## **Video inference**:

 ```shell
 python example_video_tracking.py
 ```

## **Webcam inference**:

 ```shell
 python example_webcam_tracking.py
 ```

## References:
* **TAPIR Repository:** [https://github.com/google-deepmind/tapnet/tree/main](https://github.com/google-deepmind/tapnet/tree/main)
