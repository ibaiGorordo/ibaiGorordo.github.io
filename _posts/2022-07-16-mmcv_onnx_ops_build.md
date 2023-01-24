---
layout: post
title: mmcv_onnx_ops_build
date: 2022-07-16 07:27:29 
last_modified_at: 2022-07-17 06:29:20 
url: https://github.com/ibaiGorordo/mmcv_onnx_ops_build
image:
  path: https://socialify.git.ci/ibaiGorordo/mmcv_onnx_ops_build/image?&forks=1&issues=1&language=1&name=1&owner=1&stargazers=1&theme=Light
  alt: mmcv_onnx_ops_build
categories: ["Repository", CMake]
---

## [Open In Github](https://github.com/ibaiGorordo/mmcv_onnx_ops_build)[![Open In Github](https://icons-for-free.com/download-icon-part+1+github-1320568339880199515_0.svg)](https://github.com/ibaiGorordo/mmcv_onnx_ops_build)

 Repository for building the ONNX compatible ops in MMCV to run them in onnxruntime.

# Requirements
* A C/C++ compiler for your operating system (gcc on Linux, Visual Studio on Windows, CLang on Mac)
* [Cmake](https://cmake.org/)
* [Git](https://git-scm.com/book/en/v2/Getting-Started-Installing-Git)


# Installation
1. Download the appropriate ONNX Runtime library for your system from the **[Releases](https://github.com/microsoft/onnxruntime/releases)** and extract the contents of the **lib** folder into the **[libs/onnxruntime](https://github.com/ibaiGorordo/mmcv_onnx_ops_build/tree/main/libs/onnxruntime)** folder.

2. Clone repository with submodules (Note the **--recursive** part)
```
git clone https://github.com/ibaiGorordo/mmcv_onnx_ops_build.git --recursive
cd mmcv_onnx_ops_build
```

3. Compile the library
