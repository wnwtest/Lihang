# 统计学习方法
## 前言
- 每个人都有适合自己的理解方式, 对同样的内容, 会有不同的理解
- 书如数据, 学如训练, 人即模型.

如果用我这个模型来实现相似度查找, 和李老师这本书神似的就是<半导体光电器件>了, 只可惜昔时年少, 未曾反复研读.

希望在反复研读的过程中, 将整个这本书看厚, 变薄.  
## CH2 感知机
[Perceptron](CH2/README.md)
- 感知机是二类分类的线性分类模型
- 感知机对应于特征空间中将实例划分为正负两类的分离超平面.
## CH3 k近邻法
[kNN](CH3/README.md)
- kNN是一种基本的分类与回归方法
- k值的选择, 距离度量及分类决策规则是kNN的三个基本要素.
## CH4 朴素贝叶斯法
[NB](CH4/README.md)
- 朴素贝叶斯法是基于贝叶斯定理与特征条件独立假设的分类方法.
1. IID->输入输出的联合概率分布
1. Bayes->后验概率最大的输出
- x的某种组合在先验中没有出现的情况, 会出现概率为0的情况, 对应平滑处理方案
$$P_\lambda(X^{(j)}=a_{jl}|Y=c_k)=\frac{\sum_{i=1}^{N}{I(x_i^{(j)}=a_{jl}, y_i=c_k)}+\lambda}{\sum_{i=1}^{N}{I(y_i=c_k)+S_j\lambda}}$$
1. lambda = 0 对应极大似然估计
1. lambda = 1 对应拉普拉斯平滑

## CH5 决策树
[Decision Tree](CH5/README.md)
- 决策树是一种基本的分类与回归方法
## CH6 逻辑斯谛回归与最大熵模型

[Logistic Regression and Maximum Entropy](CH6/README.md)
- 逻辑斯谛回归是统计学中的经典分类方法
- 最大熵是概率模型学习的一个准则, 将其推广到分类问题得到最大熵模型
为什么LR和ME要放在一章
- 都属于对数线性模型
- 都可用于二分类和多分类
- 两种模型的学习方法一般采用极大似然估计, 或正则化的极大似然估计. 可以形式化为无约束最优化问题, 求解方法有IIS, GD, BFGS等.

## CH7 支持向量机

[Support Vector Machines, SVM](CH7/README.md)

- 支持向量机是一种二分类模型.
- 基本模型是定义在特征空间上的间隔最大化的线性分类器, 间隔最大使他有别于[感知机](CH2/README.md)

## CH8 提升方法
[Boosting](CH8/README.md)
- 提升方法是一种常用的统计学习方法, 应用广泛且有效.

## CH12 统计学习方法总结
[Summary](CH12/README.md)

这章就简单的几页, 可以考虑如下阅读套路
1. 和第一章一起看
1. 在前面的学习中遇到不清楚的问题的时候, 过一遍这个章节.
1. 将这一章看厚, 从这一章展开到其他十个章节. 
李老师这本书真的是每次刷都会有新的收获.
