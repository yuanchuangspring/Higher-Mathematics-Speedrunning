# 线性方程组 复习笔记
## 一、知识点梳理
### (一).初等变换Elimination
1. 三种变换如下：\
(1).等式互换位置\
(2).等式乘以非零常数\
(3).等式乘非零常数后与其他等式相加减\
以上变换后解不变，且结果为标准阶梯型echelon form
### (二).向量组
1. 英文名词梳理：
   * demension 维度
   * component 向量组元素
   * unit vector 单位向量
2. 线性相关 linear dependent
3. 线性表出 linear represented
4. 向量组线性表出：向量组中的每一项都被另一个向量组线性表出
5. 向量组等价 equivalent：向量组相互线性表出
6. 极大线性无关组 maximal linearly independent subset：\
   * 定义：向量组内其他向量都可被极大组线性表出
7. 向量组的秩：向量组极大线性无关组的向量个数
8. 有关向量组线性关系的性质
   * 性质1：极大无关组与原向量组等价
   * 性质2：如果向量组B被A线性表出，且B向量数量大于A向量数量，则B线性相关
   * 性质3：两个线性无关组如果等价，则向量数量相同
   * 性质4：m维向量组，若有超过m个向量，则该向量组线性相关
   * 性质5：一个向量组的所有最大线性无关组有相同的向量数量且等价
   * 性质6：S被T线性表出，则$r(S)<=r(T)$
   * 性质7：增广向量组，原方程有解的条件是，系数向量组的秩等于增广向量组
   * 性质8：齐次方程式只有零解的充要条件是系数向量组的秩等于系数的个数/未知量个数
   * 性质9：方程组有唯一解的充要条件是系数向量组和增广向量组的秩均等于系数个数/未知数个数
### (三).矩阵初步
1. 英文名词梳理：
   * coefficient matrix 系数矩阵
   * augment matrix 增广矩阵 系数矩阵加入b一列的矩阵
2. 初等行变换 elementary row operations
   * 详见线性方程组初等变换
3. 矩阵相关性质：
   * 性质1：任何矩阵都等价于一个这样的矩阵——非零行首为1,含1的列其他元素全部为0，这样的矩阵成为最简形矩阵
   * 性质2：行秩等于列秩等于矩阵的秩
   * 性质3：矩阵的秩等于阶梯型矩阵(每行的向量个数严格递增)的非零行个数
   * 性质4：A的秩等于$A^T$的秩
### (四).线性方程组解的结构
1. 英文名词梳理：
   * solution set 解集
   * solution space 解空间
   * solution vector 解向量
2. 基础解系 basis for solutions 
   * 针对齐次方程组来说，满足以下条件：
        1. 方程组的任何一个解都能表示成基础解系的一个线性组合
        2. 基础解系必须线性无关 
3. 解的相关性质
   * 性质1：解向量组的秩等于未知量(indeterminate)的数量减去coefficient矩阵的秩，也就是n-r(证明没看懂)，且基础解系中的向量个数也就等于n-r，这里需要理解的是，基础解系即为解向量组的极大线性无关组
   * 性质2：解向量组的秩(n-r)也是自由未知量(free variable)的个数
   * 性质3：对于一般线性方程组，我们首先定义他的齐次形式方程组为导出组(derived system)，则线性方程组的所有解，都可以表示成$\gamma=\gamma_0+\eta$ ， 其中$\eta$为导出组的一个解，$\gamma_0$为线性方程组的一个特解，注意，当$\eta$取遍(run through)导出组的所有解时，线性方程的解也全部表示出来了
   * 性质4：由性质3得，线性方程组解唯一的充要条件是导出组只有零解
## 二、重点题型及解题法
1. 化简方程组并求解，运用初等变换
2. 找到参数使得方程组有解，运用性质：系数矩阵的秩等于增广矩阵的秩
3. 判断或证明是否线性相关，运用线性相关定义
4. 计算矩阵的秩，首先对矩阵进行化简，使其变为阶梯型，然后获得其中非零行的个数
5. 运用基础解系相关性质进行解的判断










