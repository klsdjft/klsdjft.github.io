---
layout:     post                    # 使用的布局（不需要改）
title:      2020-SOTA-DL            # 标题 
subtitle:                           # 副标题
date:       2020-01-31              # 时间
author:     BY                      # 作者
header-img: img/post-bg-2015.jpg    #这篇文章标题背景图片
catalog: true                       # 是否归档
tags:                               #标签
    - Deep Learning
    - Computer Vision
    - Autopilot
---
# Deep Learning State of the Art (2020) | MIT Deep Learning Series

Original video:

[Deep Learning State of the Art (2020) | MIT Deep Learning Series](https://www.youtube.com/watch?v=0VH1Lim8gL8)

## Active Learning Pipeline

![Active_Learning_Pipeline](img/pics/Active_Learning_Pipeline.png)

One of the ideas mentioned here is "Search for Others Like it", which means that our SOTA model needs to clean up the scene in the previous step "Discover Edge Case". Like: **Find a scene of a blue bicycle or two people walking side by side.** This will be a challenge for data cleansing systems.

## Single-Task and Multi-Task Learning

![Single_task_learning](img/pics/Single_task_learning.png)

> So most papers are written on single task learning. You take whatever benchmark here in the case of driving is object detection, landmark detection, drivable area, trajectory generation, right? All those have benchmarks.

![multi_task_learning](img/pics/multi_task_learning.png)

> But combing to use a single neural network that performs all those tests together, that's the fascinating challenge where you're reusing parts of the neural network to learn things that  are coupled. And then to learn things that are completely independent and doing the continuous active learning loop.

## Collaborative Deep Learning

> They're inside companies in the case of Tesla and Waymo in general, it's exciting to have people, these are actual human beings that are responsible for these particular tasks that become experts of particular perception task, expert at a particular planning task and so on. **And so the job of that expert is both to train the neural network and to discover the edge cases which maximize the improvement of the network.** 

![collaborative_Deep_Learning](img/pics/collaborative_Deep_Learning.png)

**An expert need to train the neural network and discover the special cases which maximize the improvement of the network.**