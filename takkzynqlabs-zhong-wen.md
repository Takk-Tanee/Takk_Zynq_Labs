---
description: 基于Zynq架构的多个实验的开发文档与学习步骤（长期持续更新)——Tanee
---

# Takk\_Zynq\_Labs中文

&#x20;   制作这些实例和经验分享的文档与视频，原因是由于国内目前资源较少，生态还不是很丰富。故将个人的开发经验与开发过程作为一个个的案例无偿开源至此。对于某些系统级比较复杂的项目也许会采用有偿的形式发布。但下列大部分实验95%都是无偿开源的。

&#x20;    个人制作的原因是因为经历过开发时的苦恼与不解，总结了个人的经验。并且希望对刚入门的小伙伴能有所帮助。但！这个系列绝非教程，不是教学，并不是代表系统的教学。由于本人能力和学识有限，因此这个系列只作为经验案例分享，存在错误之处或您有任何建议烦请联系本人。

&#x20;    同时十分感谢一直在支持的朋友们。

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

* Lab01\_Zynq介绍与PS端的开发环境
* Lab02\_Zynq中PL与PS通过AXI-Lite协议交互
* Lab03\_Zynq中常用的IO控制(PS\PL)
* Lab04\_Zynq中VTC视频时序控制IP核实现VGA显示
* Lab05\_Zynq中PS通过VDMA与VTC显示自定义图片到VGA显示器
* Lab06\_IIC\SCCB协议与时序
* Lab07\_【摄像头采集系统一】摄像头寄存器IIC配置模块
* Lab08\_【摄像头采集系统二】摄像头数据采集模块
* Lab09\_【摄像头采集系统三】系统Block Design以及上板测试
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



#### 1.2.2  Vivado/Vitis HLS的IP开发

* Lab01\_Vitis HLS安装配置与简介
* Lab02\_UG902总体介绍
* Lab03\_UG902分析一
* Lab04\_UG902分析一
* Lab05\_UG902分析一
* Lab06\_UG902分析一
* Lab07\_UG871实战
* Lab08\_UG1233分析
* Lab09\_HLS常用接口约束介绍与实战分析
* Lab10\_HLS常用优化约束介绍与实战分析
* Lab11\_利用VitisHLS编写第一个图像处理IP
* Lab12\_使用 xfopenncv 在 VitisHLS编写 灰度与sobel IP
* Lab13\_编写自定义的的vitisHLS视频处理库
* Lab14\_VitisHLS 与 HDL 开发对比分析
* Lab15\_VitisHLS实现神经网络的方案
* Lab16\_VitisHLS简单CNNs实现
* Lab16\_VitisHLS实现强化学习的方案
* Lab17\_欢迎建议，持续更新....



#### 1.2.3 Zynq嵌入式Linux环境开发

* Lab01\_在Zynq移植Linux内核
* Lab02\_内核模块以及驱动编写
* Lab03\_在Zynq linux系统中PS侧调用PL处理运算
* Lab04\_在Zynq linux系统中实现图像采集与显示
* Lab05\__PetaLinux介绍与开发流程_
* Lab06\_欢迎建议，持续更新....



#### 1.2.4 PYNQ开发

* Lab01\_在Zynq上部署PYNQ框架
* Lab02\_Overlay的开发与简述
* Lab03\_Pynq开发流程
* Lab04\_Pynq社区的重要性与社区案例分析
* Lab05\__Pynq图像处理开发流程以灰度转化为例_
* Lab06\_Pynq与vitisHLS的协同开发
* Lab07\_Pynq与Verilog手写自定义卷积IP实例
* Lab08\_Pynq实现神经网络的方案
* Lab09\_Pynq部署uNet方案
* Lab10\_Pynq实现SAFT-COSH算法的方案
* Lab11\_欢迎建议，持续更新....

持续更新列表，正式视频预计1月10日在bilibili平台上开始更新。有可能存在直播录制视频的可能。所有实验涉及的源码将在Github开源。

Email: taneey0519@gmail.com

All Labs' code will be there  [https://github.com/Takk-Tanee/Takk\_Zynq\_Labs](https://github.com/Takk-Tanee/Takk\_Zynq\_Labs)





This is just for Takk\_Zynq\_Labs test.

This is just for Takk\_Zynq\_Labs test.
