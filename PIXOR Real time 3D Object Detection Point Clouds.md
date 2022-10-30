# # PIXOR: Real-time 3D Object Detection from Point Clouds  

## Metadata

* Tags: #Computer-Science---Computer-Vision-and-Pattern-Recognition

* Authors: [[Bin Yang]], [[Wenjie Luo]], [[Raquel Urtasun]]

## ## Abstract

We address the problem of real-time 3D object detection from point clouds in the context of autonomous driving. Computation speed is critical as detection is a necessary component for safety. Existing approaches are, however, expensive in computation due to high dimensionality of point clouds. We utilize the 3D data more efficiently by representing the scene from the Bird's Eye View (BEV), and propose PIXOR, a proposal-free, single-stage detector that outputs oriented 3D object estimates decoded from pixel-wise neural network predictions. The input representation, network architecture, and model optimization are especially designed to balance high accuracy and real-time efficiency. We validate PIXOR on two datasets: the KITTI BEV object detection benchmark, and a large-scale 3D vehicle detection benchmark. In both datasets we show that the proposed detector surpasses other state-of-the-art methods notably in terms of Average Precision (AP), while still runs at >28 FPS.


## Zotero links
[==*Read it now! See in Zotero*==]()

* [Local library](zotero://select/items/1_W3K3ZXLT)

 * PDF Attachments
	- [Yang et al_2019_PIXOR.pdf](zotero://open-pdf/library/items/A6SNZYUA)

* DOI: [10.48550/arXiv.1902.06326](https://doi.org/10.48550/arXiv.1902.06326)

* Cite key: PIXORRealtime3DObjectDetectionPointClouds
 
***
## Summary
[[目标检测论文]]
  
## Research Objective(s)
基于激光点云的3D目标检测

## Background / Problem Statement
* 机器人技术（自动驾驶）中需要对目标（对象进行）3D检测。
* 含有3D信息的数据格式：RGB-D；LIDAR
* 对于LIDAR：点云数据呈现为非结构化------->可表示为voxel grid（计算消耗大，激光雷达稀疏） 和 2D projection（BEA；RA）----------->RA（对象大小和形状变形）
* two-stage的目标检测技术不具有实时性
## Contribute(s)
* 提出一种3D对象检测方式（PIXOR）：one stage; proposal free; dense obeject detector
* 采用鸟瞰图的映射方式
* 在现实世界中输出精确的边界框

## Method(s)
数据集：KITTI（公开）； TOR4D（私有）


## Evaluation


## Conclusion


## Notes
* 激光点云采用2D表示，没有丢失信息。深度信息以channel的方式存储，但计算更为简单（Lidar point clouds could be exploited as 2D representations without information loss, as its computation become easy）同时，对象不会重叠（objects do not overlap with each other）

## References
