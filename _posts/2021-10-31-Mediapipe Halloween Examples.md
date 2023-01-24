---
layout: post
title: Mediapipe Halloween Examples
date: 2021-10-31 10:48:38 
last_modified_at: 2023-01-20 10:21:38 
url: https://github.com/ibaiGorordo/Mediapipe-Halloween-Examples
image:
  path: https://github.com/ibaiGorordo/Mediapipe-Halloween-Examples/raw/main/doc/img/skeleton.gif
  alt: Mediapipe Skeleton Pose
---
Python scripts using the Mediapipe models for Halloween.

# WHY
Mainly for fun. But this repository also includes useful examples for things like image transformations (affine), image overlapping, model inference...

# Installation
```
git clone https://github.com/ibaiGorordo/Mediapipe-Halloween-Examples
cd Mediapipe-Halloween-Examples
pip install -r requirements.txt
```
# Original models
Most of the models were taken from Mediapipe: https://google.github.io/mediapipe/solutions/solutions.html. However, the hair segementation model is not currently suppoeted in Python, instead the model from [Kazuhito00's](https://github.com/Kazuhito00) repository was used: https://github.com/Kazuhito00/Skin-Clothes-Hair-Segmentation-using-SMP

# Examples

 * **Skeleton Pose**:

  ![Mediapipe Skeleton Pose](https://github.com/ibaiGorordo/Mediapipe-Halloween-Examples/raw/main/doc/img/skeleton.gif)
 ```
 python webcamSkeletonPose.py
 ```

 * **Halloween background**:

  ![Mediapipe Halloween background](https://github.com/ibaiGorordo/Mediapipe-Halloween-Examples/raw/main/doc/img/halloween_background.gif)
 ```
 python webcamHalloweenBackground.py
 ```

 * **Exorcist Face Mesh**:

  ![Mediapipe Exorcist Face Mesh](https://github.com/ibaiGorordo/Mediapipe-Halloween-Examples/raw/main/doc/img/exorcist.gif)
 ```
 python webcamFaceMeshExorcist.py
 ```

 * **Pumpkin face**:

  ![Mediapipe Pumpkin face](https://github.com/ibaiGorordo/Mediapipe-Halloween-Examples/raw/main/doc/img/pumpkin_face.gif)
 ```
 python webcamPumpkinFace.py
 ```

 * **Fire Hair**:

  ![Mediapipe Fire Hair](https://github.com/ibaiGorordo/Mediapipe-Halloween-Examples/raw/main/doc/img/fire_hair.gif)
 ```
 python webcamFireHair.py
 ```
 



# References:
Check the header in each of the scripts for the references for each model.
