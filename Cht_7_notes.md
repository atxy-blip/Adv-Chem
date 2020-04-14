# Chapter 7: Approximation Methods                                                                                                                                                                                                                             第七章：近似方法

第六章指出，任何比氢原子更复杂的原子或分子薛定谔方程均不能精确求解:anguished::broken_heart:。本章将介绍两种使用最广泛的近似求解方法：变分法和微扰法:rofl:。

[toc]

## 7.1 The Variational Method Provides an Upper Bound to the Ground-State Energy of a System                                                                                                                     变分法给出了基态体系的能量上限

### The Variational Method                                                                                                                                                                                                                                                                                                        变分法

> #### Dirac notation 狄拉克符号或狄拉克标记
>
> 每一个量子态都被描述为希尔伯特空间中的态矢量，定义为右矢（ket）：$|\psi \rangle$ ；每一个右矢的共轭转置定义为其左矢（bra）：$\langle \psi |$。
>
> 内积$\langle \phi |\psi \rangle$ 外积$|\psi \rangle \langle \phi |$ 当狄拉克符号作用于两个基矢时，所得值为$\langle e_{i}|e_{j}\rangle =\delta _{ij}$
> $$
> \langle \psi |\psi \rangle =\sum _{i}|\psi _{i}|^{2}
> $$
>
> $$
> \langle \phi |\left(c_{1}|\psi _{1}\rangle +c_{2}|\psi _{2}\rangle \right)=c_{1} \langle \phi |\psi _{1}\rangle +c_{2}\langle \phi |\psi _{2}\rangle \\
> {\bigg (}c_{1}\langle \phi _{1}|+c_{2}\langle \phi _{2}|{\bigg )}\;|\psi \rangle =c_{1}\langle \phi _{1}|\psi \rangle +c_{2}\langle \phi _{2}|\psi \rangle \\
> \langle \phi |\psi \rangle =\langle \psi |\phi \rangle ^{*} \\
>  (|\omega \rangle \langle \phi |)\ |\psi \rangle =|\omega \rangle \ (\langle \phi |\psi \rangle ) \\
> \langle \phi |\ (X|\psi \rangle )=(\langle \phi |X)\ |\psi \rangle
> $$

线性变分原理：任一个波函数φ都可以展开为哈密顿算符的实际本征函数的*线性*组合

厄密算符的精确本征值不详，但可以假设其存在
$$
\hat { H } | \psi _ { n } \rangle = \varepsilon _ { n } | \psi _ { n } \rangle \quad n = 0,1，\cdots
$$

$$
\langle \psi _ { n } | \psi _ { n } \rangle = \delta_{\alpha\beta}
$$

本征值$\{ | \psi _ { n } \rangle , n = 0,1,2 , \ldots \}$

将本征值从小到大排序：
$$
\varepsilon _ { 0 } \leq \varepsilon _ { 1 } \leq \varepsilon _ { 2 } \leq \cdots \leq \varepsilon _ { \alpha } \leq \cdots
$$


试探波函数trial wave function $\varphi$，平均值

$$
E _ { \varphi } = \frac { \int \varphi ^ { * } \hat { H } \varphi \mathrm{d} \tau } { \int \varphi ^ { * } \varphi \mathrm{d} \tau } \geq \varepsilon _ { 0 }
$$

> #### Proof
>
> $$
> \varphi =\sum_{n} c_n \psi_n
> $$
>
> 交换积分与求和的顺序
> $$
> E _ { \varphi } = \frac { \int \varphi ^ { * } \hat { H } \varphi \mathrm{d} \tau } { \int \varphi ^ { * } \varphi \mathrm{d} \tau }
> = \frac { \int \sum _ { n } c _ { n } ^ { * } \psi _ { n } ^ { * } \hat { H } \sum _ { m } c _ { m } \psi _ { m } \mathrm{d} \tau } { \int \sum _ { n } c _ { n } ^ { * } \psi _ { n } ^ { * } \sum _ { m } c _ { m } \psi _ { m } \mathrm{d} \tau } = \frac { \sum _ { n } \sum _ { m } c _ { n } ^ { * } c _ { m } \int \psi _ { n } ^ { * } \hat { H } \psi _ { m } \mathrm{d} \tau } { \sum _ { n } \sum _ { m } c _ { n } ^ { * } c _ { m } \int \psi _ { n } ^ { * } \psi _ { m } \mathrm{d} \tau }
> $$
>
> 运用正交条件
> $$
> \left. { \int \psi _ { n } ^ { * } \hat { H } \psi _ { m } \mathrm{d} \tau = \int \psi _ { n } ^ { * } ( \varepsilon _ { m } \psi _ { m } ) \mathrm{d} \tau = \varepsilon _ { m } \int \psi _ { n } ^ { * } \psi _ { m } \mathrm{d} \tau = \varepsilon _ { m } \delta _ { n m } } \\ 
> { \int \psi _ { n } ^ { * } \psi _ { m } \mathrm{d} \tau = \delta _ { n m } } \right.
> $$
>
> 只有$n=m$时才能保留m，消去m变为一重求和 复共轭与自身相乘得到模的平方
> $$
> \left. { E _ { \varphi } = \frac { \sum _ { n } \sum _ { m } c _ { n } ^ { * } c _ { m } \varepsilon _ { m } \delta _ { n m } } { \sum _ { n } \sum _ { m } c _ { n } ^ { * } c _ { m } \delta _ { n m } } = \frac { \sum _ { n } c _ { n } ^ { * } c _ { n } \varepsilon _ { n } } { \sum _ { n } c _ { n } ^ { * } c _ { n } } } \\
> { E _ { \varphi } - \varepsilon _ { 0 } = \frac { \sum _ { n } c _ { n } ^ { * } c _ { n } \varepsilon _ { n } } { \sum _ { n } c _ { n } ^ { * } c _ { n } } - \frac { \varepsilon _ { 0 } \sum _ { n } c _ { n } ^ { * } c _ { n } } { \sum _ { n } c _ { n } ^ { * } c _ { n } } = \frac { \sum _ { n } c _ { n } ^ { * } c _ { n } ( \varepsilon _ { n } - \varepsilon _ { 0 } ) } { \sum _ { n } c _ { n } ^ { * } c _ { n } } \geq 0 } \right.
> $$

