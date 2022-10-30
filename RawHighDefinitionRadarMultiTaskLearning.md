# # Raw High-Definition Radar for Multi-Task Learning  

## Metadata

* Tags: #Computer-Science---Computer-Vision-and-Pattern-Recognition, #Electrical-Engineering-and-Systems-Science---Image-and-Video-Processing

* Authors: [[Julien Rebut]], [[Arthur Ouaknine]], [[Waqas Malik]], [[Patrick Pérez]]

## ## Abstract

With their robustness to adverse weather conditions and ability to measure speeds, radar sensors have been part of the automotive landscape for more than two decades. Recent progress toward High Definition (HD) Imaging radar has driven the angular resolution below the degree, thus approaching laser scanning performance. However, the amount of data a HD radar delivers and the computational cost to estimate the angular positions remain a challenge. In this paper, we propose a novel HD radar sensing model, FFT-RadNet, that eliminates the overhead of computing the range-azimuth-Doppler 3D tensor, learning instead to recover angles from a range-Doppler spectrum. FFT-RadNet is trained both to detect vehicles and to segment free driving space. On both tasks, it competes with the most recent radar-based models while requiring less compute and memory. Also, we collected and annotated 2-hour worth of raw data from synchronized automotive-grade sensors (camera, laser, HD radar) in various environments (city street, highway, countryside road). This unique dataset, nick-named RADIal for "Radar, Lidar et al.", is available at https://github.com/valeoai/RADIal.


## Zotero links
[==*Read it now! See in Zotero*==]()

* [Local library](zotero://select/items/1_59GZTDNR)

 * PDF Attachments
	- [Rebut et al_2022_Raw High-Definition Radar for Multi-Task Learning.pdf](zotero://open-pdf/library/items/2QE238MA)

* DOI: [10.48550/arXiv.2112.10646](https://doi.org/10.48550/arXiv.2112.10646)

* Cite key: RawHighDefinitionRadarMultiTaskLearning
 
***
## Summary

  
## Research Objective(s)
* 雷达RD视图
* 目标检测&语义分割

## Background / Problem Statement
* 提供雷达点云的方式依赖于雷达信号处理
* 目标检测任务中，往往只利用RD视图进行two-stage的操作
* 没有考虑生成RAD tensor和点云的预处理的成本


## Contribute(s)
* 提出端到端的目标检测模型，处理原始高清雷达数据
* 同时进行目标检测和语义分割
* 使用HD雷达信号的RD数据


## Method(s)
###  MIMO pre encoder
* 对RD张量进行重排列：恢复角度信息；控制数据量
* 两层卷积预编码
	* A suitably-defined Atrous convolution layer
	* A second 3x3 convolution layer

### FPN encoder
* 利用金字塔结构学习多尺度特征

### Range-angle decoder
* 将输入特征图扩展到更高分辨率
* two-Cov-BatchNorm-Relu layers
	* swap: range-doppler --> range-azimuth

### Detection Task
* The Pixor  method(compare)
### Swgmentation Task
* PolarNet(compare)
## Evaluation


## Conclusion


## Notes


## References
