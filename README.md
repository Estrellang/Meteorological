# Meteorological

本项目为《气象遥感大数据挖掘》课程的实验报告/研究分析，使用 Python（xarray、NumPy、Matplotlib 等）处理并分析气象遥感数据。主要分析内容围绕欧洲地区多个典型城市的气象要素演变与趋势，涵盖数据合并、清洗、可视化等多个步骤。

## 📁 项目结构

```
Big Data.ipynb               # 主实验分析文件（Jupyter Notebook）
data/
└── data_stream-oper_stepType-accum.nc   # 累积型气象数据
└── data_stream-oper_stepType-instant.nc # 瞬时型气象数据
```

## 📌 核心内容

Notebook 中按步骤详细组织：

1. **数据合并与基本信息查看**
   加载两类 NetCDF 格式气象数据，并合并为一个整体数据集 `ds_combined`。

2. **选取典型城市（如巴黎）进行分析**
   基于地理坐标选择格点，聚焦具体城市的时间序列分析。

3. **数据预处理与单位转换**
   包括单位标准化（如从 Pa 转换为 hPa）、数据缺失处理等。

4. **变量可视化**
   使用 Matplotlib 绘图，包括降水量、温度、气压等随时间变化的趋势图。

5. **简单的异常检测与趋势分析**
   识别极端事件并可视化展示。

## 🛠 使用环境

建议使用如下 Python 环境：

```bash
Python >= 3.8
xarray >= 2023.1
numpy >= 1.21
matplotlib >= 3.4
netCDF4 >= 1.5
```

安装依赖：

```bash
pip install xarray numpy matplotlib netCDF4
```

## 📈 数据说明

* 数据格式：NetCDF
* 数据区域：欧洲大陆
* 时间范围：2020 年某时段
* 气象要素：降水、温度、气压、风速等

## 📚 适用场景

* 气象数据分析课程实验
* 遥感与大数据挖掘相关研究
* 使用 Python 和 xarray 进行空间时间数据探索的入门实践


---