若试探波函数依赖于若干变量$\alpha,\beta,\gamma,\cdots$
$$
E _ { \varphi } (\alpha,\beta,\gamma,\cdots) \geqslant \varepsilon _ { 0 }
$$

可根据这些变量对E求极小值，逼近基态能量

> #### Example 7.1
>
> 使用$e^{-\alpha r}$这个试探波函数计算氢原子基态能量。
> $$
> \hat { H } = - \frac { h ^ { 2 } } { 2 m _ { e } r ^ { 2 } } \frac { \mathrm{d} } { \mathrm{d} r } \left( r ^ { 2 } \frac { \mathrm{d} } { \mathrm{d} r } \right) - \frac { e ^ { 2 } } { 4 \pi \varepsilon _ { 0 } r }
> $$
> 球极坐标 三个坐标积分 $\mathrm{d} \tau = r ^ { 2 } \sin \theta \mathrm{d} r \mathrm{d} \theta \mathrm{d} \phi$
> $$
> E _ { 0 } = \frac { \int \psi _ { 0 } ^ { * } \hat { H } \psi _ { 0 } \mathrm{d} \tau } { \int \psi _ { 0 } ^ { * } \psi _ { 0 } \mathrm{d} \tau } = \frac { 4 \pi \int _ { 0 } ^ { \infty } e ^ { - \alpha r } \hat { H } e ^ { - \alpha r } r ^ { 2 } \mathrm{d} r } { 4 \pi \int _ { 0 } ^ { \infty } e ^ { - \alpha r } e ^ { - \alpha r } r ^ { 2 } \mathrm{d} r } = \frac { \hbar ^ { 2 } \alpha ^ { 2 } } { 2 m _ { e } } - \frac { e ^ { 2 } \alpha } { 4 \pi \varepsilon _ { 0 } }
> $$
>
> $$
> \frac { \mathrm{d} E _ { 0 } } { \mathrm{d} \alpha } = 0 \quad \Rightarrow \quad \alpha = \frac { m _ { e } e ^ { 2 } } { 4 \pi \varepsilon _ { 0 } \hbar ^ { 2 } }
> $$
>
> $$
> E_0 = \frac{1}{2} \left(\frac{ m _ { e } e ^ { 4 } } { 16 \pi^2 \varepsilon _ { 0 }^2 \hbar ^ { 2 } }\right)
> $$
>

变分法的关键在于选一个好的试探波函数。

### Application of the Variational Method to Two-electron Problems                                                                                                                                                                                                                     将变分法用于两电子体系

氦原子哈密顿
$$
\left. { \hat { H } = ( - \frac { \hbar ^ { 2 } } { 2 m _ { e } } \nabla _ { 1 } ^ { 2 } - \frac { 2 e ^ { 2 } } { 4 \pi \varepsilon _ { 0 } } \frac { 1 } { \vec{r} _ { 1 } } ) + ( - \frac { \hbar ^ { 2 } } { 2 m _ { e } } \nabla _ { 2 } ^ { 2 } - \frac { 2 e ^ { 2 } } { 4 \pi \varepsilon _ { 0 } } \frac { 1 } { \vec{r} _ { 2 } } ) + \frac { e ^ { 2 } } { 4 \pi \varepsilon _ { 0 } } \cdot \frac { 1 } { r _ { 12 } } }\\  \\{ = \hat { H } _ { H } ( 1 ) + \hat { H } _ { H } ( 2 ) + \frac { e ^ { 2 } } { 4 \pi \varepsilon _ { 0 } } \cdot \frac { 1 } { r _ { 12 } } } \right.
$$

选取一个反对称的试探波函数。物理意义：交换指标，多一个符号 电子是费米子fermion 

空间部分Psi与自旋部分波函数相乘

