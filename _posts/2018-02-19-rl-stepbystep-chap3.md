---
layout: post
category: "rl"
title: "深入浅出强化学习-chap3 基于模型的动态规划方法"
tags: [深入浅出强化学习, 基于模型的动态规划]
---

目录

<!-- TOC -->

- [1. 基于模型的动态方法理论](#1-基于模型的动态方法理论)
- [2. 动态规划中的数学基础](#2-动态规划中的数学基础)
    - [2.1 线性方程组的迭代解法](#21-线性方程组的迭代解法)
    - [2.2 压缩映射证明策略评估的收敛性](#22-压缩映射证明策略评估的收敛性)
- [3. 基于gym的编程实例](#3-基于gym的编程实例)
- [4. 最优控制与强化学习比较](#4-最优控制与强化学习比较)

<!-- /TOC -->



参考**《深入浅出强化学习》**

## 1. 基于模型的动态方法理论

一个完整的已知模型的马尔科夫决策过程可以用元组`\(S,A,P,r,\gamma\)`表示。`\(S\)`为状态集，`\(A\)`为动作集，`\(P\)`为**转移概率**【对应环境和智能体的**模型**】，`\(r\)`为回报函数，`\(\gamma\)`为折扣因子，用于计算累积回报`\(R=\sum_{t=0}^T\gamma ^tr_t\)`。若`\(T\)`为有限值，强化学习过程称为有限范围强化学习。若`\(T=\infty\)`，称为无限范围强化学习。下面以有限范围强化学习为例。

强化学习的目标是找到最优策略`\(\pi\)`，使得累积回报的期望最大。策略是状态到动作的映射`\(\pi:s\rightarrow a\)`，`\(tau \)`表示从状态`\(s_t\)`到最终状态`\(s_T\)`的一个序列`\(\tau:s_t,s_{t+1},...,s_T\)`，目标函数是累积回报函数的期望`\(\int R(\tau)p_{\pi}(\tau)d\tau\)`。


## 2. 动态规划中的数学基础

### 2.1 线性方程组的迭代解法

### 2.2 压缩映射证明策略评估的收敛性

## 3. 基于gym的编程实例

## 4. 最优控制与强化学习比较
