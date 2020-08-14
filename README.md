# Sparkify - 在线音乐服务用户流失分析
UDACITY 数据挖掘直通车纳米学位 Project 8

## 文件
<b> Notebook Sparkify-zh.ipynb 主程序文档  
<b> mini_sparkify_event_data.json Sparkify 日志文件（迷你子集）  
<b> Blog.pdf blog文件
  
## 项目概述
预测客户流失率是数据科学家和分析师在面向消费者的一类公司中经常遇到的一项具有挑战性的问题。

本项目中，我们使用在线音乐服务Sparkify的日志数据进行探索。

这里我们定义最终取消服务（即`Cancellation Confirmation`事件）的用户为流失用户。

我们的目标是从日志数据中抽取特征以建立一个模型，并拿它来预测测试集中的用户标签（churn），并和实际的标签对比。如果预测的结果至少优于我们设置的基线值（Baseline），我们就可以认为这个模型是有用的。而若能得出有效预测，Sparkify平台就能够赶在用户取消服务之前给他们提供折扣或激励，以此降低流失率。

在探索性数据分析阶段，我们将主要使用可视化的方法对可能的影响因素逐一分析，以期找出流失和非流失用户表现不同的因素以作为候选特征。最后我们使用逻辑回归等多个机器学习模型，在训练集和验证集上进行训练，并对比训练结果（考虑到需要兼顾准确率和召回率，我们选用F1-Score为主要参考指标）。

最终我们训练得出的最好结果是 F1-Score = 0.790, 这一结果优于 baseline (即预测所有用户都不流失) 的分数0.681，模型是有效的。

## 数据来源
Sparkify的日志数据集。完整的数据集大小为 12GB，这里我使用了它的一个 128MB 大小的迷你子集来进行分析。

## 主要依赖库
PySpark.sql, PySpark.ml, Pandas, Matplotlot.pylpot, Seaborn

## 机器学习模型
Logistic Regression, Gradient Boosted Trees, Support Vector Machines, Random Forest

## 参考
https://github.com/linpingyu/Sparkify
https://blog.csdn.net/SunflowerLuck/article/details/82822930
