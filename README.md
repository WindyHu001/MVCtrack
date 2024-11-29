# MVCTrack: Boosting 3D Point Cloud Tracking via Multimodal-Guided Virtual Cues

**Authors**: Zhaofeng Hu<sup>1†</sup>, Sifan Zhou<sup>2†*</sup>, Shibo Zhao<sup>3</sup>, Zhihang Yuan<sup>4</sup>  
<sup>1</sup>Stony Brook University, <sup>2</sup>Southeast University, <sup>3</sup>Carnegie Mellon University, <sup>4</sup>Houmo AI  
† Equal contribution, *Corresponding author  

---

## Overview

MVCTrack is an enhanced framework for **3D single object tracking (3D SOT)** in point clouds, designed to address the limitations of sparse and incomplete LiDAR data. Our approach introduces a **Multimodal-guided Virtual Cues Projection (MVCP)** scheme to enrich sparse point clouds by integrating RGB camera data, significantly improving tracking performance, particularly in scenarios with distant or small objects.

![framework](https://github.com/WindyHu001/MVCtrack/blob/master/figures/backbone.png)

This repository provides the code for **MVCTrack**, which achieves state-of-the-art performance on the **NuScenes dataset**.

---
## Video

[![Watch the video](https://img.youtube.com/vi/c-OPJ0PvvbA/hqdefault.jpg)](https://www.youtube.com/watch?v=c-OPJ0PvvbA)


## Key Features
### **Multimodal-guided Virtual Cues Projection (MVCP)**
A novel, lightweight, and plug-and-play scheme that:
1. Utilizes **2D object detection** to generate virtual cues from RGB images.
2. Projects dense 2D semantic information into **3D space** to balance point cloud density.
3. Enhances the **sparsity and completeness** of point clouds.

### **MVCTrack Framework**
An end-to-end 3D SOT tracker that:
1. Seamlessly integrates the MVCP scheme to improve tracking accuracy.
2. Effectively balances point density distribution across different distances.
3. Achieves competitive performance with minimal computational overhead.

### **State-of-the-Art Performance**
- Evaluated on the large-scale **NuScenes dataset**.
- Significantly surpasses existing multi-modal 3D trackers.
- Demonstrates exceptional performance in sparse and occluded scenarios.

![framework](https://github.com/WindyHu001/MVCtrack/blob/master/figures/nuScenes.png)


---
## Installation
Below are the key dependencies for running MVCTrack:

| Dependency | Version  |
|------------|----------|
| Python     | 3.9.0    |
| PyTorch    | 2.0.1    |
| MMEngine   | 0.7.4    |
| MMCV       | 2.0.0    |
| MMDet      | 3.0.0    |
| MMDet3D    | 1.1.0    |
| SpConv     | 2.3.6    |
| YAPF       | 0.40.0   |
## Acknowledgement

Our implementation is based on Open3DSOT, BEVTrack, P2P, MMDetection3D and MVP. Thanks for the great open-source work!

## Citation
If any parts of our paper and code help your research, please consider citing us and giving a star to our repository.