考虑单个电子
$$
\Psi _ { 0 } ( x _ { 1 } , x _ { 2 } ) = \varphi _ { 0 } ( \vec{r} _ { 1 } , \vec{r} _ { 2 } ) \Omega ( \sigma _ { 1 } , \sigma _ { 2 } ) \\
\Omega ( \sigma _ { 1 } , \sigma _ { 2 } ) = \frac { 1 } { \sqrt { 2 } } [ \alpha ( 1 ) \beta ( 2 ) - \beta ( 1 ) \alpha ( 2 ) ] \\
\varphi _ { 0 } ( \vec{r} _ { 1 } , \vec{r} _ { 2 } ) = \psi _ { 1 s } ( \vec{r} _ { 1 } ) \psi _ { 1 s } ( \vec{r} _ { 2 } ) \\
\psi _ { 1 s } ( r _ { j } ) = ( \frac { Z ^ { 3 } } { \pi a _ { 0 } ^ { 3 } } ) ^ { 1 / 2 } e ^ { - Z _ { j } / a _ { 0 } } \quad j = 1 \text { or } 2
$$

分母归一，计算平均值

自旋部分归一，只需对空间部分积分
$$
\begin{aligned}
E ( Z ) &= \int \Psi _ { 0 } ( x _ { 1 } , x _ { 2 } ) \hat { H } \Psi _ { 0 } ( x _ { 1 } , x _ { 2 } ) \mathrm{d} x _ { 1 } \mathrm{d} x _ { 2 } \\ 
&= \int \Omega ( \sigma _ { 1 } , \sigma _ { 2 } ) \Omega ( \sigma _ { 1 } , \sigma _ { 2 } ) \mathrm{d} \sigma _ { 1 } \mathrm{d} \sigma _ { 2 } \int \varphi _ { 0 } ( \vec{r} _ { 1 } , \vec{r} _ { 2 } ) \hat { H } \varphi _ { 0 } ( \vec{r} _ { 1 } , \vec{r} _ { 2 } ) \mathrm{d} \vec{r} _ { 1 } \mathrm{d} \vec{r} _ { 2 } \\
&= 1 \times \int \varphi _ { 0 } ( \vec{r} _ { 1 } , \vec{r} _ { 2 } ) \hat { H } \varphi _ { 0 } ( \vec{r} _ { 1 } , \vec{r} _ { 2 } ) \mathrm{d} \vec{r} _ { 1 } \mathrm{d} \vec{r} _ { 2 } \\
&= \frac { m _ { e } e ^ { 4 } } { 16 \pi ^ { 2 } \varepsilon _ { 0 } ^ { 2 } \hbar ^ { 2 } } ( Z ^ { 2 } - \frac { 27 } { 8 } Z )
\end{aligned}
$$

$$
\frac { \mathrm{d} E } { \mathrm{d} Z} = 0 \quad \Rightarrow \quad Z_{\text{min}} = \frac { 27 } { 16 }
$$

$$
E_{\text{min}} = -\left(\frac { 27 } { 16 } \right)^2=-2.8477
$$

实验结果$-2.9033$，化学精度1kcal/mol

## 7.2 A Trial Function That Depends Linearly on the Variational Parameters Leads to a Secular Determinant                                                                                                                                                                                                                                                                        与变量线性相关的试探波函数得到久期行列式

### The Secular Determinant                                                                                                                                                                                                                                                                         久期行列式

$$
| \Phi \rangle = \sum_{i=1}^{N} c _ { i } | \psi _ { i } \rangle
$$

$\{| \psi _ { i } \rangle\}$

假设所有的波函数都是实数集上的，定义内积
$$
\langle \Phi | \Phi \rangle = \sum _ { i j } c _ { i } c _ { j } \langle \psi _ { i } | \psi _ { j } \rangle = \sum _ { i j } c _ { i } c _ { j } S _ { i j }
$$

$$
\langle \Phi | \hat { H } | \Phi \rangle = \sum _ { i j } c _ { i } \langle \psi _ { i } | \hat { H } | \psi _ { j } \rangle c _ { j } = \sum _ { i j } c _ { i } c _ { j } H _ { i j }
$$

$$
\langle \psi _ { i } | \hat { H } | \psi _ { j } \rangle = H _ { i j } = H _ { j i } , \quad \langle \psi _ { i } | \psi _ { j } \rangle = S _ { i j } = S _ { j i }
$$

平均值计算公式 求E对c的导数

$$
E = \frac { \langle \Phi | \hat { H } | \Phi \rangle } { \langle \Phi | \Phi \rangle } = \frac { \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } H _ { i j } } { \sum _ { j = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } S _ { i j } }
$$
移项：
$$
\sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } H _ { i j } = E \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } S _ { i j }
$$
复合函数求导 右边第一项等于0
$$
\frac { \partial } { \partial c _ { k } } \left( \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } H _ { i j } \right) = \frac { \partial E } { \partial c _ { k } } \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } S _ { i j } + E \frac { \partial } { \partial c _ { k } } \left( \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } S _ { i j } \right)
$$

由于我们根据$c _ { k }$求E的极小值
$$
\frac { \partial E } { \partial c _ { k } } = 0 \quad k=1,2,\cdots
$$

故
$$
\frac { \partial } { \partial c _ { k } } ( \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } H _ { i j } ) = E \frac { \partial } { \partial c _ { k } } ( \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } S _ { i j } )
$$

