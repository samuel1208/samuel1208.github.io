---
layout: page
title: Mahalanobis Distance
---
马氏距离(不是[曼哈顿距离](./mahalanobis_dist.html#manhattan-distance))又称为Statistical Distance，两点间的马氏距离定义如下：            
$$
\hspace{8mm}d(p_1,p_2) = \sqrt{(p_1-p_2)^tS^{-1}(p_1-p_2)}     \\
\hspace{8mm}其中：    \\
\hspace{12mm}S为样本的协方差矩阵
$$       
    
* __与欧式距离的区别__      
![img](./img/mahlanobis.jpg)    

* __属性__    
1. 马氏距离的优点是它不受量纲的影响，即与原始数据的测量量纲单位无关。       
2. 马氏距离还可以排除变量之间的相关性的干扰。    
3. 马氏距离的缺点是夸大了变化微小的变量的作用。    
<br />

#### __曼哈顿距离(Manhattan Distance)__    
用以标明两个点在标准坐标系上的绝对轴距总和。如下图:    
![Manhattan](./img/manhattan.jpg)

图中红线代表曼哈顿距离(蓝色和黄色代表等价的曼哈顿距离)，绿色代表欧氏距离(直线距离)




