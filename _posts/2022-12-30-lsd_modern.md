---
layout: post
title: lsd_modern
date: 2022-12-30 02:44:04 
last_modified_at: 2023-01-06 09:14:56 
url: https://github.com/ibaiGorordo/lsd_modern
image:
  path: https://github.com/ibaiGorordo/lsd_modern/raw/main/doc/img/lines.jpg
  alt: LSD
categories: ["Repository", C++]
---

## [Open In Github](https://github.com/ibaiGorordo/lsd_modern)[![Open In Github](https://icons-for-free.com/download-icon-part+1+github-1320568339880199515_0.svg)](https://github.com/ibaiGorordo/lsd_modern)

 C++ code to try to modernize the original Line Segment Detect code

## Line Detection Comparison
Image comparison between pytlsd C++ (left) and Opencv C++ (right).
![LSD](https://github.com/ibaiGorordo/lsd_modern/raw/main/doc/img/lines.jpg)


Table with the comparison (ms) of the different parts of the code:

|                     | OpenCV (C++) | pytlsd (C++) | lsd_modern |
|---------------------|--------------|--------------|------------|
| Gaussian Blur       | 0.5          | 43           | 8          |
| Gaussian Downsample | 1.5          | 31           | 10         |
| Total               | 48           | 214          |            |

For a more detailed comparison check the [COMPARISONS.md](https://github.com/ibaiGorordo/lsd_modern/blob/main/COMPARISONS.md) file.

# Ref:
- LSD paper: [LSD: A Line Segment Detector](https://www.ipol.im/pub/art/2012/gjmr-lsd/)
- Original C code: [lsd c code](https://github.com/theWorldCreator/LSD)
- pytlsd repo: [pytlsd](https://github.com/rpautrat/pytlsd)
- Fast Gaussian blur: [Fast Gaussian blur](http://blog.ivank.net/fastest-gaussian-blur.html)
- Separable Convolution: [Separable Convolution](https://github.com/chaowang15/fast-image-convolution-cpp)


