---
layout: post
title: Mediapipe Christmas Examples
date: 2022-12-17 12:22:40 
last_modified_at: 2022-12-31 11:03:23 
url: https://github.com/ibaiGorordo/Mediapipe-Christmas-Examples
image:
  path: https://github.com/ibaiGorordo/Mediapipe-Christmas-Examples/raw/main/doc/img/backgorund_christmas.gif
  alt: Mediapipe Christmas Background
categories: ["Repository", Python]
---

## [Open In Github](https://github.com/ibaiGorordo/Mediapipe-Christmas-Examples)[![Open In Github](https://icons-for-free.com/download-icon-part+1+github-1320568339880199515_0.svg)](https://github.com/ibaiGorordo/Mediapipe-Christmas-Examples)

Python scripts using the Mediapipe models for Christmas.

# WHY
Mainly for fun. But this repository also includes useful examples for things like image transformations (affine), image overlapping, model inference...

# Installation
```
git clone https://github.com/ibaiGorordo/Mediapipe-Christmas-Examples
cd Mediapipe-Christmas-Examples
pip install -r requirements.txt
```
# Original models
Most of the models were taken from Mediapipe: [https://google.github.io/mediapipe/solutions/solutions.html.](https://google.github.io/mediapipe/solutions/solutions.html.)

# Examples

 * **Christmas Background**:

  ![Mediapipe Christmas Background](https://github.com/ibaiGorordo/Mediapipe-Christmas-Examples/raw/main/doc/img/backgorund_christmas.gif)

   - Webcam: `python webcam_christmas_background.py`
   - Video: `python video_christmas_background.py`

 * **Reindeer Face**:

  ![Mediapipe Reindeer Face](https://github.com/ibaiGorordo/Mediapipe-Christmas-Examples/raw/main/doc/img/reindeer.gif)
   - Webcam: `python webcam_reindeer_face.py`
   - Video: `python video_reindeer_face.py`

 * **Santa Face Mesh**:

  ![Mediapipe Exorcist Face Mesh](https://github.com/ibaiGorordo/Mediapipe-Christmas-Examples/raw/main/doc/img/santa_face.gif)
   - Webcam: `python webcam_facemesh_santa.py`
   - Video: `python video_facemesh_santa.py`


# References:
- Halloween examples: [https://github.com/ibaiGorordo/Mediapipe-Halloween-Examples](https://github.com/ibaiGorordo/Mediapipe-Halloween-Examples)
Check the header in each of the scripts for the references for each model.
