---
description: 基于Zynq架构的多个实验的开发文档与学习步骤（长期持续更新）
---

# Takk\_Zynq\_Labs中文

## 1. 概述

### 1.1 实验内容

1. 在Xilinx Vivado平台基于Verilog开发的Zynq实验（大概有10+个，主要以计算机视觉应用为主）
2. 嵌入式的Zynq基础开发实验 Linux/_PetaLinux（大概有5个，主要实现Linux移植与内核模块以及简单驱动的开发，实现在Linux下调用PL部分协同计算的方案）_
3. _使用VivadoHLS工具进行计算机视觉的IP核开发，可能涉及一些深度学习和CNN RNN网络 与 SAFT 算法等。_
4. _SDSOC软件的使用与简单视觉应用在SDSOC开发_
5. 基于PYNQ的计算机视觉开发与CNN模型 LENET YOLO等开发。



_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\_\__

同时在所有实验录制结束后，会录制几个实战工程：

1. 基于Verilog实现LeNet、VGG、ResNet 、F-RNN 等网络的方案与步骤
2. 基于SAFT-COSH方法的SAFT计算实现
3. 基于Verilog实现的双目视觉立体匹配与视差优化
4. 传统图像处理（涉及角点、人脸、形状、特征等）

### 1.2. 实验清单

#### 1.2.1  无操作系统的Zynq裸机开发

* Lab01\_Zynq中的PS部分介绍与串口打印
* Lab02\_Zynq中的PS与PL交互
* Lab03\_Zynq上的VGA驱动与Block Design思想
* Lab04\_Zynq上通过PS部分控制PL VGA IP 进行图像显示
* Lab05\_PL部分实现IIC驱动模块 （OV7725摄像头
* Lab06\_PS部分实现IIC驱动模块（OV7725摄像头
* Lab07\_PL实现OV7725摄像头数据采集模块
* Lab08\__纯PL部分实现摄像头采集与显示_
* Lab09\_PL与PS协同实现摄像头采集显示
* Lab10\_使用vivado HLS进行视频处理IP开发的基础分析与实践
* Lab11\_Zynq上用Verilog编写简单AXI-Stream接口视频处理IP模块
* Lab12\_PS部分的卷积模块
* Lab13\__PL部分的卷积模块_
* Lab14\_Zynq上的_Sobel边缘检测_
* Lab15\_Zynq上的_通用卷积IP_
* Lab16\_Zynq上的_图像处理开发流程_
* Lab17\_流水线优化视频处理模块
* Lab18\_Zynq上定点小数与浮点小数表示与运算
* Lab19\_Zynq上简单神经网络的实现
* Lab20\_Zynq上的Softmax层实现
* Lab21\_Zynq上LeNet进行车辆识别的示例与方案介绍
* Lab22\_欢迎建议，持续更新....

持续更新列表，正式视频预计1月10日在bilibili平台上开始更新。所有实验涉及的源码将在Github开源。

Email: taneey0519@gmail.com

All Labs' code will be there  [https://github.com/Takk-Tanee/Takk\_Zynq\_Labs](https://github.com/Takk-Tanee/Takk\_Zynq\_Labs)





This is just for Takk\_Zynq\_Labs test.

This is just for Takk\_Zynq\_Labs test.