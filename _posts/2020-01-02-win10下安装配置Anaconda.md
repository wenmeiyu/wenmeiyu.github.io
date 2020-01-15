---
layout:     post
title:      win10下安装配置Anaconda
subtitle:   win10下安装配置Anaconda
date:       2020-01-02
author:     wenmeiyu
header-img: img/post-bg-ios9-web.jpg
catalog: true
tags:
    - Anaconda
---

# 参考资料

>[官网下载地址](https://www.anaconda.com/distribution/#download)

>[清华镜像源下载地址](https://mirrors.tuna.tsinghua.edu.cn/anaconda/archive/)

>[windows10下anaconda3 5.3.0 安装教程](https://blog.csdn.net/a491945375/article/details/83758424)

## 下载

- 建议采用[清华镜像源下载地址](https://mirrors.tuna.tsinghua.edu.cn/anaconda/archive/)下载，速度比较快

## 安装

- 直接双击下载的exe文件，下一步一直到安装完成Finish

## 配置环境变量

- 把如下路径加入环境变量path

```
C:\ProgramData\Anaconda3
C:\ProgramData\Anaconda3\Library\mingw-w64\bin
C:\ProgramData\Anaconda3\Library\bin
C:\ProgramData\Anaconda3\Scripts
```

## 验证及简单命令

- 验证：
	- 输入`conda info`出现版本信息
- 常用命令：
	- `conda install packagename==1.0.1` #安装相应版本包
	- `conda activate tensorflow` #激活tensorflow环境，命令完成后，回答先命令行之前多了tensorflow
	- `source deactivate tensorflow` #退出名为tensorflow环境，回到系统默认环境
	- `conda info -e` #查看所安装环境列表，创建的环境都在~/anaconda3/envs/目录下面
	- `conda create -n [name]` #创建名为name的conda环境,如tensorflow
	- `conda remove -n [name] --all` #删除刚刚创建的conda环境??
	- `conda config --set auto_activate_base false` #设置Anaconda在新开的terminal里面不要自动进入虚拟环境base
	- `conda upgrade --all` #更新所有安装包
	- `conda create -n deeplearning python=3.6` #创建名为deeplearning的python版本为3.6的conda环境
	- `conda list`  #激活环境后查看该环境的环境包
