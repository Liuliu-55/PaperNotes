# # PointFusion: Deep Sensor Fusion for 3D Bounding Box Estimation  

## Metadata


* Authors: [[Danfei Xu]], [[Dragomir Anguelov]], [[Ashesh Jain]]

## ## Abstract

We present PointFusion, a generic 3D object detection method that leverages both image and 3D point cloud information. Unlike existing methods that either use multistage pipelines or hold sensor and dataset-speciﬁc assumptions, PointFusion is conceptually simple and applicationagnostic. The image data and the raw point cloud data are independently processed by a CNN and a PointNet architecture, respectively. The resulting outputs are then combined by a novel fusion network, which predicts multiple 3D box hypotheses and their conﬁdences, using the input 3D points as spatial anchors. We evaluate PointFusion on two distinctive datasets: the KITTI dataset that features driving scenes captured with a lidar-camera setup, and the SUN-RGBD dataset that captures indoor environments with RGB-D cameras. Our model is the ﬁrst one that is able to perform better or on-par with the state-of-the-art on these diverse datasets without any dataset-speciﬁc model tuning.


## Zotero links
[==*Read it now! See in Zotero*==]()

* [Local library](zotero://select/items/1_4YM4ZIKK)

 * PDF Attachments
	- [Xu et al_2018_PointFusion.pdf](zotero://open-pdf/library/items/2UR8IES6)

* DOI: [10.1109/CVPR.2018.00033](https://doi.org/10.1109/CVPR.2018.00033)

* Cite key: PointFusionDeepSensorFusion3DBoundingBoxEstimation
 
***
## Summary

  
## Research Objective(s)
3D[[目标检测论文]]

## Background / Problem Statement
* MV3D假设对象在自上而下的2D视图中都可以进行分割，但没有考虑到室内情况
* 自上而下的2D视图对行人以及自行车无法进行有效目标检测
* 对点云进行映射后输入网络会丢掉一部分信息，且很难保证点云稀疏性---------->使用异质结构网络（PointNet）

## Contribute(s)
* 能与所有的2D检测器结合，具有通用性
* 提出一个密集融合网络（dense fusion network）对两个异型网络进行融合

## Method(s)


## Evaluation


## Conclusion


## Notes


## References
PointNet