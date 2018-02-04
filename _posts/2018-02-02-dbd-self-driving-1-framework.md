---
layout: post
title:  "[MYOA日积月累]自动驾驶 (1) 技术框架"
date:   2018-02-02 00:10:53 +0800
categories: jekyll update
---

作为系列的第一篇文章，从开放的自动驾驶框架——百度发起的Apollo，来看看自动驾驶的技术框架。

这个技术框架可以从很多的文章和介绍资料里看到，例如附在文末的本次图片引用出处。

# Apollo技术框架的分层
由下到上，代表着技术框架由基础到高端的层次关系，有以下四个平台。
* Reference Vehicle Platform 
* Reference Hardware Platform
* Open Software Platform
* Cloud Service Platform
其实就是车辆、硬件、软件、云这四层。其中，值得一提的是，软件层带了"Open"也就是"开放"这个单词，而底层的两层都是带着"Reference"也就是"参考"这个单词。"开放"的含义是能力开放，"参考"的含义是Apollo指定了一个参考配置。按官方说法，能力会持续地通过开源等形式开放出来；参考硬件和车辆是市面上可以买得到的商品，而不再是实验室中可遇不可求的试验品。虽然软件可能调试不宜，车辆和硬件可能价格不菲，但这的确为我们开发者探索自动驾驶技术打开了一扇门。

# Reference Vehicle Platform
Reference Vehicle Platform 是参考车辆平台，其中的模块只有一个，是Drive-by-wire Vechile，也就是线控车。

# Reference Hardware Platform
Reference Hardware Platform 是参考硬件平台，有如下的模块。
* Computing Unit 计算单元
* GPS/IMU 卫星/惯性导航仪
* Camera 摄像头
* LiDAR 激光雷达
* Radar 毫米波雷达
* HMI Device 人机交互设备
* Black Box 黑匣子

# Open Software Platform
Open Software Platform 是开放软件平台，有如下的模块。
* RTOS 实时操作系统
* Runtime Framework 执行时框架
* Map Engine 地图引擎
* Localization 定位
* Perception 感知
* Planning 规划（含决策）
* Control 控制
* End-to-End 端到端
* HMI 人机交互

# Cloud Service Platform
Cloud Service Platform是云服务平台，有如下的模块。
* HD Map 高精地图
* Simulation 仿真
* Data Platform 数据平台
* Security 安全
* OTA 空中下载升级
* DuerOS 小度操作系统（语音交互）

具体框架模块在后续的文章中讨论。

参考资料：
Apollo（官网）
ApolloAuto/apollo（Github）
百度为何预言2050年95%汽车实现L4级自动驾驶_中证网
