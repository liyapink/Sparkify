# Sparkify
P8 Udacity

## 文件
<b> Notebook Sparkify-zh.ipynb
<b> Readme Readme.md
<b> Blog.pdf
  
## 项目概述
预测客户流失率是数据科学家和分析师在面向消费者的一类公司中经常遇到的一项具有挑战性的问题。本项目中，我们使用音乐云服务Sparkify的日志数据进行探索。

这里我们定义最终取消服务（即`Cancellation Confirmation`事件）的用户为流失用户，首先使用可视化等方法进行初步评估，然后使用 Spark 来抽取相关性特征，使用多个机器学习模型及不同参数进行训练，以对客户流失率作出预测。

因为流失客户数据集很小，我们选用 F1 score 作为优化指标。
最终我们训练得出的最好结果是 F1-Score = 0.758, 这一结果优于 baseline (即预测所有用户都不流失) 的分数0.680

### 数据来源
Sparkify的日志数据集。完整的数据集大小为 12GB，这里我使用了它的一个约定128GM的迷你子集来进行分析。

### 主要依赖库
PySpark.sql, PySpark.ml, Pandas, Matplotlot.pylpot, Seaborn

### 机器学习模型
Logistic Regression, Gradient Boosted Trees, Support Vector Machines, Random Forest

### 参考
