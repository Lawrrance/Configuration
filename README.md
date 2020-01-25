# Configuration
To introduce configurations about DL project.

https://github.com/ChenyangLEI/Fully-Automatic-Video-Colorization-with-Self-Regularization-and-Diversity
# Guide 指南
# Warnning ：注意选择对应版本！！！！
## 可用的版本搭配
	                        python                                   cuDNN   CUDA         
	tensorflow_gpu-1.5.0	2.7、3.3-3.6	GCC 4.8	 Bazel 0.8.0	7	9    # Recommendation
	tensorflow_gpu-1.4.0	2.7、3.3-3.6	GCC 4.8	 Bazel 0.5.4	6	8    # Recommendation
	tensorflow_gpu-1.13.1	2.7、3.3-3.6	GCC 4.8	Bazel 0.19.2	7.4	10.0
	tensorflow_gpu-1.12.0	2.7、3.3-3.6	GCC 4.8	Bazel 0.15.0	7	9
	tensorflow_gpu-1.11.0	2.7、3.3-3.6	GCC 4.8	Bazel 0.15.0	7	9
	tensorflow_gpu-1.10.0	2.7、3.3-3.6	GCC 4.8	Bazel 0.15.0	7	9
	tensorflow_gpu-1.9.0	2.7、3.3-3.6	GCC 4.8	Bazel 0.11.0	7	9
	tensorflow_gpu-1.8.0	2.7、3.3-3.6	GCC 4.8	Bazel 0.10.0	7	9
	tensorflow_gpu-1.7.0	2.7、3.3-3.6	GCC 4.8	Bazel 0.9.0	7	9
	tensorflow_gpu-1.6.0	2.7、3.3-3.6	GCC 4.8	Bazel 0.9.0	7	9
	tensorflow_gpu-1.5.0	2.7、3.3-3.6	GCC 4.8	Bazel 0.8.0	7	9
	tensorflow_gpu-1.4.0	2.7、3.3-3.6	GCC 4.8	Bazel 0.5.4	6	8
	tensorflow_gpu-1.3.0	2.7、3.3-3.6	GCC 4.8	Bazel 0.4.5	6	8
	tensorflow_gpu-1.2.0	2.7、3.3-3.6	GCC 4.8	Bazel 0.4.5	5.1	8
	tensorflow_gpu-1.1.0	2.7、3.3-3.6	GCC 4.8	Bazel 0.4.2	5.1	8
	tensorflow_gpu-1.0.0	2.7、3.3-3.6	GCC 4.8	Bazel 0.4.2	5.1	8

https://tensorflow.google.cn/install/source#linux

## Requirement 要求
Ubuntu 16.04

tensorflow 1.2.0

OpenCV 3.4.2.16

Cuda 8.0 

cudnn 7.0
## Installation 安装
### 1.Ubuntu 16.04

1.与win boot共存 
https://zhuanlan.zhihu.com/p/81961750
  
2.安装输入法，浏览器，WPS
  
3.安装显卡驱动 
https://zhuanlan.zhihu.com/p/59618999
      
4.备份
      
### 2.Cuda8 & Cudnn
选择版本，官方安装CUAD

https://developer.nvidia.com/cuda-toolkit-archive

安装显卡驱动

https://www.linuxidc.com/Linux/2018-09/154292.htm

安装多版本gcc

https://www.lagou.com/lgeduarticle/25406.html

配置CUDA环境变量

https://blog.csdn.net/QLULIBIN/article/details/80728355

验证CUDA

https://www.jianshu.com/p/dbeb1f806e7d

#### Q.权限更改 ChangeMod

https://www.twblogs.net/a/5d49ce77bd9eee5327fbd676/zh-cn

#### Q.验证过程中，在/usr/src中未找到Nvidia samples

在官方下载页面另外下载 cuDNN Code Samples and User Guide for Ubuntu18.04 (Deb)

https://askubuntu.com/questions/1021837/cuda-and-cudnn-install-where-is-cudnn-samples-v7      

官方安装CUDnn

https://developer.nvidia.com/rdp/cudnn-archive

https://docs.nvidia.com/deeplearning/sdk/cudnn-install/index.html#install-linux

#### Q.libcudnn.so.7 is not a symbolic link

https://devtalk.nvidia.com/default/topic/1032114/tensorrt/tensorrt-4-installation-libcudnn-so-7-is-not-a-symbolic-link/
          
### 3.TensorFlow & OpenCV

官方安装TF

https://tensorflow.google.cn/install/pip

## 注意：可以直接使用对应的python版本和pip版本安装（python3.4）

## e.g pip3 install tensorflow-gpu==1.2.0

安装Opcv

https://docs.opencv.org/3.4.2/d7/d9f/tutorial_linux_install.html

https://blog.csdn.net/cocoaqin/article/details/78163171

### 4.Shadowsocks

Usage:
      
http://m.knowsky.com/990432.html

主要步骤：
       
https://segmentfault.com/a/1190000011224139

Official Tutorial

Installation:
https://shadowsockshelp.github.io/Shadowsocks/linux.html

Browser Config:
https://shadowsockshelp.github.io/Shadowsocks/Firefox.html

## 注意：先要运行SS，测试延时，此外浏览器翻墙和终端翻墙要分别配置

# 测试项目

## 注意：使用python3解释器
1.下载并解压模型

python3 download_models.py

unzip ckpt_woflow.zip

2.运行测试

python main_woflow.py --model ckpt_woflow --use_gpu 1 --test_dir /PATH/TO/TEST/DIR

e.g.

python3 main_woflow.py --model ckpt_woflow --use_gpu 0 --test_dir test_sample0

（my GPU == Nvidia 960m ,gpu 0）

3.在./ckpt_woflow/ folder 查看结果

![result](https://user-images.githubusercontent.com/35630999/73123627-dce38d00-3fcc-11ea-877d-1195c51c668a.png)

