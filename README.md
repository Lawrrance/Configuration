# Configuration
To introduce configurations about DL project.

https://github.com/ChenyangLEI/Fully-Automatic-Video-Colorization-with-Self-Regularization-and-Diversity
# Guide 指南
## Requirement 要求
Ubuntu 16.04

tensorflow 1.2.0

OpenCV 3.4.2.16

Cuda 8.0 

cudnn 7.0
## Installation 安装
更换512GB固态硬盘，划分盘符安装Win10，ubuntu双系统
### 1.Ubuntu 16

      1.与win boot共存 
https://zhuanlan.zhihu.com/p/81961750
  
      2.安装输入法，浏览器，WPS
  
      3.安装显卡驱动 
      
https://zhuanlan.zhihu.com/p/59618999
  
### 2.Anaconda & Spyder

https://blog.csdn.net/u012243626/article/details/82469174 Anaconda安装

      安装图形界面
      
            conda install -c anaconda anaconda-navigator
            anaconda-navigator
            conda update     # 更新组件
      安装桌面图标
	
### Q:在Terminal中输入Python，调用的是系统自带的Py2.7
	A:Anaconda Initiate将环境变量复位了
	配置anaconda环境：
	vim ~/.bashrc
	最后一行添加：export PATH=/home/XXX/anaconda3/bin:$PATH
	XXX是你的用户名
	保存并： source ~/.bashrc
            
            
          
            
### 3.TensorFlow & OpenCV
https://blog.csdn.net/qq_31610789/article/details/80642709 Tensor安装
### 4.Cuda & Cudnn
https://developer.nvidia.com/cuda-downloads?target_os=Linux&target_arch=x86_64&target_distro=Ubuntu&target_version=1804&target_type=deblocal
### 5.Shadowsocks

Usage:
      
http://m.knowsky.com/990432.html
       
https://segmentfault.com/a/1190000011224139

Official Tutorial

Installation:
https://shadowsockshelp.github.io/Shadowsocks/linux.html

Browser Config:
https://shadowsockshelp.github.io/Shadowsocks/Firefox.html
