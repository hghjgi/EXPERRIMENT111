# 实验一：计算机视觉库的安装
2024410315019-彭艺琼

## 一、实验目的
掌握Anaconda的安装与基本操作，熟悉GPU使用环境的配置及对应版本PyTorch的安装，并完成OpenCV的安装与配置。
## 二、实验内容
### 1、Anaconda的安装及配置
打开Anaconda Prompt终端进行操作，
- 查看conda版本 <br>
- 查看conda配置信息 <br>
```bash
conda --version
conda config --show
```
结果图：<br>

### 2、conda的基本操作与OpenCV的安装
- 创建虚拟环境并制定python版本 <br>
- 进入创建的虚拟环境，安装OpenCV <br>
```bash
conda create -n cv python==3.10
activate cv
pip install opencv-python
```
### 3、GPU加速环境配置
 显示显卡状态信息
```bash
nvidia-smi
```

### 4、PyTorch安装
结合CUDA版本至PyTorch官网选择对应版本进行下载
### 5、PyTorch GPU加速环境验证
torch.cuda.is_available() 、torch.backends.cudnn.is_available() 结果进行验证
