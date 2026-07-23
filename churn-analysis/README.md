# 在线教育平台用户流失分析

## 项目简介
基于800名在线学习用户的数据，通过Python数据分析和Power BI可视化，识别流失风险因素并提出业务建议。

## 技术栈
- Python: Pandas, Matplotlib, Seaborn, Scikit-learn
- Power BI: 数据可视化与仪表盘搭建
- Jupyter Notebook: 交互式数据分析

## 核心发现
1. **学习时长是流失核心预警指标**：高风险用户平均学习时长（158小时）显著低于低风险用户（202小时）
2. **完课率比学习时长更能预测流失**：逻辑回归模型显示完课率系数为-0.62，是最强预测因子
3. **城市等级不影响学习效果**：一至四线城市用户平均分数差异小于1分
4. **VIP权益未能激励学习**：VIP与非VIP学习时长差异仅6小时

## 业务建议
1. 建立学习时长预警机制，对连续低时长用户自动触发督学提醒
2. 优化VIP权益体系，增加专属学习路径和1v1答疑
3. 重点运营三四线城市，加大下沉市场推广

## 文件说明
| 文件 | 内容 |
|------|------|
| `online_education_analysis.ipynb` | Python数据分析完整流程（EDA + 建模） |
| `Education_Churn_Analysis.pbix` | Power BI仪表盘（3页：概览/画像/预警） |
| `online_education_data.csv` | 原始数据集（800行×14列） |

## 复现方式
```bash
# 安装依赖
pip install pandas numpy matplotlib seaborn scikit-learn

# 启动Jupyter
jupyter notebook online_education_analysis.ipynb