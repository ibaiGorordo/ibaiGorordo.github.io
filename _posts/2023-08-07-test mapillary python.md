---
layout: post
title: test mapillary python
date: 2023-08-07 12:47:21 +0000
last_modified_at: 2023-08-08 00:52:02 +0000
url: https://github.com/ibaiGorordo/test-mapillary-python
image:
  path: https://github.com/ibaiGorordo/test-mapillary-python/raw/main/doc/img/combined_img.png
  alt:  Mapillary semantic map
categories: ["Repository", Python]
---

## [Open In Github](https://github.com/ibaiGorordo/test-mapillary-python)

 Python scripts for testing the mapillary python library functionalities

# Installation
```bash
pip install git+[https://github.com/ibaiGorordo/mapillary-python-sdk.git@simple_dependencies](https://github.com/ibaiGorordo/mapillary-python-sdk.git@simple_dependencies)
```

# Setup
You need to modify the `mly_token.py` file with your token. To get one:
- Visit [https://www.mapillary.com/dashboard/developer,](https://www.mapillary.com/dashboard/developer,) go to 'developers',
- Then 'register application', register a new application (read access atleast),
- then copy & paste the 'Client Token' to the `mly_token.py` file.

# Current results

## Show Semantic Segmentation map
![! Mapillary semantic map](https://github.com/ibaiGorordo/test-mapillary-python/raw/main/doc/img/combined_img.png)
