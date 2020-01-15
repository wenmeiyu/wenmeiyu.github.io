---
layout:     post
title:      python程序编译成exe可执行文件
subtitle:   python程序编译成exe可执行文件
date:       2020-01-14
author:     wenmeiyu
header-img: img/post-bg-ios9-web.jpg
catalog: true
tags:
    - python程序编译成exe
---

# 参考资料

>[将python程序打包成exe( pyintaller) 的用法](https://www.cnblogs.com/jingzeng/p/10241724.html)

>[怎么把python代码打包成exe文件](https://jingyan.baidu.com/article/14bd256e948da6bb6d2612b5.html)

>[Python如何将py文件打包成exe](https://www.cnblogs.com/smart-zihan/p/11881172.html)

## 安装

- 直接使用pip安装
	```
	pip install pyinstaller
	```
	- `pyinstaller -v`验证是否安装成功

## python程序编译成exe

- 运行如下命令把test.py文件编译成exe可执行文件
    ```
	pyinstaller -F test.py
    ```
	- 执行之后test.py文件文件目录下新生成dist文件夹，文件夹下的exe文件双击即可运行