由$\frac { \partial c _ { i } } { \partial c _ { k } } = \delta _ { i k } \quad k=1,2,\cdots$
$$
\begin{aligned}
\frac { \partial } { \partial c _ { k } } ( \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } H _ { i j } ) &= \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } \frac { \partial c _ { i } } { \partial c _ { k } } c _ { j } H _ { i j } + \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } \frac { \partial c _ { j } } { \partial c _ { k } } H _ { i j } \\
&= \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } \delta _ { i k } c _ { j } H _ { i j } + \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } \delta _ { j k } H _ { i j } \\
&= \sum _ { j = 1 } ^ { N } c _ { j } H _ { k j } + \sum _ { i = 1 } ^ { N } c _ { i } H _ { i k }
\end{aligned}
$$

i和j有相同意义 实函数$H_{ij}=H_{ji}$
$$
E \frac { \partial } { \partial c _ { k } } ( \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } S _ { i j } ) = E ( \sum _ { i = 1 } ^ { N } c _ { i } S _ { i k } + \sum _ { j = 1 } ^ { N } c _ { j } S _ { k j } )
$$

于是：
$$
\sum _ { i = 1 } ^ { N } c _ { i } H _ { i k } + \sum _ { j = 1 } ^ { N } c _ { j } H _ { i j } = E ( \sum _ { i = 1 } ^ { N } c _ { i } S _ { i k } + \sum _ { j = 1 } ^ { N } c _ { j } S _ { k j } )
$$

于是：
$$
\sum _ { i = 1 } ^ { N } c _ { i } H _ { i k } = E \sum _ { i = 1 } ^ { N } c _ { i } S _ { i k }
$$

$$
\sum _ { i = 1 } ^ { N } ( H _ { i k } - E S _ { i k } ) c _ { i } = 0 \quad ( k = 1,2 , \cdots , N )
$$

上述方程组要有非平庸解，则其对应的系数行列式=0，解出E，

$$
\begin{vmatrix}
{ H _ { 11 } - E S _ { 11 } } & { H _ { 1N } - E S _ { 1N } } &\cdots & { H _ { 1N } - E S _ { 1N } } \\ 
{ H _ { 12 } - E S _ { 12 } } & { H _ { 22 } - E S _ { 22 } } &\cdots & { H _ { 2N } - E S _ { 2N } } \\
\vdots &\vdots &\ddots &\vdots \\
{ H _ { 1N } - E S _ { 1N } } & { H _ { 2N } - E S _ { 2N } } &\cdots & { H _ { NN } - E S _ { NN } }
\end{vmatrix} = 0
$$
该行列式称为久期行列式secular determinant。

N个根 最小根接近基态能量

### An Alternative Expression                                                                                                                                                                                另一种表示

$$
\begin{pmatrix}
{ H _ { 11 } - E S _ { 11 } } & { H _ { 1N } - E S _ { 1N } } &\cdots & { H _ { 1N } - E S _ { 1N } } \\ 
{ H _ { 12 } - E S _ { 12 } } & { H _ { 22 } - E S _ { 22 } } &\cdots & { H _ { 2N } - E S _ { 2N } } \\
\vdots &\vdots &\ddots &\vdots \\
{ H _ { 1N } - E S _ { 1N } } & { H _ { 2N } - E S _ { 2N } } &\cdots & { H _ { NN } - E S _ { NN } }
\end{pmatrix}
\begin{pmatrix}
{ c _ { 1 } } \\ 
{ c _ { 2 } } \\
\vdots \\
{ c _ { N } }
\end{pmatrix} =0
$$

$$
\begin{pmatrix}
{ H _ { 11 } } & { H _ { 1N } } &\cdots & { H _ { 1N } } \\ 
{ H _ { 12 } } & { H _ { 22 } } &\cdots & { H _ { 2N } } \\
\vdots &\vdots &\ddots &\vdots \\
{ H _ { 1N } } & { H _ { 2N } } &\cdots & { H _ { NN } }
\end{pmatrix}
\begin{pmatrix}
{ c _ { 1 } } \\ 
{ c _ { 2 } } \\
\vdots \\
{ c _ { N } }
\end{pmatrix} = E 
\begin{pmatrix}
{ S _ { 11 } } & { S _ { 1N } } &\cdots & { S _ { 1N } } \\ 
{ S _ { 12 } } & { S _ { 22 } } &\cdots & { S _ { 2N } } \\
\vdots &\vdots &\ddots &\vdots \\
{ S _ { 1N } } & { S _ { 2N } } &\cdots & { S _ { NN } }
\end{pmatrix}
\begin{pmatrix}
{ c _ { 1 } } \\ 
{ c _ { 2 } } \\
\vdots \\
{ c _ { N } }
\end{pmatrix}
$$

令

$$
H = \begin{pmatrix}
{ H _ { 11 } } & { H _ { 1N } } &\cdots & { H _ { 1N } } \\ 
{ H _ { 12 } } & { H _ { 22 } } &\cdots & { H _ { 2N } } \\
\vdots &\vdots &\ddots &\vdots \\
{ H _ { 1N } } & { H _ { 2N } } &\cdots & { H _ { NN } }
\end{pmatrix} \quad c =
\begin{pmatrix}
{ c _ { 1 } } \\ 
{ c _ { 2 } } \\
\vdots \\
{ c _ { N } }
\end{pmatrix} \quad S =\begin{pmatrix}
{ S _ { 11 } } & { S _ { 1N } } &\cdots & { S _ { 1N } } \\ 
{ S _ { 12 } } & { S _ { 22 } } &\cdots & { S _ { 2N } } \\
\vdots &\vdots &\ddots &\vdots \\
{ S _ { 1N } } & { S _ { 2N } } &\cdots & { S _ { NN } }
\end{pmatrix}
$$

