# Datasets-of-Electricity-Theft-Detection
This is a collection of public datasets that can be used for electricity theft detection, which I collected from other papers and public repositories. This might be work when you have trouble with electricity datasets. 

**NOTE**: This repository exists for navigation only and _**DOES NOT**_ directly provide source datasets.

这是一组可以用于窃电检测的公共数据集集合，由我从窃电检测相关论文与公共仓库中收集而来。如果您在电力数据集方面遇到了困难，这些数据集可能会有所帮助。本仓库仅供导航使用，不直接提供源数据集。
# Household Power Consumption Dataset (HPCD)
来自 [HPCD](https://github.com/PranayKr/Smart-Meter-Data-Analytics) 。

HPCD是电力相关变量的多变量时间序列数据集，用于描述单个家庭四年的用电量。数据是在2006年12月至2010年11月期间收集的，每分钟收集一次家庭用电量的观察结果。它是一个多变量序列，由七个变量组成，分别为：

* global active power：家庭消耗的总有功功率（千瓦）。
* global reactive power：家庭消耗的总无功功率（千瓦）。 
* voltage：平均电压（伏特）。 
* global intensity：平均电流强度（安培）。 
* sub metering 1：厨房的有功电能（有功电的瓦时）。 
* sub metering 2：洗衣的有功电能（有功电瓦时）。 
* sub metering 3：气候控制系统的有功电能（有功电瓦时）。

**关键词：单用户 多维度 无异常标签**
# Electricity Consumption Dataset of State Grid Corporation of China (SGCC)
来自 [SGCC](https://github.com/henryRDlab/ElectricityTheftDetection) ，在论文 [_Wide and Deep Convolutional Neural Networks for Electricity-Theft Detection to Secure Smart Grids, TII 2017_](https://ieeexplore.ieee.org/abstract/document/8233155/) 中使用。

这是中国国家电网公司发布的现实用电量数据集。本数据集包含2014年1月1日至2016年10月31日1035天内 42372 个用电客户的用电量数据，带有真实异常标签。这是目前窃电检测最广泛使用的数据集，因为其存在的标注标签。

**关键词：多用户 单维度 有异常标签**
# Electricity Transformer Dataset (ETDataset)
来自 [ETDatase](https://github.com/zhouhaoyi/ETDataset?tab=readme-ov-file) ，在论文 [_Informer: Beyond Efficient Transformer for Long Sequence Time-Series Forecasting, AAAI 2021_](https://arxiv.org/abs/2012.07436) 中使用。

作者只公开了数据集的small版本，包含 2 台变压器在 2 个站点的数据，包括负载、油温等多个维度。数据的记录时间横跨两年，分为两个部分：
* 其中每个数据点每分钟记录一次（用 m 标记），它们来自中国一个省的两个地区，分别命名为 ETT-small-m1 和 ETT-small-m2。每个数据集包含 2 年* 365 天* 24 小时* 4 次 = 70080 个数据点。
* 此外，作者还提供了用于快速开发的每小时级别变体（以h标记记），即 ETT-small-h1 和 ETT-small-h2。每个数据点由 8 个特征组成，包括点的日期、预测值“油温”和 6 种不同类型的外部电源负载特征。

**关键词：多用户 多维度 无异常标签**
# Climate reanalysis datasets
来自 [Climate reanalysis datasets](https://github.com/energy-modelling-toolkit/climate-driven-energy-datasets) 。

作者列出了一些免费提供的基于气候再分析或气候变化预测的能源变量（其中涉及**电力需求**）重建数据集的列表。

**关键词：数据集集合**
# Smart Energy Meters in Bangalore India (SEMBI)
来自[Smart Energy Meters in Bangalore India](https://www.kaggle.com/datasets/unseemlycoder/smart-energy-meters-in-bangalore-india)。数据集过大，还没来得及研究。

# Electricity Theft Data on Kaggle (ETD on kaggle)
来自[Electricity Theft Data by Avin Joseph](https://www.kaggle.com/datasets/avinemmatty/theft-data/data)。

数据集格式与SGCC类似，包含窃电标签。但**数据可信度存疑**，其出现了**过于久远和未来的用电数据**，仅供参考。

**关键词：多用户 单维度 有异常标签**
# Theft Detection in Smart Grid Environment (TDSGE)
来自 [Theft detection in smart grid environment](https://data.mendeley.com/datasets/c3c7329tjj/1) ，在论文[_Theft detection dataset for benchmarking and machine learning based classification in a smart grid environment_](https://www.sciencedirect.com/science/article/pii/S1319157822001562?ref=pdf_download&fr=RR-2&rr=87a79bc1ea43d5fd) 中被提出。

该数据集包含 16 种不同类型消费者的能源消耗。原始数据包括多个客户一年（12 个月）的多个能耗测量值。每小时进行一次测量。  
六种不同类型的欺诈被添加到原始数据集中。它们由一些消费者可能造成的不同类型的盗窃组成。第一种盗窃包括白天的电力消耗大幅减少。通过将消耗量乘以 0.1 到 0.8 之间的随机选择值来计算此减少量。在第二种类型的盗窃中，电力消耗在任意时间段内随机下降到零。第三种类型的盗窃与第一种类型类似，但每个消耗值（每小时）乘以一个随机数。为第四种类型的盗窃生成平均消耗的随机部分。第五种类型报告平均消耗量，最后一种类型（即第六种类型）颠倒了读数顺序。  
原始数据是从开放能源数据倡议 （OEDI） 平台收集的。它是从美国能源部的项目、办公室和国家实验室汇总的高价值能源研究数据集的集中存储库。

该数据集包含异常标签，涉及多用户与多变量，但时间序列的标注很模糊。
**关键词：多用户 多维度 有异常标签**
