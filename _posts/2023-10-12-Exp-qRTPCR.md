---
layout: post
title: qRT-PCR
author: Ke Yi
categories: protocol
tags: [experiment, molecular biology, RNA]
date: 2023-8-8 09:19 +0800
last_modified_at: 2023-10-12 19:58 +0800
toc: true
---

### 描述：
>qRT-PCR实验方法

### 方法
#### 1. Trizol法提取组织RNA
1. 材料准备：DEPC水、氯仿、异丙醇、无水乙醇、Trizol
2. 取出组织样本，置于冰上（~50 mg）；
3. 用DEPC水和75%乙醇清洗组织研磨珠2次，用无尘纸擦干；
4. 加入Trizol 500 µL，开始研磨组织（每次3-5 s，提起搁置8 s，重复8-10次），直到无明显颗粒；
5. 换样，需先清洗研磨珠？
6. 室温静置5 min，加100 µL氯仿，出现分层；
7. 涡旋振荡15 s（低档轻微震荡）；
8. 室温静置2 min，12000 rpm 4 °C 离心15 min；
9. 使用100 µL移液器少量多次 转移上清液，取20-30 µL即可；
10. 加500 µL异丙醇，涡旋振荡15 s；
11. 室温静置10 min，12000 rpm 4°C离心15 min，缓慢倒出管中液体；
12. 加1 mL 75%乙醇（DEPC水稀释），涡旋振荡30 s，12000 rpm 4 °C离心5 min，缓慢倒出管中液体；
13. 倒扣与无尘纸上晾干；
14. 加20 µL DEPC水，反复吹打10 s，测浓度，-80 °C保存；
---
#### 2. 一步法RT-qPCR
1. 一步法试剂盒：PreScript One-Step RT-qPCR SYBR Green Kit (EnzyValley, Cat#S033A/B)
2. 在冰上按表格1配制反应体系
3. 盖上盖子，轻柔混匀，瞬时离心，确保所有组分在管底；
4. 按表格2设置反应程序，选择ROX校正的qPCR一起以无ROXIV信号读取模式；

表格1：<mark>标黄</mark>为试剂盒组分

| 组分                                    | 体积 (µL) |
| --------------------------------------- | --------- |
| Add RNase Free ddH2O                    | To 25     |
| <mark>2× One-Step RT-qPCR Buffer</mark>              | 12.5      |
| <mark>C-SsoRobust Taq DNA Polymerase（5U/µL）</mark> | 0.5       |
| <mark>Prescript III RT Enzyme Mix</mark>             | 0.5       |
| Forward Primer (10 µM)                  | 0.5       |
| Reverse Primer (10 µM)                  | 0.5       |
| Total RNA (10 pg-100 ng)                | 2         |

表格2：

| 阶段    | 温度  | 时间   | 循环 | 荧光信号采集 |
| ------- | ----- | ------ | ---- | ------------ |
| 反转录  | 50 °C | 5 min  | 1×   | 否           |
| 预变性  | 95 °C | 10 min | 1×   | 否           |
| PCR反应 | 95 °C | 5 Sec  | 40×  | 否           |
|    ↑     | 60 °C | 30 Sec | ↑    | 是             |