得到矩阵方程 E为常数
$$
Hc=ESc
$$

很多解 ci为列矢量
$$
H \vec{c}^i=E\vec{S}\vec{c}^i
$$

$$
\vec{C} = \begin{pmatrix} { \vec{c} ^ { 1 } } &{ \vec{c} ^ { 2 } } &\cdots &{ \vec{c} ^ { N } } \end{pmatrix} =
\begin{pmatrix}
{ c _ { 11 } } & { c _ { 11 } } &\cdots & { c _ { N1 } } \\ 
{ c _ { 12 } } & { c _ { 22 } } &\cdots & { c _ { N2 } } \\
\vdots &\vdots &\ddots &\vdots \\
{ c _ { 1N } } & { c _ { 2N } } &\cdots & { c _ { NN } }
\end{pmatrix} \quad \varepsilon=
\begin{pmatrix}
{ E _ { 1 } } &&& \\ 
& { E _ { 2 } } && \\
&& \ddots & \\
&&& { E _ { N } }
\end{pmatrix}
$$

下面的矩阵方程中每一项都是矩阵
$$
HC=SC\varepsilon
$$

线性变分法等效于解本征值方程
$$
C^{-1}S^{-1} HC=\varepsilon
$$

要求得本征值，需找到使$S^{-1} H$对角化的矩阵$C$

> #### Example 7.2
>
> 对箱中粒子模型应用线性变分法，确定其归一化波函数
> $$
> \phi = c _ { 1 } x ( 1 - x ) + c _ { 2 } x ^ { 2 } ( 1 - x ) ^ { 2 } \quad 0 \leq x \leq 1
> $$
>
> $$
> \begin{vmatrix}
> { H _ { 11 } - E S _ { 11 } } & { H _ { 12 } - E S _ { 12 } } \\ 
> { H _ { 12 } - E S _ { 12 } } & { H _ { 22 } - E S _ { 22 } } 
> \end{vmatrix} = 0
> $$
>
> $$
> \begin{vmatrix}
> { \frac { 1 } { 6 } - \frac { E ^ { \prime } } { 30 } } & { \frac { 1 } { 30 } - \frac { E ^ { \prime } } { 140 } } \\ 
> { \frac { 1 } { 30 } - \frac { E ^ { \prime } } { 140 } } & { \frac { 1 } { 105 } - \frac { E ^ { \prime } } { 630 } } 
> \end{vmatrix} = 0
> $$
>
> E最小值已知
> $$
> \frac { c _ { 2 } } { c _ { 1 } } = - \frac { H _ { 11 } - E _ { \min } S _ { 11 } } { H _ { 12 } - E _ { \min } S _ { 12 } } = \frac { \frac { h ^ { 2 } } { 6 m } - ( 4.93487 \frac { h ^ { 2 } } { m } ) \frac { 1 } { 30 } } { \frac { h ^ { 2 } } { 30 m } - ( 4.93487 \frac { h ^ { 2 } } { m } ) \frac { 1 } { 140 } } = 1.133
> $$
>
> $$
> \phi = 4.404 x ( 1 - x ) + 4.990 x ^ { 2 } ( 1 - x ) ^ { 2 }
> $$
>
> <div align=center><img src=".\figures\Figure_7.3.png" alt="Figure_7.3"/>
>
> ```python
> import matplotlib.pyplot as plt
> import numpy as np
> 
> x = np.arange(0.0, 1.0, 0.01)
> phi = 4.404 * x * ( 1 - x ) + 4.990 * x ** 2 *( 1 - x ) ** 2
> psi = np.sqrt(2) * np.sin(np.pi * x)
> 
> fig, ax = plt.subplots()
> ax.plot(x, phi)
> ax.plot(x, psi)
> 
> ax.set(xlabel='x', ylabel=r"$\phi$",
>     title='Figure 7.3 A comparison of the optimized trial \
> function with \nthe exact ground-state particle-in-a-box wave\
> function.')
> ax.grid()
> 
> plt.show()
> ```

## 7.3 Trial Functions Can Be Linear Combination of Functions that Also Contain Variational Parameters                                                                                                                                                                                 试探波函数可以是包含变量的函数的线性组合
$$
\phi=\sum_{j=1}^{N}c_jf_j
$$

氢原子
$$
\phi=\sum_{j=1}^{N}c_je^{-\alpha_jr^2}
$$

## 7.4 Perturbation Theory Expresses the Solution to One Problem in Terms of Another Problem Solved Previously                                                                                                                                                                         微扰法根据一个已解决问题给出了另一个问题的解

### Perturbation Theory                                                                                                                                                                                                                           微扰法

$$
H | \Phi _ { i } \rangle = ( H _ { 0 } + v ) | \Phi _ { i } \rangle = E _ { i } | \Phi _ { i } \rangle
$$

