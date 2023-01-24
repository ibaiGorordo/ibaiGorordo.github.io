---
layout: post
title: depthai android jni example
date: 2021-12-22 11:55:31 
last_modified_at: 2022-11-27 03:26:53 
url: https://github.com/ibaiGorordo/depthai-android-jni-example
image:
  path: https://socialify.git.ci/ibaiGorordo/depthai-android-jni-example/image?&forks=1&issues=1&language=1&name=1&owner=1&stargazers=1&theme=Light
  alt: depthai android jni example
tags: [android, computer-vision, cpp, deep-learning, depthai, jni-android, object-detection]
categories: ["Repository", C++]
---

## [Open In Github](https://github.com/ibaiGorordo/depthai-android-jni-example)[![Open In Github](https://icons-for-free.com/download-icon-part+1+github-1320568339880199515_0.svg)](https://github.com/ibaiGorordo/depthai-android-jni-example)

 Android example to get the rgb and disparity images from the OAK-D device connected to a phone.

[https://user-images.githubusercontent.com/43162939/155553973-ade18226-4111-426d-a4bc-cffdee4a0063.mp4](https://user-images.githubusercontent.com/43162939/155553973-ade18226-4111-426d-a4bc-cffdee4a0063.mp4)


# Important
- This example is a simple example to show how to use the depthai library in Android and still it is in progress, so expect bugs. For a proper support of the library in Android, you will have to wait a bit more for the official release.
- Known issue: it is necessary to allow the app to acces the MyriadX (multiple times) every time the app launches. If you have any solutions, please submit a PR.

# Compiled App (.apk)
If you want to download the app directly without having to compile the project. You can download it in the Release tab.

# Dynamic Library
The [arm64 dynamic library](https://github.com/ibaiGorordo/depthai-android-jni-example/blob/main/app/src/main/libs/depthai/arm64-v8a/libdepthai-core.so) (depthai-core) was compiled in Ubuntu 20.04 using the *xlink_device_search_improvements* branch. If you are interested in compiling it yourself, please ask in the Discord channel referenced below.

# License
I have copied directly some of the include folders for some of the dependency libraries. Therefore, all the code except the ones inside the include folder are free to use. I will try to fix it adding submodules in the future.

# References:
- *depthai-core*: [https://github.com/luxonis/depthai-core.](https://github.com/luxonis/depthai-core.) To build the depthai library for Android, particularly, the *xlink_device_search_improvements* branch.
- *Luxonis Community Discord*: [https://discord.gg/tPczgVdk.](https://discord.gg/tPczgVdk.) Check there to get updates and other information about the products from Luxonis.
- *Colormap function*: [https://www.particleincell.com/2014/colormap.](https://www.particleincell.com/2014/colormap.) Used to draw the disparity by modifying the Short Rainbow example.
