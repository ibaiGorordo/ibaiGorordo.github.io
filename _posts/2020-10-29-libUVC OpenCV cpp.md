---
layout: post
title: libUVC OpenCV cpp
date: 2020-10-29 09:11:36 
last_modified_at: 2020-10-29 12:20:32 
url: https://github.com/ibaiGorordo/libUVC-OpenCV-cpp
image:
  path: https://socialify.git.ci/ibaiGorordo/libUVC-OpenCV-cpp/image?&forks=1&issues=1&language=1&name=1&owner=1&stargazers=1&theme=Light
  alt: libUVC OpenCV cpp
categories: ["Repository", C]
---

## [Open In Github](https://github.com/ibaiGorordo/libUVC-OpenCV-cpp)[![Open In Github](https://icons-for-free.com/download-icon-part+1+github-1320568339880199515_0.svg)](https://github.com/ibaiGorordo/libUVC-OpenCV-cpp)

Example script to capture images from USB cameras using the libUVC library and OpenCV in C++.The example runs for 10 seconds and it automatically stops.
**Tested in Ubuntu 20.04.1 LTS**

# Installation
```
git clone https://github.com/ibaiGorordo/libUVC-OpenCV-Cpp.git 
cd libUVC-OpenCV-Cpp
mkdir build
cd build
cmake ..
make
sudo ./sample

```

# Required libraries
* **libusb**: ```sudo apt install libusb-1.0-0-dev```
* **OpenCV**: Built from source (tested on OpenCV 4.5.0)