已知$H_0$的本征函数和本征值，0级哈密顿 perturbation尽可能小
$$
H _ { 0 } | \psi _ { i } ^ { ( 0 ) } \rangle = E _ { i } ^ { ( 0 ) } | \psi _ { i } ^ { ( 0 ) } \rangle
$$
在$\lambda=0$附近做泰勒展开

$$
H = H _ {0} + \lambda \nu \\
E _ { i } = E _ { i } ^ { ( 0 ) } + \lambda E _ { i } ^ { ( 1 ) } + \lambda ^ { 2 } E _ { i } ^ { ( 2 ) } + \cdots \\
| \Phi _ { i } \rangle = | \psi _ { i } ^ { ( 0 ) } \rangle + \lambda | \psi _ { i } ^ { ( 1 ) } \rangle + \lambda ^ { 2 } | \psi _ { i } ^ { ( 2 ) } \rangle + \cdots
$$

$E _ { i } ^ { ( n ) }$：第n能级

$\psi _ { i } ^ { ( n ) }$：第n级波函数

定义$| i \rangle = | \psi _ { i } ^ { ( 0 ) } \rangle$，为计算方便，对$| \Phi _ { i } \rangle$做中间归一化intermediate normalization
$$
\langle i | \Phi _ { i } \rangle = \langle i | i \rangle + \lambda \langle i | \psi _ { i } ^ { ( 1 ) } \rangle + \cdots = 1
$$

第一项归一，其余项为0，其余波函数都和i正交故有
$$
\langle i | \psi _ { i } ^ { ( n ) } \rangle = 0 \quad n=1,2,3,\cdots
$$
代入薛定谔方程
$$
( H _ { 0 } + \lambda \nu ) ( | i \rangle + \lambda | \psi _ { i } ^ { ( 1 ) } \rangle + \lambda ^ { 2 } | \psi _ { i } ^ { ( 2 ) } \rangle + \cdots ) \\ 
= ( E _ { i } ^ { ( 0 ) } + \lambda E _ { i } ^ { ( 1 ) } + \lambda ^ { 2 } E _ { i } ^ { ( 2 ) } + \cdots ) ( | i \rangle + \lambda | \psi _ { i } ^ { ( 1 ) } \rangle + \cdots )
$$

$\lambda ^ { n }$系数相等

列表
$$
n = 0 H _ { 0 } | i \rangle = E _ { i } ^ { ( 0 ) } | i \rangle \\
n = 1 \\
n = 2 \\
n = 3 \\
$$


$$
\langle n | ( E _ { i } ^ { ( 0 ) } - H _ { 0 } ) | \psi _ { i } ^ { ( 1 ) } \rangle = \langle n | v - E _ { i } ^ { ( 1 ) } | i \rangle = \langle n | v | i \rangle \quad ( n \neq i )
$$

左=右
$$
\begin{aligned}
E _ { i } ^ { ( 0 ) } &= \langle i | H _ { 0 } | i \rangle \\
E _ { i } ^ { ( 1 ) } &= \langle i | \nu | i \rangle \\
E _ { i } ^ { ( 2 ) } &= \langle i | \nu | \psi _ { i } ^ { ( 1 ) } \rangle \\
E _ { i } ^ { ( 3 ) } &= \langle i | \nu | \psi _ { i } ^ { ( 2 ) } \rangle \\
\end{aligned}
$$

> #### Hermitian
>
> $$
> \langle f | \hat { A } | g \rangle = \langle \hat { A } f | g \rangle \\
>  \langle i | H _ { 0 } | \psi _ { i } ^ { ( n ) } \rangle = E _ { i } ^ { ( 0 ) } \langle i | \psi _ { i } ^ { ( n ) } \rangle = 0
> $$

n=1
$$
H _ { 0 } | \psi _ { i } ^ { ( 1 ) } \rangle + v | i \rangle = E _ { i } ^ { ( 0 ) } | \psi _ { i } ^ { ( 1 ) } \rangle + E _ { i } ^ { ( 1 ) } | i \rangle
$$
左乘$\langle i |$，左右第一项等于0
$$
\langle i | H _ { 0 } | \psi _ { i } ^ { ( 1 ) } \rangle + \langle i | \nu | i \rangle = \langle i | E _ { i } ^ { ( 0 ) } | \psi _ { i } ^ { ( 1 ) } \rangle + \langle i | E _ { i } ^ { ( 1 ) } | i \rangle
$$
一级微扰
$$
E _ { i } ^ { ( 1 ) } = \langle i | \nu | i \rangle = \left \langle \psi _ { i } ^ { ( 0 ) } \right | \nu \left | \psi _ { i } ^ { ( 0 ) } \right \rangle
$$
一级微扰$\lambda = 1$才是真正能够感兴趣的哈密顿
$$
H = H _ {0} + \nu \\
E _ { i } = E _ { i } ^ { ( 0 ) } + E _ { i } ^ { ( 1 ) } + E _ { i } ^ { ( 2 ) } + \cdots \\
\left | \Phi _ { i } \right \rangle = i + \left | \psi _ { i } ^ { ( 1 ) } \right \rangle + \left | \psi _ { i } ^ { ( 2 ) } \right \rangle + \cdots
$$
把i那部分提到外面 波函数有常数不确定性

### The zeroth-order wave function and the first-order energy                                                                                                                                                           零级波函数和一级能量

