#  **《数字图像处理》课程综合项目**——**基于多种滤波器的图像去噪算法比较与分析**

## GUI界面：

![digital_image_GUI](https://cdn.jsdelivr.net/gh/kennems/blog-image/digital_image_GUI.gif)

本项目源代码和报告均在仓库中。

## 项目简介

本项目旨在设计一个基于Matlab的图像去噪GUI系统，通过应用多种图像去噪算法，提高图像的质量和可用性。该系统集成了多种经典和现代的去噪方法，并提供了直观的用户界面，方便用户对图像进行去噪处理和效果评估。

## 主要功能概述

### 1. 图像去噪方法
系统实现了多种常见的图像去噪方法，包括：

- **均值滤波**：通过邻域像素的平均值来替代中心像素的值，有效减少高频噪声，但可能导致图像细节丢失 。
- **中值滤波**：采用滤波窗口内像素的中值替代中心像素的值，能够有效去除椒盐噪声和脉冲噪声，同时保留图像边缘和细节信息 。
- **高斯低通滤波**：利用高斯函数对图像进行低通滤波，平滑图像并减少噪声 。
- **巴特沃斯低通滤波**：一种频域滤波方法，适用于去除频率较高的噪声 。
- **小波变换**：通过小波分解和重构来实现图像去噪，能够有效保留图像的细节和边缘 。
- **非局部均值去噪**：基于图像中相似区域的像素值信息，对目标像素进行加权平均，保留图像细节但计算复杂度较高 。
- **维纳滤波**：基于最小均方误差准则，恢复由噪声污染的图像，效果显著但需预估噪声性质 。
- **同态滤波**：结合对数变换和频域滤波，增强图像对比度，去除光照变化和噪声 。

### 2. 图像噪声添加
系统支持多种噪声类型的添加，以模拟实际应用中的噪声环境，包括高斯噪声、椒盐噪声、泊松噪声和运动噪声等 。

### 3. 去噪效果评估
提供了多种图像质量评价指标，包括峰值信噪比（PSNR）、均方误差（MSE）、信噪比（SNR）和结构相似性指数（SSIM）等，帮助用户客观比较不同去噪算法的性能 。

### 4. 用户界面
系统采用Matlab GUI设计，用户可以通过界面选择去噪方法、设置相关参数、添加噪声以及查看去噪效果图，操作简便直观 。

## 结论

本项目设计的数字图像处理GUI系统，通过集成多种图像去噪方法和提供直观的用户界面，方便用户进行图像去噪处理和效果评估。该系统具有重要的理论意义和实际应用价值，为推动数字图像处理技术的进步和满足实际应用需求提供了有力支持。