#### $SU(2)$

$$
u=\begin{bmatrix}
 a & b\\
 c & d \end{bmatrix} ,\ also \ \ \  u=\begin{bmatrix}
 a & b\\
 -b^* & a^* \end{bmatrix}
$$

零迹厄米矩阵
$$
\sigma_1=\begin{bmatrix}
 0 &1 \\
 1 & 0 \end{bmatrix},\sigma_2=\begin{bmatrix}
 0 & -i\\
 i & 0 \end{bmatrix},\sigma_3=\begin{bmatrix}
 1 & 0\\
 0 & -1 \end{bmatrix}\\
 均为二阶零迹厄米矩阵：对角元必须为实数且和为0，非对角元实部相等，虚部相反\\
 因此这限制着三个实自由参数。\\
 \det =-1,1,-1\\
 \Tr = 0,0,0\\
 (*统一写在一起)
$$

$$
他们的任意线性组合也必须是二阶零迹的\\
h=x\sigma_1+y\sigma_2+z\sigma_3=\begin{bmatrix}
 z &x-iy \\
x+iy  & z \end{bmatrix}可以看作\vec{r}\cdot\vec{\sigma}
$$

https://zqw.ink/2020/05/20/SU2/

![image-20220105152830471](C:\Users\Wang Zhiyan\AppData\Roaming\Typora\typora-user-images\image-20220105152830471.png)

它与$SU(2)$的联系是什么呢？我们发现
$$
利用u的性质u^{\dagger}u=E给h构造相似变换，相似变换不改变迹（保持零迹），\dagger的性质保持厄米共轭性质\\
uhu^{-1}仍然是二阶零迹厄米\ \ \ (\ast \ u^\dagger=u^{-1})
$$
因此可以看作一种作用：
$$
uhu^{-1}=\begin{bmatrix}
 z' &x'-iy' \\
x'+iy'  & z' \end{bmatrix}
$$

![image-20220105153123279](C:\Users\Wang Zhiyan\AppData\Roaming\Typora\typora-user-images\image-20220105153123279.png)

这里有一个疑问，到底是$U^{-1}XU$还是$UXU^{-1}$？

从这里可以看到，群元和基底不是一个概念。

------

对形式
$$
u=\begin{bmatrix}
 a & b\\
 -b^* & a^* \end{bmatrix},\left\{\begin{matrix}
\ \ \ a=e^{i\alpha_3}(\cos\alpha_1 \cos \alpha_2+i\sin \alpha_1 \sin \alpha_2) \\
b=\cos\alpha_1 \sin \alpha_2+i\sin \alpha_1 \cos \alpha_2)
\end{matrix}\right.
$$
求得生成元
$$
I_1=\frac{\partial u }{\partial \alpha_1 } |_{\alpha_1=0}=\begin{bmatrix}
 0 &i \\
 i & 0 \end{bmatrix}=i\sigma_1,\\
 I_2=\frac{\partial u }{\partial \alpha_2 } |_{\alpha_2=0}=\begin{bmatrix}
 0 & 1\\
 -1 & 0 \end{bmatrix}=i\sigma_2,\\
 I_3=\frac{\partial u }{\partial \alpha_3 } |_{\alpha_3=0}=\begin{bmatrix}
 i & 0\\
 0 & -i \end{bmatrix}=i\sigma_3,
$$
如何理解呢？

1. 为什么有3个独立群参数？

![image-20220105153543134](C:\Users\Wang Zhiyan\AppData\Roaming\Typora\typora-user-images\image-20220105153543134.png)

2. 如何求得对易关系

泡利矩阵的性质：

![image-20220105153905041](C:\Users\Wang Zhiyan\AppData\Roaming\Typora\typora-user-images\image-20220105153905041.png)

![image-20220105153933681](C:\Users\Wang Zhiyan\AppData\Roaming\Typora\typora-user-images\image-20220105153933681.png)

![image-20220105154315930](C:\Users\Wang Zhiyan\AppData\Roaming\Typora\typora-user-images\image-20220105154315930.png)

上面有一点问题，应该是变换得到
$$
\sigma_b\sigma_a=\delta _{ab}-i\varepsilon_{abc}\sigma_c
$$

$$
[\sigma_a,\sigma_b]=2i\varepsilon_{abc}\sigma_c\\
如果代入I=i\sigma\\
算出来的就是[I_a,I_b]=-2i\varepsilon_{abc}\sigma_c=-2\varepsilon_{abc}I_c
$$

与他文章里的结果不一样