$$
\begin{aligned}
E _ { i } ^ { ( 1 ) } &= \left \langle \psi _ { i } ^ { ( 0 ) } | \nu | \psi _ { i } ^ { ( 0 ) } \right \rangle \\
E _ { i } ^ { ( 0 ) } + E _ { i } ^ { ( 1 ) } &= \left \langle \psi _ { i } ^ { ( 0 ) } | H _ { 0 } | \psi _ { i } ^ { ( 0 ) }  \right \rangle + \left \langle \psi _ { i } ^ { ( 0 ) } | \nu | \psi _ { i } ^ { ( 0 ) } \right \rangle \\
&= \left \langle \psi _ { i } ^ { ( 0 ) } | H | \psi _ { i } ^ { ( 0 ) } \right \rangle
\end{aligned}
$$
### The first-order wave function and the second-order energy                                                                                                                                                           一级波函数和二级能量

$n=2$
$$
\left( E _ { i } ^ { ( 0 ) } - H _ { 0 } \right) | \psi _ { i } ^ { ( 1 ) } \rangle = \left( v - E _ { i } ^ { ( 1 ) } \right) | i \rangle
$$
左乘$\langle n |$有：
$$
\left\langle n \right| \left( E _ { i } ^ { ( 0 ) } - H _ { 0 } \right) \left| \psi _ { i } ^ { ( 2 ) } \right\rangle = \left\langle n \right| v - E _ { i } ^ { ( 1 ) } \left| \psi _ { i } ^ { ( 1 ) } \right\rangle - E _ { i } ^ { ( 2 ) } \langle n | i \rangle \quad ( n \neq i )
$$
使用本征值 $H _ { 0 } | m \rangle = E _ { m } ^ { ( 0 ) } | m \rangle$
$$
| \psi _ { i } ^ { ( 1 ) } \rangle = { \sum _ { m } } ^ { \prime } | m \rangle C _ { m } ^ { ( 1 ) } \quad ( m \neq i )
$$

$$
\begin{aligned}
\langle n | \left( E _ { i } ^ { ( 0 ) } - H _ { 0 } \right) { \sum _ { m } } ^ { \prime } C _ { m } ^ { ( 1 ) } | m \rangle
&= { \sum _ { m } } ^ { \prime } \langle n | \left( E _ { i } ^ { ( 0 ) } - H _ { 0 } \right) | m \rangle C _ { m } ^ { ( 1 ) } \\
&= { \sum _ { m } } ^ { \prime } ( n | ( E _ { i } ^ { ( 0 ) } - E _ { m } ^ { ( 0 ) } ) | m \rangle C _ { m } ^ { ( 1 ) } \\
&= { \sum _ { m } } ^ { \prime } ( E _ { i } ^ { ( 0 ) } - E _ { m } ^ { ( 0 ) } ) \langle n | m \rangle C _ { m } ^ { ( 1 ) } \\
&= ( E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } ) C _ { n } ^ { ( 1 ) }
\end{aligned}
$$

$$
( E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } ) C _ { n } ^ { ( 1 ) } = \langle n | v | i \rangle \quad C _ { n } ^ { ( 1 ) } = \frac { \langle n | v | i \rangle } { E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } }
$$

一级波函数为：
$$
| \psi _ { i } ^ { ( 1 ) } \rangle = {\sum _ { n }} ^ { \prime } | n \rangle \frac { \langle n | \nu | i \rangle } { E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } } \quad ( n \neq i )
$$

二级能量为：
$$
E _ { i } ^ { ( 2 ) } = \langle i | v | \psi _ { i } ^ { ( 1 ) } \rangle = \sum _ { n } \langle i | v | n \rangle \frac { \langle n | v | i \rangle } { E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } } = \sum _ { n } \cdot \frac { \langle i | v | n \rangle \langle n | v | i \rangle } { E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } }
$$
### The second-order wave function and the third-order energy                                                                                                                                                          二级波函数和三级能量

$n=2$
$$
\left( E _ { i } ^ { ( 0 ) } - H _ { 0 } \right) | \psi _ { i } ^ { ( 2 ) } \rangle = \left( v - E _ { i } ^ { ( 1 ) } \right) | \psi _ { i } ^ { ( 1 ) } \rangle - E _ { i } ^ { ( 2 ) } | i \rangle
$$

左乘$\langle n |$有：
$$
\langle n | \left( E _ { i } ^ { ( 0 ) } - H _ { 0 } \right) | \psi _ { i } ^ { ( 2 ) } \rangle = \langle n | v - E _ { i } ^ { ( 1 ) } | \psi _ { i } ^ { ( 1 ) } \rangle - E _ { i } ^ { ( 2 ) } \langle n | i \rangle \quad ( n \neq i )
$$
$$
\left( E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } \right) \langle n | \psi _ { i } ^ { ( 2 ) } \rangle = \langle n | v | \psi _ { i } ^ { ( 1 ) } \rangle - E _ { i } ^ { ( 1 ) } \langle n | \psi _ { i } ^ { ( 1 ) } \rangle
$$

