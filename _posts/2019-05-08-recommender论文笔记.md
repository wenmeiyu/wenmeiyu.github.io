---
layout:     post
title:      recommender论文笔记
subtitle:   recommender系统中的矩阵因式分解相关论文笔记
date:       2019-05-08
author:     wenmeiyu
header-img: img/post-bg-ios9-web.jpg
catalog: true
tags:
    - matrix factorization
    - paper
	- recommender system
---
# 参考资料

>[Matrix Factorization Techniques for Recommender Systems](https://www.computer.org/csdl/magazine/co/2009/08/mco2009080030/13rRUxBa5fj)
>[l-Injection: Toward Effective Collaborative Filtering Using Uninteresting Items](https://ieeexplore.ieee.org/abstract/document/7913668)
>[A non negative matrix factorization for collaborative filtering recommender systems based on a Bayesian probabilistic model](https://www.sciencedirect.com/science/article/pii/S0950705115005006)

# paper1 matrix factorization

matrix          矩阵
factorization  因式分解
techniques
for
recommender
systems

#### 1.Abstract/Background   摘要/背景

Netflix Prize  competition  Netflix大奖赛

#### 2.Recommender system strategies 推荐系统策略

content filtering 内容过滤
broadly speaking 广泛地说
profile 轮廓，外形，简况，特征
genre 类型，种类
and so forth 等等
content-based strategies require gathering external information that might not be available or easy to collect   产品（电影/音乐）和用户特征信息不易采集
Music Genome Project  音乐基因组计划
alternative 选择性的，交替的

#### 3.Matrix factorization methods  矩阵因式分解方法

#### 4.A basic matrix factorization model  基于矩阵因式分解的模型
singular value decomposition(SVD)  奇异值分解

#### 5.Learning algorithms

- Stochastic gradient descent  随机的  梯度  下降    随机梯度下降
- Alternating least squares   交替的  最少的 平方    交替最小二乘  

#### 6.Adding biases  增加 偏差

#### 7.Additional input sources  额外的 输入 源

#### 8.Temporal dynamics   动力学  时间动态

#### 9.Inputs with varying confidence levels  具有不同置信水平的输入

#### 10.Netflix prize competition    Netflix大奖赛

extent 程度，范围

---
# paper2 l-Injection

l-Injection  注射
toward  向
effecttive  有效的
collaborative  协同
filtering     过滤
using
uninteresting  无趣味的，乏味的
items

Collaborative Filtering  协同过滤

novel  稀奇的
framework  框架
sparsity 稀疏
unrated  未分级的

All **datasets** and codes that we used are available at:[https://goo.gl/KUrmip](https://goo.gl/KUrmip)
已下载哈哈哈哈哈

the Watcha dataset is privately  私下的
released from a Korean movie recommendation company
[http://watcha.net](http://watcha.net)

CCF-推荐的会议和期刊：[https://www.ccf.org.cn/xspj/gyml/](https://www.ccf.org.cn/xspj/gyml/)


#### 1.Introduction   介绍
preferences 偏好

#### 2.Preliminaries  预赛

#### 3.Proposed Approach  被提及的方法  提出 方法
- 3.1 Inferring Pre-Use Preferences  推理  使用前 偏爱，优先权
- 3.2 Identifying Uninteresting Items  识别  无趣的 目标
- 3.3 l-Injection  注射
- 3.4 Why Does the l-Injected Matrix Help?

#### 4.Experiments 实验

- 4.1 Experimental Setup   实验步骤
- 4.2 Inference of Pre-Use Preferences    推理  使用前 偏爱，优先权
- 4.3 User Satisfaction for Uninteresting Items  用户的 满意 无趣的 目标
- 4.4 Effect of l-Injection  影响
- 4.5 Accuracy of Modified CF Algorithms  精确度  改进的
- 4.6 Running Time of Modified CF Algorithms 改进的
- 4.7 Summary of Experimental Results   摘要

#### 5.Related Work  相关工作

#### 6.Conclusions   总结

---
# review paper
杨博, 赵鹏飞. 推荐算法综述[J]. 山西大学学报(自然科学版), 2011, 34(3):337-350.
2 　问题及分析
2 .1 　稀疏性问题
实际应用中数据的稀疏性
2 .2 　可扩展性问题
算法复杂度
2 .3 　特征提取问题
基于内容推荐的多样性
2 .4 　其他问题
例如托攻击问题[ 63] 、隐私问题[ 64]

---
# paper3 non negative matrix factorization 

A non negative matrix factorization 非负矩阵因式分解
for collaborative filtering 
recommender systems 
based on a Bayesian probabilistic model






