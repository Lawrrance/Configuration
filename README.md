# Configuration
To introduce configurations about DL project.

https://github.com/ChenyangLEI/Fully-Automatic-Video-Colorization-with-Self-Regularization-and-Diversity
# Guide 指南
# Warnning ：注意选择经过测试的构建配置 
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
更换512GB固态硬盘，划分盘符安装Win10，ubuntu双系统
### 1.Ubuntu 18 

      1.与win boot共存 
https://zhuanlan.zhihu.com/p/81961750
  
      2.安装输入法，浏览器，WPS
  
      3.安装显卡驱动 
      
https://zhuanlan.zhihu.com/p/59618999
  
### 2.Anaconda & Spyder
	流程参考
	https://blog.csdn.net/u012243626/article/details/82469174 
	Anaconda安装
	https://docs.anaconda.com/anaconda/

      安装图形界面
      
            conda install -c anaconda anaconda-navigator
            anaconda-navigator
            conda update     # 更新组件
	    
      安装桌面图标
	
#### Q:在Terminal中输入Python，调用的是系统自带的Py2.7
	A:Anaconda Initiate将环境变量复位了
	配置anaconda环境：
	vim ~/.bashrc
	最后一行添加：export PATH=/home/XXX/anaconda3/bin:$PATH
	XXX是你的用户名
	保存并： source ~/.bashrc
            
            
          
            
### 3.TensorFlow & OpenCV
https://blog.csdn.net/qq_31610789/article/details/80642709 Tensor安装
### 4.Cuda & Cudnn
官方安装CUAD

https://developer.nvidia.com/cuda-downloads?target_os=Linux&target_arch=x86_64&target_distro=Ubuntu&target_version=1804&target_type=deblocal

验证CUDA

https://www.jianshu.com/p/dbeb1f806e7d

官方安装CUDnn

https://docs.nvidia.com/deeplearning/sdk/cudnn-install/index.html#install-linux

#### Q.权限更改 ChangeMod
	https://www.twblogs.net/a/5d49ce77bd9eee5327fbd676/zh-cn
#### Q.验证过程中，在/usr/src中未找到Nvidia samples
	在官方下载页面另外下载 cuDNN Code Samples and User Guide for Ubuntu18.04 (Deb)
	https://askubuntu.com/questions/1021837/cuda-and-cudnn-install-where-is-cudnn-samples-v7
### 5.Shadowsocks

Usage:
      
http://m.knowsky.com/990432.html

主要步骤：
       
https://segmentfault.com/a/1190000011224139

Official Tutorial

Installation:
https://shadowsockshelp.github.io/Shadowsocks/linux.html

Browser Config:
https://shadowsockshelp.github.io/Shadowsocks/Firefox.html