$$
\langle n | \psi _ { i } ^ { ( 2 ) } \rangle = \frac { \langle n | v | \psi _ { i } ^ { ( 1 ) } \rangle } { \left( E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } \right) } - E _ { i } ^ { ( 1 ) } \frac { \langle n | \psi _ { i } ^ { ( 1 ) } \rangle } { \left( E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } \right) }
$$
二级波函数为：
$$
\langle n | \psi _ { i } ^ { ( 2 ) } \rangle = \frac { \langle n | v | \psi _ { i } ^ { ( 1 ) } \rangle } { \left( E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } \right) } - E _ { i } ^ { ( 1 ) } \frac { \langle n | \psi _ { i } ^ { ( 1 ) } \rangle } { \left( E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } \right) }
$$
三级能量为：
$$
\begin{aligned}
E _ { i } ^ { ( 3 ) } &= \langle i | v | \psi _ { i } ^ { ( 2 ) } \rangle \\ 
&= { \sum } ^ { \prime } \langle i | v | n \rangle \langle n | \psi _ { i } ^ { ( 2 ) } \rangle \\
&= { \sum _ { n } } ^ { \prime } \frac { \langle i | v | n \rangle \langle n | v | \psi _ { i } ^ { ( 1 ) } \rangle } { \left( E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } \right) } - E _ { i } ^ { ( 1 ) } { \sum _ { n } } ^ { \prime } \frac { \langle i | v | n \rangle \langle n | \psi _ { i } ^ { ( 1 ) } \rangle } { \left( E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } \right) }
\end{aligned}
$$

代入一级波函数后得到最终形式：
$$
E _ { i } ^ { ( 3 ) } = {\sum _ { n m }} ^ { \prime } \frac { \langle i | v | n \rangle \langle n | v | m \rangle \langle m | v | i \rangle } { \left( E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } \right) \left ( E _ { i } ^ { ( 0 ) } - E _ { m } ^ { ( 0 ) }  \right) } - E _ { i } ^ { ( 1 ) } {\sum _ { n }} ^ { \prime } \cdot \frac { \langle i | v | n \rangle \langle n | v | i \rangle } { \left( E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } \right) ^ { 2 } }
$$



> 与变分方法的联系：$H_0$的本征函数$\psi _ { i } ^ { ( 0 ) }$作为试探波函数
>
> 
>
> $E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } = 0$，不受扰动的能级简并，微扰法失效
>
> $\frac { \langle n | \nu | i \rangle } { E _ { i } ^ { ( 0 ) } - E _ { n } ^ { ( 0 ) } } \ll 1$时微扰法很好
>
> 
>
> 氦原子基态可，激发态不可
>
> 两个类氢原子1s 2s 左右交换 构造零级波函数，有简并
>
> 
>
> 外加电场 电场作为微扰
>
>  
>
> 简谐振子
>

### Application of Perturbation Theory to the Helium Atom                                                                                                                                                  将微扰法应用于氦原子

39页最后一公式

空间部分对称 相加 取1/sqrt2
$$
E _ { 0 } \approx E _ { 0 } ^ { ( 0 ) } + E _ { 0 } ^ { ( 1 ) } = - \frac { 1 } { 2 } Z ^ { 2 } - \frac { 1 } { 2 } Z ^ { 2 } + \frac { 5 } { 8 } Z = - Z ^ { 2 } + \frac { 5 } { 8 } Z = - 2.8477 \quad ( Z = 2 )
$$


> #### Example 7.3
>
> 箱中粒子
>
> 零级波函数和能量
>
> 一级能量
> $$
> E _ { n } ^ { ( 1 ) } = \int _ { 0 } ^ { a } \psi _ { n } ^ { ( 0 ) } * ( \frac { V _ { 0 } x } { a } ) \psi _ { n } ^ { ( 0 ) } d x = \frac { 2 V _ { 0 } } { a ^ { 2 } } \int _ { 0 } ^ { a } x \sin ^ { 2 } \frac { n \pi x } { a } d x = \frac { V _ { 0 } } { 2 }
> $$
> 
>
> 

---

## Mathchapter F: Matrices

### 1 Matrix

#### 1) The addition or subtraction rule
$$
C = A \pm B
$$
#### 2) The matrix multiplication rule

### 2 Some important definitions and properties of square matrices

#### 1) Diagonal matrix 对角矩阵

#### 2) The trace of the matrix A 迹

#### 3) The unit matrix 单位矩阵

$$
IA = AI = A
$$


#### 4) The inverse of the matrix A, denoted by A^-1^ 逆矩阵

#### 5) Unitary matrix 酉矩阵

#### 6) A Hermitian matrix is self-adjoint 厄密矩阵自共轭

## Mathchapter G: Matrix Eigenvalue Problems
$$
Hc=ESc
$$
> #### Example G1
>
> $$
> A = \begin{pmatrix} a & 1 \\ 1 & a \end{pmatrix}
> $$
>
> 

$$
D = \begin{pmatrix} 
\lambda & 1 &&\\
1 & \lambda &&\\ 
\lambda \\
\lambda \\
\end{pmatrix}
$$

相似变换
$$
D = C ^ { -1 } A C = C ^ { T } A C
$$
对角化A等效于解本征值问题



> #### Example G2
>
> 将G1中的矩阵对角化， i.e. $A = \begin{pmatrix} a & 1 \\ 1 & a \end{pmatrix}$
>
> 