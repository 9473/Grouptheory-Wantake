$$
维数=独立群参数个数，可能不等于阶数
$$



$$
GL(2,R)\\
4个独立群参数\\
D(\alpha)=\begin{bmatrix}
  \alpha_1 & \alpha_2 \\
   \alpha_3 & \alpha_4
\end{bmatrix},\det D \ne 0\\
恒元D(\alpha)=\begin{bmatrix}
  1 & 0 \\
   0 & 1
\end{bmatrix},\alpha=(\alpha_1,\alpha_2,\alpha_3,\alpha_4)=(1,0,0,1)\\
I_1=\begin{bmatrix}
  1 & 0 \\
   0 & 0
\end{bmatrix},I_2=\begin{bmatrix}
  0 & 1 \\
   0 & 0
\end{bmatrix},I_3=\begin{bmatrix}
  0 & 0 \\
   1 & 0
\end{bmatrix},I_4=\begin{bmatrix}
  0 & 0 \\
   0 & 1
\end{bmatrix}\\
也即I_{11}=\begin{bmatrix}
  1 & 0 \\
   0 & 0
\end{bmatrix},I_{12}=\begin{bmatrix}
  0 & 1 \\
   0 & 0
\end{bmatrix},I_{21}=\begin{bmatrix}
  0 & 0 \\
   1 & 0
\end{bmatrix},I_{22}=\begin{bmatrix}
  0 & 0 \\
   0 & 1
\end{bmatrix}\\ 
[I_{11},I_{12}]=I_{11}I_{12}-I_{12}I_{11}=I_{11}-0=I_{11}\\
[I_{11},I_{21}]=0-I_{21}=-I_{21}\\
[I_{11},I_{22}]=0-0=0\\
[I_{12},I_{21}]=I_{21}-I_{12}=\begin{bmatrix}
  0 & -1 \\
   1 & 0
\end{bmatrix}\\
[I_{12},I_{22}]=I_{22}\\
[I_{21},I_{22}]=0
$$

$$
GL(n,R)\\
n×n矩阵,n^2个独立群参数\\
I_{ij}=\begin{bmatrix}
  & &  \\
  & 1_{(第i行第j列)} &  \\
  &  &\\
\end{bmatrix},I_{jk}=\begin{bmatrix}
  & &  \\
  & 1_{(第j行第k列)} &  \\
  &  &\\
\end{bmatrix}\\
[I_{ij},I_{jk}]=I_{ij}I_{jk}-I_{jk}I_{ij}=\begin{bmatrix}
  & &  \\
  & 1_{(第i行第k列)} &  \\
  &  &\\
\end{bmatrix}-0=I_{ik}\\
I_{ij}I_{jk}=\delta_{jj}I_{ik}\\
I_{ij}I_{lm}=\delta_{jl}I_{ik}\\
类推得知
[I_{ij},I_{lm}]=\delta_{jl}I_{im}-\delta_{mi}I_{lj}
$$

$$
SL(2,R)\\
3个独立群参数\\

D(\alpha)=\begin{bmatrix}
  \alpha_1 & \alpha_2 \\
   \alpha_3 & \alpha_4
\end{bmatrix},\det D = 1,\alpha_4=\frac{1+\alpha_2\alpha_3}{\alpha_1}\\
恒元D(\alpha)=\begin{bmatrix}
  1 & 0 \\
   0 & 1
\end{bmatrix},\alpha=(\alpha_1,\alpha_2,\alpha_3)=(1,0,0)\\
I_1=\begin{bmatrix}
  1 & 0 \\
   0 & -1
\end{bmatrix},I_2=\begin{bmatrix}
  0 & 1 \\
   0 & 0
\end{bmatrix},I_3=\begin{bmatrix}
  0 & 0 \\
   1 & 0
\end{bmatrix}\\
[I_1,I_2]=2I_2\\
[I_2,I_3]=I_1\\
[I_3,I_1]=2I_3
$$

$$
SL(n,R)\\
n^2-1个独立群参数，\\ \det D=1只给出一个约束方程，只减小一个自由度
$$



















D. Taylor, Pairs of Generators for Matrix groups {I}, The Cayley Bulletin 3, (1987), 76-85

