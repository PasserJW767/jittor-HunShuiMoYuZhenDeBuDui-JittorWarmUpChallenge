# Jittor-浑水摸鱼真的不队-计图挑战热身赛MNIST数字随机生成

![主要结果](https://www.gitlink.org.cn/api/liutongJ/jittor-pre-MNISTGeneration/raw/result.png?ref=master)

## 简介
本项目包含了第三届计图挑战赛计图 - MNIST数字随机生成的代码实现。本项目的特点是：采用了Conditional GAN方法对随机向量字符串处理，取得了随机字符串的图片，并达到97.11%的精度。

## 安装 

本项目可在 1 张 NVIDIA TITAN Xp 上运行，训练时间约为 0.5 小时。

#### 运行环境
- ubuntu 18.04
- python >= 3.7
- jittor >= 1.3.5

#### 安装依赖
执行以下命令安装 python 依赖
```
pip install -r requirements.txt
```

#### 预训练模型
预训练模型模型下载地址为链接：https://pan.baidu.com/s/1cSYwtWa5gCXjJDeiiGZoHw?pwd=wto4 ，下载后放入根目录下。

## 数据预处理
代码中集成了jittor对手写数据集MNIST的下载及预处理，无需进行手动操作

## 训练及推理
```
python CGAN.py
```

## 致谢

此项目基于论文 *Conditional generative adversarial nets* 实现，部分代码参考了 [jittor-gan](https://github.com/Jittor/gan-jittor)。