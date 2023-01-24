---
layout: post
title: UnrealCV stereo depth generation
date: 2021-09-05 12:01:35 
last_modified_at: 2022-09-20 10:48:33 
url: https://github.com/ibaiGorordo/UnrealCV-stereo-depth-generation
image:
  path: https://github.com/ibaiGorordo/UnrealCV-stereo-depth-generation/raw/main/doc/img/unrealcvStereo.gif
  alt: UnrealCV stereo depth
tags: [unrealcv, unreal-engine-4, computer-vision, stereo-vision, stereo-depth-estimation, synthetic-data]
categories: ["Repository", Python]
---

## [Open In Github](https://github.com/ibaiGorordo/UnrealCV-stereo-depth-generation)[![Open In Github](https://icons-for-free.com/download-icon-part+1+github-1320568339880199515_0.svg)](https://github.com/ibaiGorordo/UnrealCV-stereo-depth-generation)

Python scripts for generating synthetic stereo depth data using the UnrealCV library.

# Example (https://youtu.be/Yui48w71SG0)
![UnrealCV stereo depth](https://github.com/ibaiGorordo/UnrealCV-stereo-depth-generation/raw/main/doc/img/unrealcvStereo.gif)

# How to use
* Download the binary scene from the model zoo: [http://docs.unrealcv.org/en/master/reference/model_zoo.html](http://docs.unrealcv.org/en/master/reference/model_zoo.html)
* Install pyunrealcv: `pip install unrealcv`
* Important:bangbang: Modify the **unrealcv.ini** file in the `WindowsNoEditor/RealisticRendering/Binaries/Win64` path (depending on the OS system) inside the scene folder like this:

`EnableRightEye=True`

* Run `python generate_stereo_unrealcv.py` 


# References
* **UnrealCV**: [https://github.com/unrealcv/unrealcv](https://github.com/unrealcv/unrealcv)
