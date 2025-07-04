# BreastCancer-MultiModal-DL
# 多模态深度学习模型用于乳腺癌化疗疗效与毒性预测

本项目为论文“基于多模态深度学习的卷积与图网络模型预测乳腺癌化疗疗效与毒性风险的整合分析”的配套资源，提供部分图像数据处理流程和示意结果。

## 项目概述

本研究提出一种多模态深度学习框架，整合医学影像、临床信息与基因组数据，以预测乳腺癌患者化疗的疗效与毒性。本文主要构建了基于 CNN（卷积神经网络）和 GCN（图卷积神经网络）的特征提取与融合模型，在多个独立指标上表现出优越性能。

## 数据说明

本仓库中提供部分医学图像数据的预处理流程与示例，包括良性与恶性乳腺癌组织图像及其对应的分割掩码（mask）。数据结构如下：

```
--cancer_data
    --benign_imgs/
    --benign_mask/
    --malignant_imgs/
    --malignant_mask/
```

由于存储与伦理限制，图像数据已进行标准化处理，数量可能与文中描述略有出入。该部分数据主要用于图像分割模型的训练与可视化展示，并不包含患者的隐私信息或敏感基因数据。

## 基因与临床数据来源

由于原始基因组与临床数据未保留，本文所用基因组信息来自公开项目 **TCGA-BRCA（The Cancer Genome Atlas - Breast Invasive Carcinoma）**，该项目为公共数据库，涵盖约1,000例乳腺癌患者的基因表达、体细胞突变及详细的临床注释。研究者可通过如下链接获取相关数据：

👉 [TCGA-BRCA 数据集](https://portal.gdc.cancer.gov/projects/TCGA-BRCA)

## 代码说明

出于后续研究工作的连续性及项目依赖考虑，**完整的模型代码与多模态集成结构暂时不予公开**，待项目完成后将择期整理发布。

## 致谢

感谢 TCGA 及 GDC Portal 提供的开放数据支持。
