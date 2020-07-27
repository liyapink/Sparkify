# Sparkify
P8 Udacity

## 文件
<b> Notebook Sparkify-zh.ipynb
<b> Readme Readme.md
<b> Blog.pdf
  
## 项目概述
问题描述 评价指标
预测客户流失率是数据科学家和分析师在面向消费者的一类公司中经常遇到的一项具有挑战性的问题。还有，能用 Spark 高效处理大数据集是数据领域职位急需的一种能力。
学到如何用 Spark 操纵大的真实数据集来抽取相关性特征来预测客户流失情况
通过分析音乐云服务Sparkify的日志数据集, 预测客户流失率
完整的数据集大小为 12GB，你可以在下个页面的 workspace 中分析它的一个迷你子集。
Sparkify is a music streaming service just as Spotify and Pandora. The data provided is the user log of the service, having demographic info, user activities, timestamps and etc. We try to analyze the log and build a model to identify customers who are highly likely to quit using our service, and thus, send marketing offers to them to prevent them from churning. We use F1 score to measure of model performance because we need precision and recall at the same time as we don't want to miss too many customers who are likely to churn whilst we don't want to waste too much on those who are not likely to churn. The model we built has a F1 score of 0.800, which is 16% higher than sending everybody offers. There is also a short article about this project posted here.

### 数据来源
User log extracted from our service.

### 依赖库
PySpark, Pandas, Seaborn, Matplotlot.pylpot

### 机器学习模型
Logistic Regression, Gradient Boosted Trees, Support Vector Machines, Random Forest

### 参考
