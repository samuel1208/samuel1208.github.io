---
layout: page
title: Fourier Transformation
---
傅立叶变换在信号处理以及图像处理中出现的频率实在太高，高的实在是忍不住了，遂整理一下。

#### __傅立叶级数__
---    
法国数学家傅里叶发现，任何周期函数都可以用正弦函数和余弦函数构成的无穷级数来表示（选择正弦函数与余弦函数作为基函数是因为它们是正交的），后世称傅里叶级数为一种特殊的三角级数。即：    
给定一个`周期为T`的函数x(t),那么它可以表示为无穷级数：    
$$
\hspace{8mm}x(t) = \sum_{k=-\infty}^{\infty} a_ke^{jk(\frac{2\pi}{T})t}   \hspace{16mm}(1)\\
\hspace{16mm}其中： \hspace{4mm}a_k = \frac{1}{T}\int_T x(t)e^{-jk(\frac{2\pi}{T})t}dt   \hspace{16mm}(2)
$$    
1. 注意$$a_k$$中的积分范围是`一个周期`    
2. 注意到$$e^{jk(\frac{2\pi}{T})t}$$是`周期为T的函数`。故k取不同值时的周期信号具有谐波关系(`即它们都具有一个共同周期T`)。k=0时，称为直流分量，k=1时具有基波频率称为一次谐波或基波，类似的有二次谐波，三次谐波等等    
<br/>    

#### __傅立叶变换__
---    
*  __连续形式__    
$$
F(w) = \mathscr{F}[f(t)] = \int^{\infty}_{-\infty}{f(t)e^{-iwt}dt}    \\
f(t) = \mathscr{F}^{-1}[F(w)] = \frac{1}{2\pi}\int^{\infty}_{-\infty}{F(w)e^{iwt}dw}    
$$
*  __离散形式__    
$$
$$
