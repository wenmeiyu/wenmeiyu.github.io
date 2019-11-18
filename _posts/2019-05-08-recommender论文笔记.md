---
layout:     post
title:      recommender论文笔记
subtitle:   recommender系统中的矩阵因式分解相关论文笔记
date:       2019-05-08
author:     wenmeiyu
header-img: img/post-bg-ios9-web.jpg
catalog: true
tags:
    - paper
---
# 参考资料

>[Matrix Factorization Techniques for Recommender Systems](https://www.computer.org/csdl/magazine/co/2009/08/mco2009080030/13rRUxBa5fj)
>[l-Injection: Toward Effective Collaborative Filtering Using Uninteresting Items](https://ieeexplore.ieee.org/abstract/document/7913668)
>[A non negative matrix factorization for collaborative filtering recommender systems based on a Bayesian probabilistic model](https://www.sciencedirect.com/science/article/pii/S0950705115005006)

---
# paper1 matrix factorization

matrix          矩阵
factorization  因式分解
techniques
for
recommender
systems

Koren, Yehuda, Robert Bell, and Chris Volinsky. "Matrix factorization techniques for recommender systems." Computer 8 (2009): 30-37.

#### 1.Abstract/Background   摘要/背景

Netflix Prize  competition  Netflix大奖赛

#### 2.Recommender system strategies 推荐系统策略

broadly speaking 广泛地说

- two strategies
	- content filtering 内容过滤
		- the Music Genome Project
		- the neighborhood methods and latent factor models

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

[一个关于这篇论文的理解](https://blog.csdn.net/weixin_42081343/article/details/80368298)

SVD(Singular Value Decomposition) 奇异值分解：

[一个用于降维的奇异值分解](https://www.cnblogs.com/pinard/p/6251584.html)
	- 相当于分解成为三个维数更小的矩阵
[一个SVD在推荐系统中的应用](https://www.cnblogs.com/lzllovesyl/p/5243370.html)
	- 优势在于：用户的评分数据是稀疏矩阵，可以用SVD将数据映射到低维空间，然后计算低维空间中的item之间的相似度，对用户未评分的item进行评分预测，最后将预测评分高的item推荐给用户。

## 论文翻译



 
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

- 4.7 Summary of Experimental Results   摘要  总结

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

Knowledge-BasedSystems   ccf-c

#### abstract  
Our technique is based on factorizing  因式分解
the rating matrix 评分矩阵
into two non negative matrices 非负矩阵
whose components 成分
lie with in the range[0,1] with an understandable  
probabilistic  概率的
meaning.

#### 1.Introduction

Recommender systems 分为两大类:

- Based on contents.

- Based on collaborative filtering.
	- Based on Memory
	- Based on models

In our paper we will present an ovel technique for factoring the rating matrix, preserving the advantages of the classical factorization technique:

#### 4.Model

- 4.1 Over view of our technique

## 论文翻译

基于贝叶斯概率模型应用于协同过滤推荐系统的的非负矩阵因式分解

#### 摘要

在这篇文章中，我们提出了一个基于矩阵因式分解的推荐系统的预测用户尝试的新算法。我们的算法是基于分解评分矩阵为两个非负矩阵，矩阵的因素为一个可以理解的概率的意义以及范围在[0,1]区间。通过这个分解我们可以更加准确预测用户的评分，找出具有相似性的用户，同时调整和解释我们算法得出的推荐结果。

#### 1.引言

- 推荐系统是一类能够提供个性化推荐结果给用户的系统。推荐系统已经广泛用于不同的领域，例如音乐，电视剧，书籍，线上学习和电子商务。但是，大多数的论文研究主要关注电影的推荐。
- 推荐系统通常根据系统的输入分为两大类：
	- 基于内容。这一类推荐系统要求目标被一些特征和文字详细描述。因此，这些推荐系统需要用户告知他们不同类型的目标喜好的偏好。这个可以通过观察用户消费不同类型目标物品隐含地获取。
	- 基于协同过滤。这类推荐系统使用一个评分矩阵M对每一个用户提供关于他有多喜欢一些目标的信息。这类推荐系统
- 基于协同过滤的推荐系统可以根据推荐用户喜好所用的算法分为如下代表：
	- 基于记忆。
	- 基于模型。
- 在我们的论文中，我们提出一个分解评分矩阵的新方法，保持了经典的矩阵因式分解的优势。
	- 就像在经典的矩阵因式分解中，我们也考虑到了存在。。。
- 除了保持经典的矩阵因式分解的优势，我们的方法提供了额外的优势：
	- 在经典的矩阵因式分解算法中，矩阵因子可以是任意值，而我们的方法把它限制在[0,1]区间。
	- 区别于经典的矩阵因式分解。。。

#### 2.相关工作

#### 3.动机

#### 4.模型

- 本章我们将会提出本文的概率模型。4.1将会给出我们的方法的参数，输入和输出；4.2中我们提出关于用户评价目标的概率模型；4.3我们指出和我们模型相关的数学问题；4.4我们讨论分析算法的输出结果；4.5我们描述这个模型的学习算法；4.6我们最后指出方法的输出结果对模型参数的影响
- 4.1 我们的技术视图
	- 本章节我们提出算法的黑盒描述。这个算法对找到用户分享相同尝试的设置和预测一个用户喜欢一个目标的可能性很有用。
	- 输入
	- 参数 
---
# 其他资料及笔记

**协同过滤**：
- 协同过滤简单来说是利用某兴趣相投、拥有共同经验之群体的喜好来推荐用户感兴趣的信息，个人通过合作的机制给予信息相当程度的回应（如评分）并记录下来以达到过滤的目的进而帮助别人筛选信息，回应不一定局限于特别感兴趣的，特别不感兴趣信息的纪录也相当重要。
- 主要分为基于用户的协同过滤算法和基于物品的协同过滤算法。
	- 基于用户的协同过滤算法的关键是找到相同偏好的用户，找到了偏好最近的几个用户，他们偏好的物品便是要给你推荐的目标。
	- 基于物品的协同过滤算法的关键是计算其它物品和历史物品的相似度，相似度最近的几个物品便是要推荐的物品。
	- （换句话说，协同过滤算法的关键是解决**相似度问题**）。
	- 相似度计算主要有三个经典算法：余弦定理相似性度量、欧氏距离相似度度量和杰卡德相似性度量。
	- [一个协同过滤实现案例](https://blog.csdn.net/u012995888/article/details/79077681)

**矩阵因式分解**：
- 矩阵分解的思想很简单，对于用户-物品这个评分矩阵R，我们可以将其分解为用户-特性矩阵P，以及特性-物品矩阵Q。R=PQ。这样做的好处有两点： 
	- 1. 得到了用户的偏好，以及物品的特性 
	- 2. 降低了矩阵的维度。 

**疑问**：
- paper1 中的矩阵因式分解和SVD有什么区别？
	- 矩阵因式分解分为经典的矩阵因式分解和SVD等等
- 矩阵分解的方式有很多？包含paper3的非负矩阵因式分解，SVD奇异值分解等？
	- 是的

---
# 论文构想

5000 words TO 8000 words

- 加入评价文字的情感分析
- 爬取评分矩阵，获取情感分析矩阵，矩阵分解成向量，向量重新得到不再稀疏的评分结果，协同推荐相似度高用户和相似度高的目标
- 结果比对： 1. 相同数据集不同算法比较  2. 相同数据集不同算法比较，可比较多个算法











