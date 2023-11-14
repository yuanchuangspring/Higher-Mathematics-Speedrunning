# 线性映射、矩阵 复习笔记
## 一、知识点梳理
### (一).线性映射 linear map
1. 基本定义：一个映射如果满足以下条件：
   1. $f(k\alpha)=kf(\alpha)$
   2. $f(\alpha_1+\alpha_2)=f(\alpha_1)+f(\alpha_2)$\
    则称该映射为线性映射。注意，一般做题时，只需判断$f(k_1\alpha_1+k_2\alpha_2)=k_1f(\alpha_1)+k_2f(\alpha_2)$即可
2. 线性变换 linear transformation：对于$V_1$到$V_2$的映射，如果$V_1=V_2$，则称该映射为线性变换
3. A linear map f is completely determined by its images at the unit vectors:
   * 这句话指的是f定义域中的任一向量都可以由单位向量表出，所以$f(\alpha)可以由f(\epsilon_i)$表示，由此我们可以将线性映射转变为矩阵的形式。详见第四条。
4. 线性映射的矩阵表示：
   * 首先，我们设$V_1$中的单位向量为$\epsilon_1···\epsilon_n$，而$V_2$中的单位向量为$\epsilon_1'···\epsilon_m'$，则每一个$f(\epsilon_i)$都可以用$\epsilon_j'$表示，具体如下：\
        $$
        f(x) = \begin{cases}f(\epsilon_1)=(\alpha11,\alpha21,···,\alpha m1)=\alpha11\epsilon_1'+···+\alpha m1\epsilon_m',\\
        \dots\\
        f(\epsilon_n)=(\alpha1n,\alpha2n,···,\alpha nm)=\alpha1n\epsilon_1'+···+\alpha nm\epsilon_m'
        \end{cases}
        $$
   * 所以，矩阵$A=(f(\epsilon_1)···f(\epsilon_n))$就被称作matrix of the linear map
5. 线性映射的几个特殊类型：
   1. 0映射 zero map：$0(\alpha)=0$
   2. $ker(f)$：the kernel of f 指的是当$f(k)=0$时k的值
   3. identity map：$id(\alpha)=\alpha$
6. 线性映射和线性方程组解的关系：线性方程组在$\beta$处的解，实际上是线性映射在$\beta$处的原像
### (二).线性映射和矩阵的运算 operations of matrices
1. 英文名词梳理：
   * product 乘积
   * multiplication of g by f 意指$g(f)$复合映射
2. 线性映射运算略
3. 矩阵运算：
   1. 矩阵的加减：必须保证同型矩阵，对应元素相加减
   2. 矩阵乘法：左行右列，依次相乘
   3. 矩阵的n次方幂：详见第3条，单独说明
4. 矩阵幂运算总结：
   1. 对角矩阵(unit matrix)n次方还是它本身
   2. 对角矩阵加一个角的形式：将对角单独拆分出来，运用多项式定理，进行运算
   3. 可以差分成一个行向量一个列向量的，拆开来，错位相乘
### (三).分块矩阵 partitioned matrices
1. 英文名词梳理：
   * block 块矩阵
   * m
2. 分块矩阵相乘：必须满足左矩阵的列分法和右矩阵的行分法相同，不然乘积无意义
3. 分块矩阵的转置：先以块为单位进行转置，再对每一个小块进行转置
4. 题外话：$r(A)=r(A^TA)=r(AA^T)$这个上课讲的时候走神了，没搞明白怎么证明的，不知道为什么在这一节课最后讲这个······
## 二、重点题型及解题法
1. 判断一个映射是否为线性映射，运用定义最后给出的办法
2. 写出一个线性映射的矩阵，运用相关定义
3. 复合映射的运算
4. 矩阵的运算，特别是乘法
5. 计算矩阵的n次方幂，详细解题法参见 一.3
6. 分块矩阵相乘
