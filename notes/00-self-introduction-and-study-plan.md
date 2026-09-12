# 自我介绍与学习计划

## 1. 自我介绍

我具有数学专业本科背景，目前开始系统学习 Python、深度学习和图像处理。我的主要研究兴趣是显微图像复原与计算成像，希望将数学理论、传统图像处理方法与深度学习方法结合起来。

现阶段的主要目标是掌握深度学习基础，并逐步完成 SN2N 项目的代码阅读、环境配置、实验复现和结果分析。

## 2. 当前开发环境

| 项目 | 当前配置 |
|---|---|
| 操作系统 | Windows |
| Python 环境 | Conda：dl-env |
| Python 版本 | 3.10.21 |
| 显卡 | NVIDIA GeForce RTX 5060 Ti |
| 开发工具 | VS Code、Jupyter |
| 版本管理 | Git、GitHub |

## 3. 学习计划

| 阶段 | 主要内容 | 预期成果 |
|---|---|---|
| 第一阶段 | Python、NumPy、Matplotlib | 能够独立完成数据处理和绘图 |
| 第二阶段 | PyTorch 与神经网络基础 | 完成基础网络训练实验 |
| 第三阶段 | 图像去噪与自监督学习 | 理解常见去噪方法 |
| 第四阶段 | 阅读并运行 SN2N | 成功复现实验结果 |
| 第五阶段 | 分析和改进实验 | 整理实验记录与研究总结 |

## 4. Python 环境测试

```python
import sys
import numpy as np

print("Python版本：", sys.version)
print("NumPy版本：", np.__version__)
```

## 5. 图像质量评价公式

均方误差（MSE）定义为：

$$
\mathrm{MSE}=\frac{1}{MN}\sum_{i=1}^{M}\sum_{j=1}^{N}
\left[I(i,j)-K(i,j)\right]^2
$$

峰值信噪比（PSNR）定义为：

$$
\mathrm{PSNR}=10\log_{10}\left(\frac{L^2}{\mathrm{MSE}}\right)
$$

二维离散卷积可以表示为：

$$
y(i,j)=\sum_m\sum_n x(m,n)h(i-m,j-n)
$$

其中，$I$ 表示参考图像，$K$ 表示待评价图像，$L$ 表示图像像素的最大可能取值，$h$ 表示卷积核。

## 6. 阶段目标

- 熟练使用 Conda、VS Code、Jupyter 和 Git。
- 掌握 PyTorch 的基本使用方法。
- 理解卷积神经网络与图像去噪原理。
- 能够阅读并调试深度学习项目代码。
- 完成 SN2N 项目的复现与实验记录。