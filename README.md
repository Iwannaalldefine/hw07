# 肺炎 X 光影像二分类实战 (Chest X-Ray Pneumonia Classification) 

《人工智能导论》课程作业 07 - 胸部 X 光肺炎影像二分类实战。
本项目基于深度学习技术，对 Kaggle 公开的儿童胸部 X 光数据集进行端到端分类（NORMAL vs PNEUMONIA）。

## 📂 目录结构说明

hw07/
├── train.ipynb        # 包含数据加载、模型构建、训练和评估的完整 Jupyter Notebook（含执行日志）
├── requirements.txt   # 项目依赖文件
├── README.md          # 项目运行说明书 (本文档)
├── report.md          # 核心实验报告及医学诊断降维分析
└── figures/           # 存放运行生成的训练曲线、混淆矩阵等截图

## 🛠️ 环境依赖 & 运行方式

**运行环境推荐：** Kaggle Notebook (强烈推荐，免下载数据，免费 GPU)

**依赖包 (requirements.txt):**
- torch
- torchvision
- matplotlib
- seaborn
- scikit-learn

**一键运行指南（Kaggle）：**
1. 登录 Kaggle，新建 Notebook，开启 `GPU T4 x2` 算力，并在设置中开启 `Internet`。
2. 点击右上角 `Add Data`，搜索并挂载数据集 `Chest X-Ray Images (Pneumonia)` (提供方: Paul Mooney)。
3. 导入本仓库中的 `train.ipynb` 文件，点击 `Run All` 即可一键复现全部结果。

## 📊 核心指标摘要 (测试集)
- **总体准确率 (Accuracy):** 82.85%
- **肺炎类别召回率 (Pneumonia Recall):** 97.44% (临床极佳表现)
- **漏诊病例 (False Negative):** 仅 10 例 (占比极低)