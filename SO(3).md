------

#### $SO(3)$

$$
定义g\in SO(3),g\vec{r}=\vec{r}\\
就是要证明\det(g-E)=0 \ \ \ \ \ \ \ast (g-E)\vec{r}=0
$$

假若我们在这里把$\vec{r}$称为$\hat{k}$，那么取与之垂直的$\hat{i},\hat{j}$：
$$
C_k(\psi)=\begin{bmatrix}
 \cos \psi & -\sin \psi & \\
\sin \psi  & \cos \psi & \\
  &  &1
\end{bmatrix}
$$
<img src="C:\Users\Wang Zhiyan\AppData\Roaming\Typora\typora-user-images\image-20211206161944787.png" alt="image-20211206161944787" style="zoom: 50%;" />

来源，当眼睛从k轴望去，逆时针转动$\psi$角

坐标变换：
$$
变换矩阵P:\vec{r}'=Q\vec{r}\\
(\hat{i}',\hat{j}',\hat{k}')=(\hat{i},\hat{j},\hat{k})P\\
P^{-1}=P^T，给出：\\
线性变换A在旧基下的矩阵表示[A]_B与新基下的矩阵表示[A]_{B'}有：\\
[A]_B=P[A]_{B'}P^{-1}
$$
==我想一下，理解$g\vec{r}=\vec{r}$（完全重合）与只转动一定角度是否矛盾？==

不矛盾，因为转动角度是转动角度，$C_k(\psi)$保证的是k轴不变即：$C_k(\psi)\vec{k}=\vec{k}$。再思考一下转动矩阵是怎么引入的。
$$
SO(3)的欧拉角表示：SO(3)可以看作是一个球面转到与其重合的另一个位置\\
R(\alpha,\beta,\gamma)=C_{z''}(\gamma)C_{y'}(\beta)C_z(\alpha)
$$

<img src="C:\Users\Wang Zhiyan\AppData\Roaming\Typora\typora-user-images\image-20211207191804963.png" alt="image-20211207191804963" style="zoom:50%;" />
$$
由于C_{y'}(\beta)是在坐标Ox'y'z'中表示成\\
C_{y'}(\beta)=\begin{bmatrix}
 \cos \beta &  & \sin \beta \\
  & 1 & \\
-\sin \beta  &  &\cos \beta
\end{bmatrix}\\
所以要进行坐标变换：
由于新基Ox'y'z'是旧基Oxyz经过C_z(\alpha)变换成的，所以：\\
(\hat{i}',\hat{j}',\hat{k}')=(\hat{i},\hat{j},\hat{k})P \ \ 即(\hat{i}',\hat{j}',\hat{k}')=(\hat{i},\hat{j},\hat{k})\begin{bmatrix}
 \cos \alpha & -\sin \alpha & \\
\sin \alpha  & \cos \alpha & \\
  &  &1
\end{bmatrix}\\
C_{y'}(\beta)在Oxyz下的表示为：\\
\begin{bmatrix}
 \cos \alpha & -\sin \alpha & \\
\sin \alpha  & \cos \alpha & \\
  &  &1
\end{bmatrix}\begin{bmatrix}
 \cos \beta &  & \sin \beta \\
  & 1 & \\
-\sin \beta  &  &\cos \beta
\end{bmatrix}\begin{bmatrix}
 \cos \alpha & -\sin \alpha & \\
\sin \alpha  & \cos \alpha & \\
  &  &1
\end{bmatrix}^{-1}
$$

同理$C_{z''}(\gamma)$

于是
$$
R(\alpha,\beta,\gamma)=C_{z''}(\gamma)C_{y'}(\beta)C_z(\alpha)\\
=\begin{bmatrix}
 \cos \alpha \cos \beta\cos \gamma-\sin \alpha\sin\gamma & -\sin \alpha\cos \beta\sin\gamma-\sin \alpha\cos \gamma &  \cos \alpha \sin \beta\\
\sin \alpha \cos \beta\cos \gamma +\cos \alpha\sin\gamma& -\cos \alpha \cos \beta\sin\gamma+\cos \alpha\cos \gamma&\sin \alpha \sin \beta\\
 -\sin \beta\cos \gamma & \sin \beta\sin\gamma &\cos \beta
\end{bmatrix}
$$
另外，显然绕空间中任意一个轴都可以写成：

$$
A=P\begin{bmatrix}
 \cos \psi & -\sin \psi & \\
\sin \psi  & \cos \psi & \\
  &  &1
\end{bmatrix}P^{-1}
$$
它的解释是，类比上面以新基Ox'y'z'的y'轴转动角度，可以变换到旧基表示。在这里将选定的任意轴看作新基的z轴即z'轴，绕z'轴转动就会写成类似的形式，绕z'轴转动的矩阵写在中间($C_{y'}(\beta)$)，将z轴变换到z'轴的变换矩阵写在两边($C_z(\alpha)$)
$$
由于这是一个相似变换的形式，A=PC_k(\psi)P^{-1}\\
相似变换不改变迹,\Tr[PC_k(\psi)P^{-1}]=\Tr[C_k(\psi)]=1+2\cos\psi \\
也就是说，绕任意一个轴，只要转动的角度\psi是相同的，构成同类（\ast 这些不同的轴相同的角度的变换构成同类）
$$
必须要重申一下的是：
$$
C_{k_1}(\psi_1)C_{k_2}(\psi_2)=C_{k_3}(\psi_3)\\
作为SO(3)中的元素，两个元素相乘之后，转轴是可以变的。没有规定只能是同转轴的转动才能相乘。\\
前面也说了相似变换gC_k(\psi)g^{-1}的迹不变，实际上这个整体还可以表示绕gk轴转动：\\
gC_k(\psi)g^{-1}g\vec{k}=g\vec{k}
$$

------

#### $SO(3)$

$$
SO(3)还可以写成\\
C_{n(\theta,\varphi)}(\omega)=S(\varphi,\theta)C_k(\omega)S(\varphi,\theta)^{-1}\\
对比R(\alpha,\beta,\gamma)=C_{z''}(\gamma)C_{y'}(\beta)C_z(\alpha)可以发现，它反而有点像\\
任意表示A=PC_k(\psi)P^{-1}
$$

$$
C_{n(\theta,\varphi)}(\omega)=S(\varphi,\theta)C_k(\omega)S(\varphi,\theta)^{-1}
$$

这个形式不能用来求解生成元
$$
当\omega=0时，无论\theta ,\varphi为什么值，结果都为E，也就是说这里不是一一对应。\\也就是说在恒元E附近，存在不是一一对应\\所以参数R(\theta,\varphi,\omega)不能用来求解生成元
$$
要用下面这个形式
$$
D(\omega)=C_{n(\theta,\varphi)}(\omega)=e^{-i\omega_i T_i}
$$
利用这个新形式以及生成元的定义：$I_{element}\frac{\partial Group}{\partial element}|_{element=0} $
$$
I_1=\frac{\partial D(\omega) }{\partial \omega_1}|_{\omega_1=0} =\frac{\partial e^{-i\omega_1 T_1}}{\partial \omega_1}|_{\omega_1=0}=-iT
_1e^{-i\omega_1 T_1}|_{\omega_1=0}\\
I_1=\begin{bmatrix}
 0 &  & \\
  &  & -1\\
  & 1 &
\end{bmatrix},\ T_1=\begin{bmatrix}
 0 &  & \\
  &  & -i\\
  & i &
\end{bmatrix}
$$
我们发现这与y-z平面转动（y-z平面的$SO(2)$）很相似
$$
y-z平面,SO(2):D(\theta)=\begin{bmatrix}
 1 &  & \\
  & \cos \theta & -\sin \theta \\
  & \sin \theta & \cos \theta
\end{bmatrix}\\
I=\frac{\partial D(\theta) }{\partial \theta}|_{\theta=0} =\begin{bmatrix}
 0 &  & \\
  &  & -1\\
  & 1 &
\end{bmatrix}=I_1
$$
这样类推
$$
I_1=\begin{bmatrix}
 0 &  & \\
  &  & -1\\
  & 1 &
\end{bmatrix},\ T_1=\begin{bmatrix}
 0 &  & \\
  &  & -i\\
  & i &
\end{bmatrix}————(y-z)\\
I_2=\begin{bmatrix}
  &  & 1\\
  & 0 & \\
-1  &  &
\end{bmatrix},\ T_2=\begin{bmatrix}
  &  &i \\
  & 0 & \\
 -i &  &
\end{bmatrix}————(x-z)\\
I_3=\begin{bmatrix}
  & -1 & \\
 1 &  & \\
  &  &0
\end{bmatrix},\ T_3=\begin{bmatrix}
  & -i & \\
 i &  & \\
  & &0
\end{bmatrix}————(x-y)
$$

$$
\mathbf{Conclusion}\\
SO(3):D(\omega)=e^{i\omega_iT_i}\overset{I_i=-iT_i}{\rightarrow} e^{\omega_iI_i}
\\这个式子会涉及到后面李群的生成
$$

------

两种形式的联系
$$
C_{n(\theta,\varphi)}(\omega)=S(\varphi,\theta)C_k(\omega)S(\varphi,\theta)^{-1}\\
R(\alpha,\beta,\gamma)=C_{z''}(\gamma)C_{y'}(\beta)C_z(\alpha)\ \ :Eular表示
$$

$$
任意轴转动A=PC_k(\omega)P^{-1}\\
将n轴变到k轴再转\omega：C_{n(\theta,\varphi)}(\omega)=S(\varphi,\theta)C_k(\omega)S(\varphi,\theta)^{-1}，再利用S(\varphi,\theta)转回n轴\\
(当然，我觉得从某种意义上是将k视角调到n轴转动再调回，挪动眼睛，是一个概念)\\
其中S(\varphi,\theta)=C_k(\varphi)C_j(\theta)=\begin{bmatrix}
 \cos \varphi\cos\theta & -\sin \varphi &\cos \varphi \sin\theta \\
  \sin \varphi \cos\theta& \cos \varphi & \sin \varphi \sin\theta  \\
 -\sin\theta & 0 &\cos\theta
\end{bmatrix}\\
也就是说\\
S(\varphi,\theta)k=n,S(\varphi,\theta)^{-1}n=k\\
if \ set \ Rk=n,so\ S(\varphi,\theta)^{-1}Rk=k\\
说明k是S(\varphi,\theta)^{-1}R的转动轴，就可以表示：S(\varphi,\theta)^{-1}R=C_k(\gamma)\\
两边同时左乘：\\
R=S(\varphi,\theta)C_k(\gamma)=C_k(\varphi)C_j(\theta)C_k(\gamma)\\
形式如R(\alpha,\beta,\gamma)=C_{z''}(\gamma)C_{y'}(\beta)C_z(\alpha)
$$

------

## $Conclusion$

$$
群表示\\
C_{n(\theta,\varphi)}(\omega)=S(\varphi,\theta)C_k(\omega)S(\varphi,\theta)^{-1}\\
S(\varphi,\theta)=C_k(\varphi)C_j(\theta)=\begin{bmatrix}
 \cos \varphi\cos\theta & -\sin \varphi &\cos \varphi \sin\theta \\
  \sin \varphi \cos\theta& \cos \varphi & \sin \varphi \sin\theta  \\
 -\sin\theta & 0 &\cos\theta
\end{bmatrix}\\
D(\omega)=C_{n(\theta,\varphi)}(\omega)=e^{-i\omega_i T_i},\\
T_1=\begin{bmatrix}
 0 &  & \\
  &  & -i\\
  & i &
\end{bmatrix}, T_2=\begin{bmatrix}
  &  &i \\
  & 0 & \\
 -i &  &
\end{bmatrix}, T_3=\begin{bmatrix}
  & -i & \\
 i &  & \\
  & &0
\end{bmatrix}\\
R(\alpha,\beta,\gamma)=C_{z''}(\gamma)C_{y'}(\beta)C_z(\alpha)\\
R(\alpha,\beta,\gamma)=C_{z''}(\gamma)C_{y'}(\beta)C_z(\alpha)\\
=\begin{bmatrix}
 \cos \alpha \cos \beta\cos \gamma-\sin \alpha\sin\gamma & -\sin \alpha\cos \beta\sin\gamma-\sin \alpha\cos \gamma &  \cos \alpha \sin \beta\\
\sin \alpha \cos \beta\cos \gamma +\cos \alpha\sin\gamma& -\cos \alpha \cos \beta\sin\gamma+\cos \alpha\cos \gamma&\sin \alpha \sin \beta\\
 -\sin \beta\cos \gamma & \sin \beta\sin\gamma &\cos \beta
\end{bmatrix}
$$

$$
生成元\\
3个独立群参数:\varphi,\theta,\omega或者 三个欧拉角\alpha,\beta,\gamma \\
I_1=\begin{bmatrix}
 0 &  & \\
  &  & -1\\
  & 1 &
\end{bmatrix},
I_2=\begin{bmatrix}
  &  & 1\\
  & 0 & \\
-1  &  &
\end{bmatrix},
I_3=\begin{bmatrix}
  & -1 & \\
 1 &  & \\
  &  &0
\end{bmatrix}
$$

$$
生成元对易关系\\
[I_i,I_j]=\varepsilon _{ijk} I_k,\\
C_{ij}^{k}=\varepsilon _{ijk}
$$

$$
无穷小算子\\
X_1=x_2\partial_3-x_3\partial_2\\
X_2=x_3\partial_1-x_1\partial_3\\
X_3=x_1\partial_2-x_2\partial_1
$$

$$
算子对易关系\\
[X_i,X_j]=-\varepsilon _{ijk} X_k
$$

------

https://blog.csdn.net/luoshi006/article/details/78290177

