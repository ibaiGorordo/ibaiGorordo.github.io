---
layout: post
title: Perception Neuron Read Calc File
date: 2019-06-13 11:30:51 +0000
last_modified_at: 2022-10-02 06:44:43 +0000
url: https://github.com/ibaiGorordo/Perception-Neuron-Read-Calc-File
image:
  path: https://socialify.git.ci/ibaiGorordo/Perception-Neuron-Read-Calc-File/image?&forks=1&issues=1&language=1&name=1&owner=1&stargazers=1&theme=Light
  alt: Perception Neuron Read Calc File
tags: [matlab, perception-neuron, calc-file, motion-capture, inertial-sensors]
categories: ["Repository", MATLAB]
---

## [Open In Github](https://github.com/ibaiGorordo/Perception-Neuron-Read-Calc-File)

Program to read the .calc file from the Perception Neuron (Noitom).

The function takes the filename string and outputs the following variables:
* **skeleton**: Structure array which includes the data for each of the skeleton parts (check the Header variable to find the order of the different parts). Each skeleton part structure contains the following variables:
  * *Name*: Name of the skeleton part.
  * *Pos*: 3D position of the skeleton part.
  * *Vel*: 3D velocity of the skeleton part.
  * *quat*: 3D orientation of the skeleton part in quaternions.
  * *Accel*: 3D Accelerations of the skeleton part.
  * *AngVel*: 3D angular velocities of the skeleton part.
* **timeMat**: Array containing the time information.
* **rightFootContact**: Boolean array containing when the right foot was in contact with the ground.
* **leftFootContact**: Boolean array containing when the right foot was in contact with the ground.
