---
layout: page
title: NN Regularization
---
正则化（Regularization）的目的是为了防止过拟合，即为了防止学习模型只是对训练集有很好的表现，而对其他不在训练集的样本则效果不好。

#### __Dropout__
---
[Geoffrey E. Hinton](http://www.cs.toronto.edu/~hinton/)组于2012年的文章[1]与[2]      
__训练时__    
就是一层的某个元素的值保留的概率为P，其为0的概率为1-P。具体可以表述为如下公式：     
$$\hspace{4mm}o=M * a(...) \\
\hspace{8mm}* -- 表示两个向量的中对应的元素相乘 \\
\hspace{8mm}a()-- active function \\
\hspace{8mm}M -- 元素为0 or 1的向量  \\
$$    
__检测时__   
需要将加了的dropout的层的输出乘以(1-P)。`或者在训练的时候乘以1/(1-P)，检测的时候则不用进行处理(见文章[3])`        
__注意__：在预学习中使用dropout的时候，也需要将输出放大回来，即乘以1/(1-P)    

#### __DropConnect__  
---    
coming soon    

#### __References__
---
1.  Improving neural networks by preventing co-adaptation of feature detectors
2.  Dropout: A Simple Way to Prevent Neural Networks from Overfitting
3.  Improving deep neural networks for LVCSR using rectified linear units and dropout

