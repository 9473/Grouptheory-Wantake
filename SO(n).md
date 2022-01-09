![image-20211229002731136](C:\Users\Wang Zhiyan\AppData\Roaming\Typora\typora-user-images\image-20211229002731136.png)

![image-20211229002852609](C:\Users\Wang Zhiyan\AppData\Roaming\Typora\typora-user-images\image-20211229002852609.png)
$$
但是我觉得这里有一点问题，凭什么<gx,gy>=<x,y>?\\
没问题，因为保内积
$$
![image-20211229002951706](C:\Users\Wang Zhiyan\AppData\Roaming\Typora\typora-user-images\image-20211229002951706.png)

------

![image-20220105155850327](C:\Users\Wang Zhiyan\AppData\Roaming\Typora\typora-user-images\image-20220105155850327.png)

可以看到，其实可以概括成一个约束条件$R^TR=I$自动保证了$\det =1$。但是实际上写开就是分别对对角矩阵元和非对角矩阵元的方程。
$$
推广
$$

![image-20211229003028479](C:\Users\Wang Zhiyan\AppData\Roaming\Typora\typora-user-images\image-20211229003028479.png)

![image-20211229003047277](C:\Users\Wang Zhiyan\AppData\Roaming\Typora\typora-user-images\image-20211229003047277.png)

![image-20211229003105304](C:\Users\Wang Zhiyan\AppData\Roaming\Typora\typora-user-images\image-20211229003105304.png)
$$
n\times n，n^2个元素，\\
减掉约束：\\
n个=1的求和方程(i=1,2,3,... n)\\

为什么有n(n+1)/2个约束方程？
$$


![image-20211229004006248](C:\Users\Wang Zhiyan\AppData\Roaming\Typora\typora-user-images\image-20211229004006248.png)
$$
看来\det >0这个条件没用到？应该是默认了\det >0\\
你想想，有逆=转置
$$
延伸阅读

https://zqw.ink/2020/05/14/TensorI/

