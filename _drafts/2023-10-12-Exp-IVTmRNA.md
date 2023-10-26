---
layout: post
title: 体外转录 IVT mRNA
author: Ke Yi
categories: protocol
tags: [experiment, molecular biology, RNA]
date: 2022-2-21 17:30 +0800
last_modified_at: 2023-6-6 19:12 +0800
toc: true
---

### 描述：
>  HiScribe ™ T7 ARCA mRNA Kit (with tailing) 货号 NEB # E2060S
>  Link: [HiScribe ™ T7 ARCA mRNA Kit (with tailing)](https://international.neb.com/products/e2060-hiscribe-t7-arca-mrna-kit-with-tailing#Product%20Information)

### 材料
1. <font color="#ff0000">HiScribe ™ T7 ARCA mRNA Kit (with tailing)</font> 试剂盒
2. 模板 dsDNA （<span style="background:#fff88f">含T7启动子接头</span>）
3. DEPC水
4. 冰70%乙醇
5. 可选：纯化方法（LiCl法、苯酚-氯仿法、纯化柱法）

### 方法
#### 1. 模板dsDNA
##### 1.1 T7 promoter:
5'- ==TAATACGACTCACTATA== GGG...(DNA template)-3'
转录后产物为：
5'- GGG...(DNA template)-3'
##### 1.2 质粒模板
略
##### 1.3 PCR模板
PCR正义链引物加T7 promoter

#### 2. 标准mRNA合成
1. 按下表配制反应体系

| Reagent         | Amount   | Final concentration                                               |
| --------------- | -------- | ----------------------------------------------------------------- |
| DEPC水          | to 20 µL |                                                                   |
| 2X ARCA/NTP Mix | 10 µL    | 1 mM GTP, 4 mM ARCA, 1.25 mM CTP, 1.25 mM UTP, >1.25 mM ATP final |
| Template DNA    | x        | 1 µg                                                              |
| T7 RNA 多聚酶   | 2 µL     |                                                                   |

2. 37 °C孵育 30 min
3. 去除模板DNA：加2 µL DNase， 37 °C孵育 15 min
4. 可选：留 1 µL 用于跑胶检测

#### 3. 加尾
1. 按下表配制反应体系

| Reagent                                  | Amount (µL) | Amount (µL) |
| ---------------------------------------- | ----------- | ----------- |
| DEPC水                                   | 20          | 65          |
| IVT reaction                             | 20          | 20          |
| Poly(A) Polymerase Reaction Buffer (10X) | 5           | 10          |
| Poly(A) Polymerase                       | 5           | 5           |
| Total Volume                             | 50          | 100         |

2. 37 °C孵育 30 min
3. 可选：留 1 µL 用于跑胶检测

#### 4. mRNA纯化
##### 4.1 LiCl沉淀法
1. 在50 μL 加尾反应产物中，加入25μl LiCl溶液并充分混合。
2. 在-20℃下孵育30 min。
3. 在4°C下以最高速度离心15 min，使RNA沉淀。
4. 仔细清除上清液。
5. 加入 500 μL 冷的70%的乙醇冲洗RNA沉淀，在4℃下离心10 min。
6. 小心地除去乙醇。短暂旋转试管，使管壁上的液体下降。
7. 用10 µL 枪头小心地除去残留的液体。
8. 晾干颗粒，将mRNA重悬于50 μL 的 DEPC水 中。
9. 将RNA在 65°C 下加热 5-10 min，使RNA完全溶解。搅拌均匀。
10. 将RNA储存在-80 °C。
