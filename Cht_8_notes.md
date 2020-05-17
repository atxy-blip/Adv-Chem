# Chapter 8: Multielectron Atoms                                                                                                                                                                           第八章：多电子分子

本章将展现量子力学在原子的电子性质上的有力应用:heart_eyes:。

[toc]

## 8.1 Atomic and Molecular Calculations Are Expressed in Atomic Units                                                                                                    使用原子单位表示原子分子计算

原子单位Atomic units：

- Mass: the mass of an electron ($m_e$)
- Charge: the charge on a proton (e)
- Angular momentum: $\hbar$
- Length (Bohr radius):$a_0$
- Energy (a hartree) : $E _ { h } = \frac { m _ { e } e ^ { 4 } } { 16 \pi ^ { 2 } \varepsilon _ { 0 } ^ { 2 } \hbar ^ { 2 } }$



#### Table 8.1 Atomic Units and their SI equivalents

|      Quantity       |     Atomic Unit     |                        SI Equivalent                         |
| :-----------------: | :-----------------: | :----------------------------------------------------------: |
|        Mass         |        $m_e$        |           $9.1094 \times 10^{-31}{\,\mathrm{kg}}$            |
|       Charge        |         $e$         |            $1.6022 \times 10^{-19}{\,\mathrm{C}}$            |
|  Angular Momemtum   |       $\hbar$       |    $1.0546 \times 10^{-34}{\,\mathrm{J}\cdot\mathrm{s}}$     |
|       Length        |        $a_0$        |            $5.2918 \times 10^{-11}{\,\mathrm{m}}$            |
|       Energy        |        $E_h$        |            $4.3597 \times 10^{-18}{\,\mathrm{J}}$            |
| Permittivity 穿透性 | $4\pi\varepsilon_0$ | $1.1127 \times 10^{-19}{\,\mathrm{C^2}\cdot\mathrm{J^{-1}}\cdot\mathrm{m^{-1}}}$ |

氢原子

氦原子有两个核外电子，其哈密顿可以表示为
$$
\hat { H } = - \frac { \hbar ^ { 2 } } { 2 m _ { e } } \nabla _ { 1 } ^ { 2 } - \frac { \hbar ^ { 2 } } { 2 m _ { e } } \nabla _ { 2 } ^ { 2 } - \frac { 2 e ^ { 2 } } { 4 \pi \varepsilon _ { 0 } } \frac { 1 } { \vec{r} _ { 1 } } - \frac { 2 e ^ { 2 } } { 4 \pi \varepsilon _ { 0 } } \frac { 1 } { \vec{r} _ { 2 } } + \frac { e ^ { 2 } } { 4 \pi \varepsilon _ { 0 } } \cdot \frac { 1 } { r _ { 12 } }
$$

简写为：
$$
\hat { H } = - \frac { 1 } { 2 } \nabla _ { 1 } ^ { 2 } - \frac { 1 } { 2 } \nabla _ { 2 } ^ { 2 } - \frac { 2 } { \vec{r} _ { 1 } } - \frac { 2 } { \vec{r} _ { 2 } } +  \frac { 1 } { r _ { 12 } }
$$

$$
E=\iint=I_1+I_2+J_{12}
$$





原子

核
$$
\hat { H } = - \frac { m _ { e } } { 2 m _ { p } } \nabla _ { 1 } ^ { 2 }
$$


## 8.2 Both Perturbation Theory and the Variational Method Can Yield Excellent Results for Helium                                                                                                                                                  微扰法和变分法都能对氦原子做出好的结果

### Perturbation Theory 微扰法

$$
E = - Z ^ { 2 } + \frac { 5 } { 8 } Z = - \frac { 11 } { 4 } E _ { h } = - 2.750 E _ { h }
$$

高阶微扰能给出较精确的结果
$$
E = - Z ^ { 2 } + \frac { 5 } { 8 } Z - 0.15766 + \frac { 0.00870 } { Z } + \frac { 0.000889 } { Z } + \ldots . = - 2.9037 E _ { h }
$$



### Variational Method 变分法

$$
\Psi _ { 0 } = \psi _ { 1 s } \left ( \vec { r } _ { 1 } \right ) \psi _ { 1 s } \left ( \vec { r } _ { 2 } \right ) \frac { 1 } { \sqrt { 2 } } \left [ \alpha \left ( 1 \right ) \beta \left ( 2 \right ) - \beta \left ( 1 \right ) \alpha \left ( 2 \right ) \right ] \\
\psi _ { 1 s } \left ( \vec { r } _ { i } \right ) = \left ( \frac { Z ^ { 3 } } { \pi } \right ) ^ { \frac { 1 } { 2 } } e ^ { - Z r _ { i } } \\
E = - \left ( \frac { 27 } { 16 } \right ) ^ { 2 } E _ { h } = - 2.8477 E _ { h }
$$

电离能
$$
IE=E_{\text{He}^+} -E_{\text{He}}
$$
$0.9033E_h$

1AU=$627.5\, \mathrm{kcal} \cdot \mathrm{m}^{-1}$

## 8.3 An Electron Has An Intrinsic Spin Angular Momentum                                                                                                                   电子有内禀自旋角动量

### Spin Angular Momentum自旋角动量

电子的自旋不是经典的物理量

非相对论量子力学中作为假设引入

$$
\hat { L } ^ { 2 } , \hat { L } _ { x } , \hat { L } _ { y } , \hat { L } _ { z }
$$

$$
\hat { S } ^ { 2 } , \hat { S } _ { x } , \hat { S } _ { y } , \hat { S } _ { z }
$$

$$
\hat { S } ^ { 2 } = \hat { S } _ { x } ^ { 2 } + \hat { S } _ { y } ^ { 2 } + \hat { S } _ { z } ^ { 2 }
$$


$$
\left [ \hat{S}_y, \hat{S}_z \right ] = i \hbar \hat{S}_x;\quad
\left [ \hat{S}_z, \hat{S}_x \right ] = i \hbar \hat{S}_y;\quad
\left [ \hat{S}_x, \hat{S}_y \right ] = i \hbar \hat{S}_z \\ 
\left [ \hat{S}^2, \hat{S}_x \right ]=\left [ \hat{S}^2, \hat{S}_y \right ]=\left [ \hat{S}^2, \hat{S}_z \right ]=0
$$




### The Eigenvalues of $\hat { S } ^ { 2 }$ And $\hat { S } _ { z }$ (in Atomic Units) 原子单位制的自旋本征值

$$
\hat { S } ^ { 2 } Y = s \left ( s + 1 \right ) Y \quad s = 0 , \frac { 1 } { 2 } , 1, \frac { 3 } { 2 } , \cdots \\
\hat { S } _ { z } Y = m _ { s } Y \quad m _ { s } = - s , - s + 1 , \cdots , s - 1 , s
$$

其中s称为粒子的自旋。所有的电子都有1/2的自旋

两电子耦合 矢量长度固定，总自旋S取值0或1

电子自旋的本征函数为$\alpha, \beta$，分别对应$\frac { 1 } { 2 } , - \frac { 1 } { 2 }$的本征值。
$$
\hat { S } _ { z } \alpha = \frac { 1 } { 2 } \alpha \quad \hat { S } _ { z } \beta = - \frac { 1 } { 2 } \beta \\
\hat { S } ^ { 2 } \alpha = \frac { 3 } { 4 } \alpha \quad \hat { S } ^ { 2 } \beta = \frac { 3 } { 4 } \beta
$$


$$
\alpha: \left| \frac { 1 } { 2 } , \frac { 1 } { 2 } \right \rangle \quad
\beta: \left| \frac { 1 } { 2 } , - \frac { 1 } { 2 } \right \rangle
$$

第一个是s，第二个是ms Sz本征值

任何电子的自旋函数都可以表示为$C_1\alpha+C_2\beta$

The spin-up function: $\alpha(\sigma)$

The spin-down function: $\beta(\sigma)$

$\sigma$称为自旋变量

正交归一条件：
$$
\int \alpha ^ { * } \left ( \sigma \right ) \alpha \left ( \sigma \right ) d \sigma = \int \beta ^ { * } \left ( \sigma \right ) \beta \left ( \sigma \right ) d \sigma = 1 \\
\int \alpha ^ { * } \left ( \sigma \right ) \beta \left ( \sigma \right ) d \sigma = \int \beta ^ { * } \left ( \sigma \right ) \alpha \left ( \sigma \right ) d \sigma = 0
$$

### Ladder Operators for Electron Spin 电子自旋的梯形算符

自旋角动量的上升和下降算符为：
$$
\hat { S } _ { + } = \hat { S } _ { x } + i \hat { S } _ { y } \quad \hat { S } _ { - } = \hat { S } _ { x } - i \hat { S } _ { y }
$$

在原子单位中使用如下关系
$$
\hat { S } _ { + } | s , m _ { s } \rangle = \sqrt { \left ( s - m _ { s } \right ) \left ( s + m _ { s } + 1 \right ) } | s , m _ { s } + 1 \rangle \\ 
\hat { S } _ { - } | s , m _ { s } \rangle = \sqrt { \left ( s + m _ { s } \right ) \left ( s - m _ { s } + 1 \right ) } | s , m _ { s } - 1 \rangle
$$

有：
$$
\begin{aligned}
\hat { S } _ { + } | \alpha \rangle &= 0&
\hat { S } _ { + } | \beta \rangle &= \alpha \\
\hat { S } _ { - } | \alpha \rangle &= \beta &
\hat { S } _ { - } | \beta \rangle &= 0
\end{aligned}
$$
另有：
$$
\hat { S } ^ { 2 } = \hat { S } _ { + } \hat { S } _ { - } - \hat { S } _ { z } + \hat { S } _ { z } ^ { 2 } \quad \hat { S } ^ { 2 } = \hat { S } _ { - } \hat { S } _ { + } + \hat { S } _ { z } + \hat { S } _ { z } ^ { 2 }
$$


## 8.4 Addition of Angular Momenta 角动量的加和

$$

$$

### 1 The total angular momentum: $\hat{M}$ 总角动量

$$
\vec { M } = \vec { M } _ { 1 } + \vec { M } _ { 2 }
$$

总角动量有三个分量


$$
\hat { M } = \hat { M } _ { 1 } + \hat { M } _ { 2 }
$$
对于平方$\hat { M } ^ { 2 }$
$$
\hat { M } ^ { 2 } = \hat { M } \cdot \hat { M } = \hat { M } _ { x } ^ { 2 } + \hat { M } _ { y } ^ { 2 } + \hat { M } _ { z } ^ { 2 }
$$

$$
\hat { M } ^ { 2 } = \left ( \hat { M } _ { 1 } + \hat { M } _ { 2 } \right ) \cdot \left ( \hat { M } _ { 1 } + \hat { M } _ { 2 } \right ) 
= \hat { M } _ { 1 } ^ { 2 } + \hat { M } _ { 2 } ^ { 2 } + \hat { M } _ { 1 } \cdot \hat { M } _ { 2 } + \hat { M } _ { 2 } \cdot \hat { M } _ { 1 }
$$

由于$\hat { M } _ { 1 }, \hat { M } _ { 2 }$相互对易
$$
\begin{aligned}
\hat { M } ^ { 2 } &= \hat { M } _ { 1 } ^ { 2 } + \hat { M } _ { 2 } ^ { 2 } + 2 \hat { M } _ { 1 } \cdot \hat { M } _ { 2 } \\
 &= \hat { M } _ { 1 } ^ { 2 } + \hat { M } _ { 2 } ^ { 2 } + 2 \left ( \hat { M } _ { 1 x } \hat { M } _ { 2 x } + \hat { M } _ { 1 y } \hat { M } _ { 2 y } + \hat { M } _ { 1 z } \hat { M } _ { 2 z } \right ) \\
& = \hat { M } _ { 1 } ^ { 2 } + \hat { M } _ { 2 } ^ { 2 } + 2 \hat { M } _ { 1 } \hat { M } _ { 2 z } + \hat { M } _ { 1 } \hat { M } _ { 2 } + \hat { M } _ { 1 } \hat { M } _ { 2 + }
\end{aligned}
$$



### 2 The angular-momentum commutation relations 角动量互易关系

$$
\left [ \hat{M}_y, \hat{M}_z \right ] = i \hbar \hat{M}_x;\quad
\left [ \hat{M}_z, \hat{M}_x \right ] = i \hbar \hat{M}_y;\quad
\left [ \hat{M}_x, \hat{M}_y \right ] = i \hbar \hat{M}_z \\ 
\left [ \hat{M}^2, \hat{M}_x \right ]=\left [ \hat{M}^2, \hat{M}_y \right]= \left [ \hat{M}^2, \hat{M}_z \right ]=0
$$

> #### Proof
>
> $$
> \begin{aligned}
> \left [ \hat { M } _ { x } , \hat { M } _ { y } \right ] &= \left [ \hat { M } _ { 1 x } + \hat { M } _ { 2 x } , \hat { M } _ { 1 y } + \hat { M } _ { 2 y } \right ] \\
> & = \lfloor \hat { M } _ { 1 x } , \hat { M } _ { 1 y } + \hat { M } _ { 2 y } \rfloor + \lfloor \hat { M } _ { 2 x } , \hat { M } _ { 1 y } + \hat { M } _ { 2 y } \rfloor \\
> & = \left [ \hat { M } _ { 1 x } , \hat { M } _ { 1 y } \right ] + \left [ \hat { M } _ { 1 x } , \hat { M } _ { 2 y } \right ] + \left [ \hat { M } _ { 2 x } , \hat { M } _ { 1 y } \right ] + \left [ \hat { M } _ { 2 x } , \hat { M } _ { 2 y } \right ] \\
> & = i \hbar \hat { M } _ { 1 z } + i \hbar \hat { M } _ { 2 z } \\
> & = i \hbar \left ( \hat { M } _ { 1 z } + \hat { M } _ { 2 z } \right ) \\ 
> &= i \hbar \hat { M }
> \end{aligned}
> $$
>

因此可以同时确定平方和分量

此外还有
$$
 \left [ \hat { M } _ { 1 } ^ { 2 } , \hat { M } _ { z } \right ] = 0 \quad \left [ \hat { M } _ { 2 } ^ { 2 } , \hat { M } _ { z } \right ] = 0 \quad \left [ \hat { M } _ { 1 } ^ { 2 } , \hat { M } ^ { 2 } \right ] = 0 \\ \left [ \hat { M } _ { 2 } ^ { 2 } , \hat { M } ^ { 2 } \right ] = 0 \quad \hat { M } _ { 1 } ^ { 2 } , \hat { M } _ { 2 } ^ { 2 } = 0 
$$
四个算符有共同本征函数，写作$| j _ { 1 } j _ { 2 } J M _ { J } \rangle$，根据对易关系式推出本征值
$$
\hat { M } _ { 1 } ^ { 2 } | j _ { 1 } j _ { 2 } J M _ { j } \rangle = j _ { 1 } \left ( j _ { 1 } + 1 \right ) | j _ { 1 } j _ { 2 } J M _ { J } \rangle \\
\hat { M } _ { 2 } ^ { 2 } | j _ { 1 } j _ { 2 } J M _ { J } \rangle = j _ { 2 } \left ( j _ { 2 } + 1 \right ) | j _ { 1 } j _ { 2 } J M _ { J } \rangle \\
\hat { M } ^ { 2 } | j _ { 1 } j _ { 2 } J M _ { J } \rangle = J \left ( J + 1 \right ) | j _ { 1 } j _ { 2 } J M _ { J } \rangle \quad J = 0 , \frac { 1 } { 2 } , 1, \cdots \\
\hat { M } _ { z } | j _ { 1 } j _ { 2 } J M _ { J } \rangle = M _ { J } | j _ { 1 } j _ { 2 } J M _ { J } \rangle \quad M _ { J } = - J , - J + 1 , \cdots , J
$$




$$
\begin{aligned}
\hat { M } _ { z } | j _ { 1 } j _ { 2 } J M _ { J } \rangle &= M _ { J } \sum _ { m _ { 1 } , m _ { 2 } } c \left ( j _ { 1 } j _ { 2 } J M _ { J } ; m _ { 1 } m _ { 2 } \right ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle \\
&= \sum _ { m _ { 1 } , m _ { 2 } } c \left ( j _ { 1 } j _ { 2 } J M _ { J } ; m _ { 1 } m _ { 2 } \right ) M _ { J } | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle \\
\hat { M } _ { z } | j _ { 1 } j _ { 2 } J M _ { j } \rangle &= \hat { M } _ { z } \sum _ { m _ { 1 } , m _ { 2 } } c \left ( j _ { 1 } j _ { 2 } J M _ { j } ; m _ { 1 } m _ { 2 } \right ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle \\
&= \left ( \hat { M } _ { 1 z } + \hat { M } _ { 2 z } \right ) \sum _ { m _ { 1 } , m _ { 2 } } c \left ( j _ { 1 } j _ { 2 } J M _ { j } ; m _ { 1 } m _ { 2 } \right ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle \\
&= \sum _ { m _ { 1 } , m _ { 2 } } c \left ( j _ { 1 } j _ { 2 } J M _ { j } ; m _ { 1 } m _ { 2 } \right ) \left ( m _ { 1 } + m _ { 2 } \right ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle
\end{aligned}
$$
$M_J=m_1+m_2$

### 3 The eigenvalues and eigenfunctions of $\hat { M } ^ { 2 }, \hat { M } _ { z }$ 角动量算符的本征值和本征函数

$| j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle$

本征函数为$| j _ { 1 } j _ { 2 } J M _ { J } \rangle$
$$
| j _ { 1 } j _ { 2 } J M _ { J } \rangle = \sum _ { m _ { 1 } , m _ { 2 } ,\\ m _ { 1 } + m _ { 2 } = M _ { 1 } } c \left ( j _ { 1 } j _ { 2 } J M _ { J } ; m _ { 1 } m _ { 2 } \right ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle
$$
线性组合多个状态，得到想要的本征值函数

$\left ( j _ { 1 } j _ { 2 } J M _ { J } ; m _ { 1 } m _ { 2 } \right )$ Clebsch-Gordan (CG)系数

展开表达式
$$
\begin{aligned}
\hat { M } _ { z } | j _ { 1 } j _ { 2 } J M _ { j } \rangle 
&= M _ { j } \sum _ { m _ { 1 } , m _ { 2 } } c \left ( j _ { 1 } j _ { 2 } J M _ { j } ; m _ { 1 } m _ { 2 } \right ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle \\ &= \sum c \left ( j _ { 1 } j _ { 2 } J M _ { j } ; m _ { 1 } m _ { 2 } \right ) M _ { J } | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle 
\end{aligned}
$$

$$
\begin{aligned} 
\hat { M } _ { z } | j _ { 1 } j _ { 2 } J M _ { j } \rangle &= \hat { M } _ { z } \sum _ { m _ { 1 } , m _ { 2 } } c \left ( j _ { 1 } j _ { 2 } J M _ { j } ; m _ { 1 } m _ { 2 } \right ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle \\ 
&= \left ( \hat { M } _ { 1 z } + \hat { M } _ { 2 } \right ) \sum _ { m _ { 1 } m _ { 2 } } c \left ( j _ { 1 } j _ { 2 } J M _ { j } ; m _ { 1 } m _ { 2 } \right ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle \\
&= \sum _ { m _ { 1 } , m _ { 2 } } c \left ( j _ { 1 } j _ { 2 } J M _ { j } ; m _ { 1 } m _ { 2 } \right ) \left ( m _ { 1 } + m _ { 2 } \right ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle
\end{aligned}
$$

$M _ { J } = m _ { 1 } + m _ { 2 }$

两粒子体系的角动量

$J=j_1+j_2,j_1+j_2-1,\cdots,|j_1-j_2|$

角动量耦合 z分量-J到J

两电子体系总自旋取值

> #### Proof
>
> $$
> M _ { J } = m _ { 1 } + m _ { 2 } = j_1+j_2
> $$
>
> ##### 1
>
> MJ从-J到J J最大=j1+j2
>
> ##### 2
>
> 第二大的 线性组合 得到新的态
>
> ##### 3
>
> 确立最小值 总状态数$\left (2j_1+1\right )\left (2j_2+1\right )$
> $$
> \left ( 2 j _ { 1 } + 1 \right ) \left ( 2 j _ { 2 } + 1 \right ) = \sum _ { J = J _ { \min } } ^ { J _ { \max } } \left ( 2 J + 1 \right ) = \left ( J _ { \max } + 1 \right ) ^ { 2 } - J _ { \min } ^ { 2 }
> $$
>
> $$
> J _ { \min } ^ { 2 } = \left (j_1-j_2\right )^ { 2 } \quad \Rightarrow \quad J _ { \min } = |j_1-j_2|
> $$
>

> #### Example 8.1
>
> 3个电子 j1=1 j2=2 j3=3
>
> j1+j2 3 2 1
>
> +j3 6 5 4 3 2 1 0 5 4 3 2 1 4 3 2

### 4 How to construct the eigenfunctions $| j _ { 1 } j _ { 2 } J M _ { J } \rangle$ 如何构建本征函数

$| j _ { 1 } j _ { 2 } J M _ { J } \rangle$可被简化为$| J M _ { J } \rangle$，可进行如下分组
$$
\begin{aligned}
&j_1+j_2 & j_1+j_2-1 \\
&| j _ { 1 } +j _ { 2 }, j _ { 1 } +j _ { 2 }\rangle
\end{aligned}
$$

$$
\left ( 2 j _ { 1 } + 1 \right ) \left ( 2 j _ { 2 } + 1 \right ) = \sum _ { J = J _ { \min } } ^ { J _ { \max } } \left ( 2 J + 1 \right ) = \left ( J _ { \max } + 1 \right ) ^ { 2 } - J _ { \min } ^ { 2 }
$$

#### The Top State in the First Column

易证$| j _ { 1 } +j _ { 2 }, j _ { 1 } +j _ { 2 }\rangle=| j _ { 1 } j _ { 1 } \rangle| j _ { 2 }j _ { 2 }\rangle$

类比$\hat { S } _ { - } | s , m _ { s } \rangle = \sqrt { \left ( s + m _ { s } \right ) \left ( s - m _ { s } + 1 \right ) } | s , m _ { s } - 1 \rangle$可得：
$$
\hat { M } _ { - } | j _ { 1 } + j _ { 2 } ,\ j _ { 1 } + j _ { 2 } \rangle = \sqrt { 2 ( j _ { 1 } + j _ { 2 } ) } | j _ { 1 } + j _ { 2 } ,\ j _ { 1 } + j _ { 2 } - 1 \rangle
$$
其中$\hat{M}_{-}=\left(\hat{M}_{1-}+\hat{M}_{2-}\right)$，移项得
$$
\begin{aligned}
\left|j_{1}+j_{2}, j_{1}+j_{2}-1\right\rangle &=\frac{1}{\sqrt{2\left(j_{1}+j_{2}\right)}} \hat{M}_{-}\left|j_{1}+j_{2}, j_{1}+j_{2}\right\rangle \\
&=\frac{1}{\sqrt{2\left(j_{1}+j_{2}\right)}}\left(\hat{M}_{1-}+\hat{M}_{2-}\right)\left|j_{1} j_{1}\right\rangle\left|j_{2} j_{2}\right\rangle \\
&=\sqrt{\frac{j_{1}}{j_{1}+j_{2}}}\left|j_{1}\left(j_{1}-1\right)\right\rangle\left|j_{2} j_{2}\right\rangle+\sqrt{\frac{j_{2}}{j_{1}+j_{2}}}\left|j_{1} j_{1}\right\rangle\left|j_{2}\left(j_{2}-1\right)\right\rangle
\end{aligned}
$$

#### The Top State in the Second Column

$$
\left|j_{1}+j_{2}-1, j_{1}+j_{2}-1\right\rangle
$$

$\left|j_{1} j_{1}\right\rangle\left|j_{2}\left(j_{2}-1\right)\right\rangle,\ \left|j_{1}\left(j_{1}-1\right)\right\rangle\left|j_{2} j_{2}\right\rangle$

两个态正交 区别在于第一列是+，第二列是-
$$
\left|j_{1}+j_{2}-1, j_{1}+j_{2}-1\right\rangle = \sqrt { \frac { j _ { 1 } } { j _ { 1 } + j _ { 2 } } } | j _ { 1 } j _ { 1 } \rangle | j _ { 2 } \left ( j _ { 2 } - 1 \right ) \rangle - \sqrt { \frac { j _ { 2 } } { j _ { 1 } + j _ { 2 } } } | j _ { 1 } \left ( j _ { 1 } - 1 \right ) \rangle | j _ { 2 } j _ { 2 } \rangle
$$

### 5 Eigenvalues and eigenfunctions of two–electron spin functions                                                                                                                                        两电子自旋体系的本征值和本征函数

$\hat { S } _ { 1 } , \hat { S } _ { 2 } , \hat { S } ^ { 2 } , \hat { S } _ { z }$

$| s _ { 1 } s _ { 2 } S M _ { s } \rangle$可被简化为$| S M _ { s } \rangle$
$$
\begin{aligned}
 &S& M _ { s }  && | S M _ { s } \rangle jhb\\
 &S=1(\text{Triplet}) &jhbj& &jgbbh

\end{aligned}
$$

$$
| S M _ { s } \rangle = C _ { 1 } \alpha ( 1 ) \alpha ( 2 ) + C _ { 2 } \alpha ( 1 ) \beta ( 2 ) + C _ { 3 } \beta ( 1 ) \alpha ( 2 ) + C _ { 4 } \beta ( 1 ) \beta ( 2 )
$$

$$
\begin{align}
    u  &= \arctan x             &  dv &= 1 \, dx  \\ 
    du &= \frac{1}{1 + x^2}dx  &  v  &= x.
\end{align}
$$



> #### Example 8.2
>
> 证明$| 11 \rangle = \alpha ( 1 ) \alpha ( 2 )$。
> $$
> \hat { S } ^ { 2 } = \hat { S } _ { 1 } ^ { 2 } + \hat { S } _ { 2 } ^ { 2 } + 2 \hat { S } _ { 1 z } \hat { S } _ { 2 z } + ( \hat { S } _ { 1 + } \hat { S } _ { 2 - } + \hat { S } _ { 1 - } \hat { S } _ { 2 + } )
> $$
> 
> $$
> \begin{aligned}
> \hat{S}^{2} \alpha(1) \alpha(2) &=\left[\hat{S}_{1}^{2}+\hat{S}_{2}^{2}+2 \hat{S}_{12} \hat{S}_{2 z}+\left(\hat{S}_{1} \hat{S}_{2-}+\hat{S}_{1} \hat{S}_{2+}\right)\right] \alpha(1) \alpha(2) \\
> &=\left[\frac{3}{4}+\frac{3}{4}+2 \times \frac{1}{4}+0\right] \alpha(1) \alpha(2) \\
> &=2 \alpha(1) \alpha(2)=s(s+1) \alpha(1) \alpha(2)
> \end{aligned}
> $$
> s=1
> $$
> { \hat { S } _ { z } \alpha ( 1 ) \alpha ( 2 ) = ( \hat { S } _ { 1 z } + \hat { S } _ { 2 z } ) \alpha ( 1 ) \alpha ( 2 ) }{ = ( \frac { 1 } { 2 } + \frac { 1 } { 2 } ) \alpha ( 1 ) \alpha ( 2 ) = \alpha ( 1 ) \alpha ( 2 ) = M _ { s } \alpha ( 1 ) \alpha ( 2 ) }
> $$
>
> $$
> | 11 \rangle = \alpha ( 1 ) \alpha ( 2 )
> $$
>
> 



## 8.5 Wave Functions Must Be Antisymmetric in the Interchange of Any Two Electrons                                                                                                                                                                                         在任意两个电子的交换中波函数必须是反对称的

自旋轨道是表示电子空间分布和自旋的波函数

#### Postulate 6

All electronic wave functions must be antisymmetric under the interchange of any two electrons.

$$
\left. { \Psi _ { 1 } \left ( 1,2 \right ) = \psi \left ( 1,2 \right ) + \psi \left ( 2,1 \right ) = 1 s \alpha \left ( 1 \right ) 1 s \beta \left ( 2 \right ) + 1 s \alpha \left ( 2 \right ) 1 s \beta \left ( 1 \right ) } \\ 
{ \Psi _ { 2 } \left ( 1,2 \right ) = \psi \left ( 1,2 \right ) - \psi \left ( 2,1 \right ) = 1 s \alpha \left ( 1 \right ) 1 s \beta \left ( 2 \right ) - 1 s \alpha \left ( 2 \right ) 1 s \beta \left ( 1 \right ) } \right.
$$

上面一个相加的形式不满足反对称的要求
$$
\left. { \psi \left ( 1,2 \right ) = 1 s \left ( 1 \right ) \alpha \left ( 1 \right ) 1 s \left ( 2 \right ) \beta \left ( 2 \right ) \equiv 1 s \alpha \left ( 1 \right ) 1 s \beta \left ( 2 \right ) } \\ 
{ \psi \left ( 2,1 \right ) = 1 s \alpha \left ( 2 \right ) 1 s \beta \left ( 1 \right ) } \right.
$$

描述氦原子
$$
\Psi _ { 2 } \left ( 2,1 \right ) = - \Psi _ { 2 } \left ( 1,2 \right )
$$

锂原子1s2 2s1 就1s两个反对称 2s一个电子自旋自由

## 8.6 Antisymmetric Wave Functions Can Be Represented by Slater Determinants                                                                                                                                                                         用斯莱特行列式表示反对称波函数

MIT Slater 

用行列式表示
$$
\begin{aligned}
\Psi \left ( 1,2 \right ) &= \begin{vmatrix} { 1 s \alpha \left ( 1 \right ) } & { 1 s \beta \left ( 1 \right ) } \\ { 1 s \alpha \left ( 2 \right ) } & { 1 s \beta \left ( 2 \right ) }\end{vmatrix} \\
&= 1 s \left ( 1 \right ) \alpha \left ( 1 \right ) s \left ( 2 \right ) \beta \left ( 2 \right ) - 1 s \left ( 1 \right ) \beta \left ( 1 \right ) 1 s \left ( 2 \right ) \alpha \left ( 2 \right ) \\ 
&= 1 s \left ( 1 \right ) 1 s \left ( 2 \right ) \left [ \alpha \left ( 1 \right ) \beta \left ( 2 \right ) - \beta \left ( 1 \right ) \alpha \left ( 2 \right ) \right ]
\end{aligned}
$$

描述的是00单重态 空间部分对称，自旋部分反对称

基态三重态，则是+，自旋部分对称，空间部分不是反对称，不可能

激发态 1s 2s 可以构造三重态$1 s \left ( 1 \right ) 2 s \left ( 2 \right ) -1 s \left ( 2 \right ) 2 s \left ( 1 \right )$

归一化
$$
\Psi \left ( 1,2 \right ) = \frac{1}{\sqrt{2}}\begin{vmatrix} { 1 s \alpha \left ( 1 \right ) } & { 1 s \beta \left ( 1 \right ) } \\ { 1 s \alpha \left ( 2 \right ) } & { 1 s \beta \left ( 2 \right ) }\end{vmatrix}
$$

N电子体系波函数 行：电子 列：自旋轨道
$$
\Psi\left (1,2, \ldots, N\right )=\frac{1}{\sqrt{N !}}\begin{vmatrix}
\chi_{1}\left (1\right ) & \chi_{2}\left (1\right ) & \dots & \chi_{N}\left (1\right ) \\
\chi_{1}\left (2\right ) & \chi_{2}\left (2\right ) & \dots & \chi_{N}\left (2\right ) \\
\vdots & \vdots & \ddots & \vdots \\
\chi_{1}\left (N\right ) & \chi_{2}\left (N\right ) & \dots & \chi_{N}\left (N\right )
\end{vmatrix}
$$

交换两个电子的坐标，可以看出行列式是反对称的
$$
\Psi\left (2,1, \ldots, N\right )=\frac{1}{\sqrt{N !}}\begin{vmatrix}
\chi_{1}\left (2\right ) & \chi_{2}\left (2\right ) & \dots & \chi_{N}\left (2\right ) \\
\chi_{1}\left (1\right ) & \chi_{2}\left (1\right ) & \dots & \chi_{N}\left (1\right ) \\
\vdots & \vdots & \ddots & \vdots \\
\chi_{1}\left (N\right ) & \chi_{2}\left (N\right ) & \dots & \chi_{N}\left (N\right )
\end{vmatrix}=-\Psi\left (1,2, \ldots, N\right )
$$

使用对角元简写为$\Psi = | \chi _ { 1 } \chi _ { 2 } \cdots \chi _ { N } \rangle$

如果两列相等，行列式为零，波函数不存在

#### Pauli Exclusion Principle 泡利不相容原理

No two electrons in an atom or a molecule can have the same spin orbital.

## 8.7 The Hartree-Fock Method

独立粒子近似 平均场 类似于变分法

两句话描述：

1. 体系波函数用一个行列式描述，这个行列式由一组正交归一的自旋轨道组成。

2. 根据限制求行列式对应的泛函的最小期望值，得到的一组方程。

$$
| \psi _ { 0 } \rangle = | \chi _ { 1 } \chi _ { 2 } \cdots \chi _ { N } \rangle
$$

the Slater-Condon rule
$$
E _ { 0 } \left [ \{ \alpha _ { a } \} \right ] = \langle \psi _ { 0 } | \hat { H } | \psi _ { 0 } \rangle = \sum _ { a = 1 } ^ { N } \langle \chi _ { a } | h | \chi _ { a } \rangle + \frac { 1 } { 2 } \sum _ { a } ^ { N } \sum _ { b } ^ { N } \left [ \langle \chi _ { a } \chi _ { b } | \chi _ { a } \chi _ { b } \rangle - \langle \chi _ { a } \chi _ { b } | \chi _ { b } \chi _ { a } \rangle \right ]
$$

$$
\langle \chi _ { a } | h | \chi _ { a } \rangle = \int d \vec { x } _ { 1 } \chi _ { a } ^ { * } \left ( 1 \right ) h \left ( 1 \right ) \chi _ { a } \left ( 1 \right )
$$

$$
\langle \chi _ { a } \chi _ { b } | \chi _ { a } \chi _ { b } \rangle = \int d x _ { 1 } d \vec { x } _ { 2 } \chi _ { a } ^ { * } \left ( 1 \right ) \chi _ { b } ^ { * } \left ( 2 \right ) r _ { 12 } ^ { - 1 } \chi _ { a } \left ( 1 \right ) \chi _ { b } \left ( 2 \right )
$$

泛函是函数的函数 

使用限制$\int d \vec { x } _ { 1 } \chi _ { a } ^ { * } \left ( 1 \right ) \chi _ { b } \left ( 1 \right ) = \delta _ { a b }$求$E _ { 0 } \left [ \{ \chi _ { a } \} \right ]$的最小值

canonical HF equation:

$$
f | \chi _ { a } \rangle = \varepsilon _ { a } | \chi _ { a } \rangle \quad \text { or } \quad f \left ( 1 \right ) \chi _ { a } \left ( 1 \right ) = \varepsilon _ { a } \chi _ { a } \left ( 1 \right )
$$

$$
f \left ( 1 \right ) = h \left ( 1 \right ) + \sum _ { b } \left [ J _ { b } \left ( 1 \right ) - K _ { b } \left ( 1 \right ) \right ] = h \left ( 1 \right ) + v ^ { \text{HF} } \left ( 1 \right )
$$

$$
v ^ { \text{HF} } \left ( 1 \right ) = \sum _ { b } \left [ J _ { b } \left ( 1 \right ) - K _ { b } \left ( 1 \right ) \right ]
$$

$v ^ { \text{HF} } \left ( 1 \right )$有效单电子势，有两项，库伦算符和交换算符 每次解一个方程就可以

库伦算符the Coulomb operator：
$$
J _ { b } \left ( 1 \right ) = \int d \vec { x } _ { 2 } | \chi _ { b } \left ( 2 \right ) | ^ { 2 } r _ { 12 } ^ { - 1 } \\
J _ { b } \left ( 1 \right ) \chi _ { a } \left ( 1 \right ) = \left [ \int d \vec { x } _ { 2 } \chi _ { b } ^ { * } \left ( 2 \right ) r _ { 12 } ^ { - 1 } \chi _ { b } \left ( 2 \right ) \right ] \chi _ { a } \left ( 1 \right )
$$

(1)表示只与电子1有关 两个电子的相互作用

交换算符：
$$
K _ { b } \left ( 1 \right ) = \left [ \int d \vec { x } _ { 2 } \chi _ { b } ^ { * } \left ( 2 \right ) r _ { 12 } ^ { - 1 } P _ { 12 } \chi _ { b } \left ( 2 \right ) \right] \\
$$

$$
K _ { b } \left ( 1 \right ) \chi _ { a } \left ( 1 \right ) = \left [ \int d \vec { x } _ { 2 } \chi _ { b } ^ { * } \left ( 2 \right ) r _ { 12 } ^ { - 1 } P _ { 12 } \chi _ { b } \left ( 2 \right ) \right] \chi _ { a } \left ( 1 \right ) \\
= \left [ \int d \vec { x } _ { 2 } \chi _ { b } ^ { * } \left ( 2 \right ) r _ { 12 } ^ { - 1 } \chi _ { a } \left ( 2 \right ) \right] \chi _ { b } \left ( 1 \right )
$$


$$
\langle \chi _ { a } \left ( 1 \right ) J _ { b } \left ( 1 \right ) \rangle \chi _ { a } \left ( 1 \right ) \rangle = \int d x _ { 1 } d \vec { x } _ { 2 } \chi _ { a } ^ { * } \left ( 1 \right ) \chi _ { b } ^ { * } \left ( 2 \right ) r _ { 12 } ^ { - 1 } \chi _ { a } \left ( 1 \right ) \chi _ { b } \left ( 2 \right ) = \langle a b | a b \rangle \\
\langle \chi _ { a } \left ( 1 \right ) | K _ { b } \left ( 1 \right ) \rangle _ { a } \left ( 1 \right ) \rangle = \int d \vec { x } _ { 1 } d \vec { x } _ { 2 } \chi _ { a } ^ { * } \left ( 1 \right ) \chi _ { b } ^ { * } \left ( 2 \right ) r _ { 12 } ^ { - 1 } \chi _ { b } \left ( 1 \right ) \chi _ { a } \left ( 2 \right ) = \langle a b | b a \rangle
$$

$\varepsilon _ { i }$：与$\chi_i$有关的自旋轨道能量

$$
\varepsilon _ { a } = \langle \chi _ { a } | f | \chi _ { a } \rangle = \langle a | h | a \rangle + \sum _ { L } \langle a b \| a b \rangle
$$

$$
E _ { 0 } = \sum _ { a } ^ { N } \langle a | h | a \rangle + \frac { 1 } { 2 } \sum _ { a } ^ { N } \sum _ { b } ^ { N } \langle a b \| a b \rangle \left ( \neq \sum _ { a } ^ { N } \varepsilon _ { a } \right )
$$



此方法有多个变种：

### Restricted HF (RHF)

每个空间轨道被偶数个电子占据（双占据） 闭壳层
$$
\chi _ { i } \left ( \vec { x } \right ) = \begin{cases} 
{ \psi _ { j } \left ( \vec { r } \right ) \alpha \left ( \sigma \right ) } \\ 
{ \psi _ { j } \left ( \vec { r } \right ) \beta \left ( \sigma \right ) }
\end{cases}
$$

行列式为 有横线的是beta电子，没有的是alpha电子
$$
| \psi _ { 0 } \rangle = | \chi _ { 1 } \chi _ { 2 } \cdots \chi _ { N } \rangle = \left | \psi _ { 1 } \overline { \psi } _ { 1 } \cdots \psi _ { a } \overline { \psi } _ { a } \cdots \psi _ { N / 2 } \overline { \psi } _ { N / 2 } \right \rangle
$$

$$
f \left ( \vec { r } _ { 1 } \right ) \psi _ { j } \left ( \vec { r } _ { 1 } \right ) = \varepsilon _ { j } \psi _ { j } \left ( \vec { r } _ { 1 } \right )
$$

### Restricted open-shell HF (ROHF)

奇数个电子 除了双占据的轨道外，还有一个或多个占据的轨道

最后一项是一个alpha电子
$$
| \psi _ { 0 } \rangle = | \chi _ { 1 } \chi _ { 2 } \cdots \chi _ { N } \rangle = | \psi _ { 1 } \overline { \psi } _ { 1 } \cdots \psi _ { a } \overline { \psi } _ { a } \cdots { \psi } _ { N / 2 } \rangle
$$

$$
f \left ( \vec { r } _ { 1 } \right ) \psi _ { j } \left ( \vec { r } _ { 1 } \right ) = \varepsilon _ { j } \psi _ { j } \left ( \vec { r } _ { 1 } \right )
$$

### Unrestricted HF (UHF)

有两套空间轨道，一套装alpha电子，另一套装beta电子

psi2不相等
$$
\Psi _ { \text{UHF} } = \left | \psi _ { 1 } ^ { \alpha } \overline { \psi _ { 1 } ^ { \beta } } \psi _ { 2 } ^ { \alpha } \overline { \psi _ { 2 } ^ { \beta } } \cdots \right \rangle
$$

有两套HF方程
$$
f ^ { \alpha } \left ( 1 \right ) \psi _ { j } ^ { \alpha } \left ( 1 \right ) = \varepsilon _ { j } ^ { \alpha } \psi _ { j } ^ { \alpha } \left ( 1 \right ) ; \quad f ^ { \beta } \left ( 1 \right ) \psi _ { j } ^ { \beta } \left ( 1 \right ) = \varepsilon _ { j } ^ { \beta } \psi _ { j } ^ { \beta } \left ( 1 \right )
$$

锂原子有3个电子 ROHF 1s装两个电子 或UHF 1s a 1s b

用UHF表示 轨道标号 空间部分不一样 2s alpha 同样是1s有 alpha beta psi1改成1s

UHF有自旋污染 不是本征函数 只能说近似单态或近似三态 RHF是纯的



He原子 RHF $| \psi _ { 1s } \overline { \psi } _ { 1s } \psi _ { 2s } \overline { \psi } _ { 2s } \rangle$

### Hartree‒Fock‒Roothaan Equation

线性变分原理
$$

$$

Hartree‒Fock‒Roothaan Equation
$$
\sum F _ { \mu \nu } c _ { \nu } = \varepsilon \sum S _ { \mu \nu } c _ { \nu } \quad \text { or } \quad F c = \varepsilon S c
$$

矩阵
$$
S _ { \mu \nu } = \int d \vec { r } _ { 1 } \phi _ { u } ^ { * } \left ( \vec { r } _ { 1 } \right ) \phi _ { v } \left ( \vec { r } _ { 1 } \right ) \quad F _ { i v } = \int d \vec { r } _ { 1 } \phi _ { u } ^ { * } \left ( 1 \right ) f \left ( 1 \right ) \phi _ { v } \left ( 1 \right )
$$

解不止一个，使用下标进行区分， ci是列向量
$$
F c_i = \varepsilon_i S c_i
$$

$$
\vec{C} = \begin{pmatrix} { \vec{c} ^ { 1 } } &{ \vec{c} ^ { 2 } } &\cdots &{ \vec{c} ^ { N } } \end{pmatrix} =
\begin{pmatrix}
{ c _ { 11 } } & { c _ { 11 } } &\cdots & { c _ { N1 } } \\ 
{ c _ { 12 } } & { c _ { 22 } } &\cdots & { c _ { N2 } } \\
\vdots &\vdots &\ddots &\vdots \\
{ c _ { 1N } } & { c _ { 2N } } &\cdots & { c _ { NN } }
\end{pmatrix} \quad \varepsilon=\begin{pmatrix}
{ E _ { 1 } } &&& \\ & { E _ { 2 } } && \\ && \ddots & \\
&&& { E _ { N } }\end{pmatrix}
$$

$$
F^{\prime} C^{\prime} = C^{\prime} E
$$

解HF方程得到一组轨道和它的轨道

轨道能量的物理意义

#### Koopman’s Theorem

$$
{ IP = {^ { N - 1 } E _ { i }} - {^ { N } E _ { 0 }} = - \varepsilon _ { i } } \\ { EA = {^ { N } E _ { 0 }} - {^ { N + 1 } E ^ { r }} = - \varepsilon _ r }
$$

电离是把电子打掉 变成自由电子 吸收的能量 第i个轨道电离能 占据轨道occupied orbital 电离能等于轨道能量的负值

得到电子 填到新的轨道 第r个轨道电子亲和能 空轨道virtual orbital

光电子能谱 打掉电子测量光谱

计算结果与实验结果吻合得很好



对两个分子进行HF计算 a的电子跑到b上

### The Building-up Principle 构造原理

又称the Aufbau principle，将电子按轨道能量从低到高往上排。

$$
1s \quad 2s \quad 2p \quad 3s \quad 3p \quad 4s \quad 3d \quad 4p \quad 5s \quad 4d \quad 5p \quad 6s \quad \cdots
$$
对多电子原子，2s和2p的简并性被打破

此原理并不绝对 比如Xenon

> 2个$4f$电子有$C_{14}^{2}=91$个不同状态。

### What Is Missing in the HF Method?

一部分库伦相互作用没有考虑

相关能
$$
CE=E_{EXACT}-E_{HF}
$$
post-HF

## 8.8 A Term Symbol Gives A Detailed Description of An Electron Configuration  光谱项给出电子组态的精确描述

总角动量 总自旋角动量The total orbital angular momentum and total spin angular momentum are given by the vector sums
$$
\vec{L}=\sum_{i}\vec{l}_i \quad \vec{S}=\sum_{i}\vec{s}_i
$$
The z components of L and S are given by scalar sums
$$
L _ { z } = \sum _ { i } l _ { i z } = \sum _ { i } m _ { i l } = M _ { L } \quad S _ { z } = \sum _ { i } s _ { i k } = \sum _ { i } m _ { i s } = M
$$
The total angular momentum J is given by
$$
J=L+S
$$
and the z component is
$$
J _ { z } = L _ { z } + S _ { z } = M _ { L } + M _ { S } = M
$$
原子谱项atomic term的定义为:
$$
^{2S+1}L_{J}
$$
$L$: total orbital angular momentum; $S$: total spin angular momentum; $J$: total angular momentum

2S+1 自旋多重度

|  L   |  0   |  1   |  2   |  3   |  4   |  5   |  6   |  7   |  8  |  9  |
| :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: | :--: |:--: |:--: |
|      | S | P | D | F | G | H | I | J | K | L |

原子谱项的简并度$(2L+1)(2S+1)$

### The configuration of a closed subshell: $^{1}S$

$^{1}S$
$$
\Psi = | 1 s \alpha \ 1 s \beta |
$$

### Two electrons in different subshells

Find the possible values of L from l 1 and l 2 ;and the possible value of S from s 1 and s 2 .For an electronic configuration: 1s 2 2s 2 2p 1 3d 1We only need to consider two subshells, 2p 1 3d 1(l 1 =1, l 2 =2 , s 1 =1/2, s 2 =1/2) L=3,2,1; S=0,1

l1l2对应p和d轨道

角动量耦合规则

原子谱项为 $\ce{^1P ^1D ^1 F ^3 P ^3 D ^3 F}$

For this configuration, the wave function is a linear combination of 60 determinants. Each term corresponds to an energy level.
$$
\Psi = \sum _ { i } C _ { i } D _ { i } \quad D _ { 1 } = | 1 s \alpha\ 1 s \beta\ 2 s \alpha\ 2 s \beta\ 2 p _ { + 1 } \alpha\ 3 d _ { + 2 } \alpha |
$$

2p13d1能级 f3 21重简并

###  Two electrons in the same subshell

Take 1s 2 2s 2 2p 2 (the ground state of carbon) as an example.

| $M_S\downarrow\ M_L\rightarrow$ |              0              |  1   |  2   |
| :---: | :-------------------------: | :--: | :--: |
|   1   |                             |  $|p_1\ \alpha\ p_0\ \alpha|$  |   $|p_1\ \alpha\ p_{-1}\ \alpha|$   |
|   0   | $|p_1\ \alpha\ p_1\ \beta|$ | $|p_1\ \alpha\ p_0\ \beta| \\ |p_0\ \alpha\ p_1\ \beta|$ | $|p_1\ \alpha\ p_{-1}\ \beta| \\ |p_{-1}\ \alpha\ p_1\ \beta| \\|p_0\ \alpha\ p_0\ \beta|$ |

一共15个行列式

Pauli不相容，有些不存在

### Steps for Identifying Term Symbols

1. Write out all possible unique determinants with non-negative M L and M S values and arrange them into groups.

2. Identify the highest M S value in the box, and for all determinants with this M S value, find out the highest M L value.

3. For this S and L combination, the term symbol is 3 P.

4. Because the level with quantum numbers L and S contains determinants, one must remove from the original box this number of determinants to get a new Table.



5. After deleting four entries, one can obtain the following Table and returns to step 2 and carries out the process again.

| $M_S\downarrow\ M_L\rightarrow$ |              0              |              1              |                             2                              |
| :-----------------------------: | :-------------------------: | :-------------------------: | :--------------------------------------------------------: |
|                1                |                             |                             |                                                            |
|                0                | $|p_1\ \alpha\ p_1\ \beta|$ | $|p_0\ \alpha\ p_1\ \beta|$ | $|p_{-1}\ \alpha\ p_1\ \beta| \\|p_0\ \alpha\ p_0\ \beta|$ |



> #### Example 8.3
>
> 

## 8.9 The Allowed Values of J are L+S, L+S-1, …, |L-S|

The values of J for the term symbols can be determined in terms
of the values of L and S，
$$
J=L+S
$$

$$
J = L + S , L + S - 1 , L + S - 2 , \ldots , | L - S |
$$

If spin-orbit coupling is present, the terms will further split into levels.

3F3 7重简并

加上J后 p2 3P分裂成3个 210 1D j=2 1S 0 有5个能级



钠原子 3s1谱项 自旋多重度2 L=0 S2 J=1/2  doubletP J=1/2 3/2

## 8.10 Hund’s Rules Are Used to Determine the Term Symbol of the Ground Electronic State

### Hund’s Rules

## 8.11 Atomic Term Symbols Are Used to Describe Atomic Spectra

Atomic spectral lines can be assigned to transitions between energy
levels described by atomic term symbols. The fine structure of
atomic spectra lines is caused by the spin-orbital coupling.

The Hamiltonian of a multielectron atom can be written as:
$$
\hat { H } = - \frac { 1 } { 2 } \sum _ { j } \nabla _ { j } ^ { 2 } - \sum _ { j } \frac { Z } { r _ { j } } + \sum _ { i < j } \frac { 1 } { r _ { i j } } + \sum _ { j } \xi ( r _ { j } ) l _ { j } \cdot s _ { j }
$$
The last term describes the spin-orbital coupling. One can express the Hamiltonian into the following form,
$$
\hat { H } = \hat { H } _ {0} + \hat { H } _ {\text{S.O.}}
$$

### The Spin-Orbit Interaction Term

$$
\hat { H } _ { \text{S.O.}} = \sum _ { i } \xi _ { i } ( r _ { i } ) \hat { L } _ { i } \cdot \hat { S } _ { i } \quad \hat { H } = \hat { H } _ { 0 } + \hat { H } _ { \text{S.O.} }
$$

It is difficult to find the eigenfunctions and eigenvalues of the operator.
The effect of the spin-orbit interaction term is usually estimated with first-order perturbation theory.
$$
\vec {J} = \vec {L} + \vec {S}
$$

$$
\left. { \hat { L } \cdot \hat { S } = \frac { 1 } { 2 } ( \hat { J } ^ { 2 } - \hat { L } ^ { 2 } - \hat { S } ^ { 2 } ) } \\ { \hat { L } \cdot \hat { S } \Psi = \frac { 1 } { 2 } [ J ( J + 1 ) - L ( L + 1 ) - S ( S + 1 ) ] \Psi } \right.
$$

确定量
$$
E _ { n } ^ { ( 1 ) } = \int \psi _ { n } ^ { ( 0 ) * } \hat { H } _ { S O } ^ { ( 1 ) } \psi _ { n } ^ { ( 0 ) } d \tau
$$

$$
\hat { H } _ { S O } ^ { ( 1 ) } = \frac { Z } { 2 ( 137 ) ^ { 2 } } \frac { 1 } { r ^ { 3 } } \hat { l } \cdot \hat { S }
$$

$$
E _ { n } ^ { ( 1 ) } = \frac { 1 } { 2 } \{ j ( j + 1 ) - l ( l + 1 ) - s ( s + 1 ) \} \frac { Z } { 2 ( 137 ) ^ { 2 } } \langle \frac { 1 } { r ^ { 3 } } \rangle
$$

$$
\langle \frac { 1 } { r ^ { 3 } } \rangle = \frac { Z ^ { 3 } } { n ^ { 3 } l ( l + 1 ) ( l + \frac { 1 } { 2 } ) }
$$

$$
E _ { n } ^ { ( 1 ) } = \frac { Z ^ { 4 } } { 2 ( 137 ) ^ { 2 } n ^ { 3 } } \frac { \{ j ( j + 1 ) - l ( l + 1 ) - s ( s + 1 ) \} } { 2 l ( l + 1 ) ( l + \frac { 1 } { 2 } ) } \quad \text { a. } u
$$

$$
E _ { s o . } = \frac { 1 } { 2 } A [ J ( J + 1 ) - L ( L + 1 ) - S ( S + 1 ) ]
$$

### The spin-orbital effect is important in heavier atoms

旋轨耦合作用强的时候微扰法失效 荧光和磷光

# Supplementary Material 补充材料

## The Derivation of the Hartree-Fock Equation

### 1 Functional variation

试探波函数
$$
E(\widetilde{\Phi}) =\langle \widetilde{\Phi}|\hat{H}|\widetilde{\Phi}\rangle 
$$


$$
\tilde { \Phi } \rightarrow \tilde { \Phi } + \delta \tilde { \Phi } \quad ( \tilde { \Phi } ^ { * } \rightarrow \tilde { \Phi } ^ { * } + \delta \tilde { \Phi } ^ { * } )
$$

$$
\begin{aligned}
E(\widetilde{\Phi}+\delta \widetilde{\Phi}) &=\langle\widetilde{\Phi}+\delta \widetilde{\Phi}|\hat{H}| \widetilde{\Phi}+\delta \widetilde{\Phi}\rangle \\
&=E(\widetilde{\Phi})+\langle\delta \widetilde{\Phi} \hat{H} \widetilde{\Phi}\rangle+\langle\widetilde{\Phi} \hat{H} | \delta \widetilde{\Phi}\rangle\}+\ldots \\
&=E(\widetilde{\Phi})+\delta E+\cdots
\end{aligned}
$$

一阶泛函=0
$$
\delta E = \langle \delta \tilde { \Phi } | \hat { H } | \tilde { \Phi } \rangle + \langle \tilde { \Phi } | \hat { H } | \delta \tilde { \Phi } \rangle = 0
$$

stationary point

### 2 Minimization of the energy of a single determinant

单一轨道$| \psi _ { 0 } \rangle = | \chi _ { 1 } \chi _ { 2 } \cdots \chi _ { N } \rangle$

中括弧代替尖括弧，意义一样
$$
E _ { 0 } = \langle \psi _ { 0 } | \hat { H } | \psi _ { 0 } \rangle = \sum _ { a = 1 } ^ { N } [ a | h | a ] + \frac { 1 } { 2 } \sum _ { a } ^ { N } \sum _ { b } ^ { N } ( [ a a | b b ] - [ a b | b a ] ) = E _ { 0 } [ \{ \chi _ { a } \} ]
$$

$$
[ a | h | a ] = \int d \vec { x } _ { 1 } \chi _ { a } ^ { * } ( 1 ) h \chi _ { a } ( 1 )
$$

$$
[ a a | b b ] = \int d \vec { x } _ { 1 } d \vec { x } _ { 2 } \chi _ { a } ^ { * } ( 1 ) \chi _ { a } ( 1 ) r _ { 12 } ^ { - 1 } \chi _ { b } ^ { * } ( 2 ) \chi _ { b } ( 2 )
$$

E看成一组轨道的泛函 泛函的极值问题，约束条件为$\int d \overline { x } _ { 1 } \chi _ { a } ^ { * } ( 1 ) \chi _ { b } ( 1 ) = [ a | b ] = \delta _ { a b }$

构建新的关于自旋轨道的泛函$L [ \{ \chi _ { a } \} ]$，将有约束条件的变分问题转化为没有约束的
$$
L [ \{ \chi _ { a } \} ] = E _ { 0 } [ \{ \chi _ { a } \} ] - \sum _ { a = 1 } ^ { N } \sum _ { b = 1 } ^ { N } \varepsilon _ { ba } ( [ a | b ] - \delta _ { a b } )
$$

拉格朗日量

L是实数
$$
\begin{aligned}
L ^ { * } &= E _ { 0 } [ \{ \chi _ { a } \} ] - \sum _ { a = 1 } ^ { N } \sum _ { b = 1 } ^ { N } \varepsilon _ { b a } ^ { * } ( [ a | b ] ^ { * } - \delta _ { a b } ) \\
&= E _ { 0 } [ \{ \chi _ { a } \} ] - \sum _ { a = 1 } ^ { N } \sum _ { b = 1 } ^ { N } \varepsilon _ { a b } ^ { * } ( [ b | a ] ^ { * } - \delta _ { a b } ) \\
&= E _ { 0 } [ \{ \chi _ { a } \} ] - \sum _ { a = 1 } ^ { N } \sum _ { b = 1 } ^ { N } \varepsilon _ { a b } ^ { * } ( [ a | b ] - \delta _ { a b } )
\end{aligned}
$$

$\varepsilon _ { ba } =\varepsilon _ { a b } ^ { * }$ 酉矩阵 积分指标的交换

令$\chi _ { a } \rightarrow \chi _ { a } + \delta \chi _ { a }$，计算一阶变分
$$
\delta [ a | b ] = \delta \int d \vec { x } _ { 1 } \chi _ { a } ^ { * } ( 1 ) \chi _ { b } ( 1 ) = [ \delta \chi _ { a } | \chi _ { b } ] + [ \chi _ { a } | \delta \chi _ { b } ]
$$

$$
\begin{aligned}
\delta E _ { 0 } &= \sum _ { i = 1 } ^ { N } ( [ \delta \chi _ { a } | h | \chi _ { a } ] + [ \chi _ { a } | h | \delta \chi _ { a } ] )\\
&+ \frac { 1 } { 2 } \sum _ { a = 1 } ^ { N } \sum _ { b = 1 } ^ { N } ( [ \delta \chi _ { a } \chi _ { a } | \chi _ { b } \chi _ { b } ] + [ \chi _ { a } \delta \chi _ { a } | \chi _ { b } \chi _ { b } ] + [ \chi _ { a } \chi _ { a } | \delta \chi _ { b } \chi _ { b } ] + [ \chi _ { a } \chi _ { a } | \chi _ { b } \delta \chi _ { b } ] ) \\
&- \frac { 1 } { 2 } \sum _ { a = 1 } ^ { N } \sum _ { b = 1 } ^ { N } ( [ \delta \chi _ { a } \chi _ { b } | \chi _ { b } \chi _ { a } ] + [ \chi _ { a } \delta \chi _ { b } | \chi _ { b } \chi _ { a } ] + [ \chi _ { a } \chi _ { b } | \delta \chi _ { b } \chi _ { a } ] + [ \chi _ { a } \chi _ { b } | \chi _ { b } \delta \chi _ { a } ] )
\end{aligned}
$$

运用交换ab的关系 第二行第一项第三项相等
$$
\frac { 1 } { 2 } \sum _ { a = 1 } ^ { N } \sum _ { b = 1 } ^ { N } [ \chi _ { a } \chi _ { a } | \delta \chi _ { b } \chi _ { b } ] = \frac { 1 } { 2 } \sum _ { a = 1 } ^ { N } \sum _ { b = 1 } ^ { N } [ \delta \chi _ { b } \chi _ { b } | \chi _ { a } \chi _ { a } ] = \frac { 1 } { 2 } \sum _ { a = 1 } ^ { N } \sum _ { b = 1 } ^ { N } [ \delta \chi _ { a } \chi _ { a } | \chi _ { b } \chi _ { b } ]
$$

复共轭关系
$$
[ \chi _ { a } \delta \chi _ { a } | \chi _ { b } \chi _ { b } ] = [ \delta \chi _ { a } \chi _ { a } | \chi _ { b } \chi _ { b } ] ^ { * }
$$

$$
\sum _ { a = 1 } ^ { N } \sum _ { b = 1 } ^ { N } [ \chi _ { a } \delta \chi _ { b } | \chi _ { b } \chi _ { a } ] = \sum _ { a } \sum _ { b } [ \chi _ { b } \delta \chi _ { a } | \chi _ { a } \chi _ { b } ]
= \left \{ \sum _ { a } \sum _ { b } [ \delta \chi _ { a } \chi _ { b } | \chi _ { b } \chi _ { a } ] \right \} ^ {*}
$$

C.C. = complex conjugate
$$
\delta E _ { 0 } = \sum _ { a = 1 } ^ { N } [ \delta \chi _ { a } | h | \chi _ { a } ] + \sum _ { a = 1 } ^ { N } \sum _ { b = 1 } ^ { N } [ \delta \chi _ { a } \chi _ { a } | \chi _ { b } \chi _ { b } ] - \sum _ { a = 1 } ^ { N } \sum _ { b = 1 } ^ { N } [ \delta \chi _ { a } \chi _ { b } | \chi _ { b } \chi _ { a } ] + \rm{C.C.}
$$

约束条件项 交换第二项的标记
$$
\begin{aligned}
\sum_{a b} \varepsilon_{b a} \delta[a | b] &=\sum_{a b} \varepsilon_{b a}\left[\delta \chi_{a} | \chi_{b}\right]+\sum_{a b} \varepsilon_{b a}\left[\chi_{a} | \delta \chi_{b}\right] \\
&=\sum_{a b} \varepsilon_{b a}\left[\delta \chi_{a} | \chi_{b}\right]+\sum_{a b} \varepsilon_{a b}\left[\chi_{b} | \delta \chi_{a}\right] \\
&=\sum_{a b} \varepsilon_{b a}\left[\delta \chi_{a} | \chi_{b}\right]+\sum_{a b} \varepsilon_{b a}^{*}\left[\delta \chi_{a} | \chi_{b}\right]^{*} \\
&=\sum_{a b} \varepsilon_{b a}\left[\delta \chi_{a} | \chi_{b}\right]+\rm{C.C.}
\end{aligned}
$$

得到
$$
\begin{aligned}
\delta_{L}=&\delta_{E_{0}}-\sum_{a=1}^{N} \sum_{b=1}^{N} \varepsilon_{b a} \delta[a | b] \\
=&\sum_{a=1}^{N}\left[\delta \chi_{a}|h| \chi_{a}\right]+\sum_{a=1}^{N} \sum_{b=1}^{N}\left(\left[\delta \chi_{a} \chi_{a} | \chi_{b} \chi_{b}\right]-\left[\delta \chi_{a} \chi_{b} | \chi_{b} \chi_{a}\right]\right) \\ 
&-\sum_{a=1}^{N} \sum_{b=1}^{N} \varepsilon_{b a}\left[\delta \chi_{a} | \chi_{b}\right]+\rm{C.C.} =0
\end{aligned}
$$

双电子积分变为有效单电子

引入库伦算符$J_b(1)$

电子在chib2运动会有库仑相互作用

交换算符$K_b(1)$



用库伦算符和交换算符重写
$$
\delta _ { L } = \sum _ { a = 1 } ^ { N } \int d \vec { x } _ { 1 } \delta \chi _ { a } ^ { * } ( 1 ) \left[ h ( 1 ) \chi _ { a } ( 1 ) + \sum _ { b = 1 } ^ { N } ( J _ { b } ( 1 ) - K _ { b } ( 1 ) ) \chi _ { a } ( 1 ) - \sum _ { b = 1 } ^ { N } \varepsilon _ { b a } \chi _ { b } ( 1 ) \right]+\rm{C.C.}=0
$$
任意的$\delta \chi _ { a } ^ { * } ( 1 )$

引入Fock算符$f$
$$
f ( 1 ) = h ( 1 ) + \sum _ { b } ( J _ { b } ( 1 ) - K _ { b } ( 1 ) )
$$
变化为
$$
f ( 1 ) \chi _ { a } ( 1 ) = \sum _ { b = 1 } ^ { N } \varepsilon _ { b a } \chi _ { b } ( 1 ) \quad \text { or } \quad f | \chi _ { a } \rangle = \sum _ { b = 1 } ^ { N } \varepsilon _ { b a } | \chi _ { b } \rangle
$$

### 3 The canonical HF equation 正则

#### 1

$$
\begin{aligned}
\left\langle\chi_{a}^{\prime} | \chi_{c}^{\prime}\right\rangle &=\left\langle\sum_{b} \chi_{b} U_{b a} | \sum_{d} \chi_{d} U_{d c}\right\rangle \\
&=\sum_{b} \sum U_{b q}^{*} U_{d c} \underbrace{\left\langle\chi_{b} | \chi_{d}\right\rangle}_{=\delta_{M}} \\
&=\sum_{b} U_{b a}^{*} U_{b c}=\sum_{b}\left(U^{+}\right)_{a b} U_{b c}\\
&=\left(U^{+} U\right)_{a c}=\delta_{a c} \\
\left\langle\chi_{a}| \chi_{c}\right\rangle&=\delta_{ac}
\end{aligned}
$$


$$
\begin{aligned}
{A}^{\prime}=\begin{pmatrix}
TODO
\end{pmatrix}
\end{aligned}
$$

$$
\det({A}^{\prime})=\det(AU)=\det(A)\det(U)
$$

$U^+U=I$
$$
\det(U^+U)=\det(U^+)\det(U)
$$

#### 2

$$
f ( 1 ) = h ( 1 ) + \sum _ { b } ( J _ { b } ( 1 ) - K _ { b } ( 1 ) )
$$

跟轨道没关系，不需讨论
$$
\begin{aligned}
\sum_{a} J_{a}^{\prime}(1) &=\sum_{a} \int d \vec{x}_{2} \chi_{a}^{* *}(2) r_{12}^{-1} \chi_{a}^{\prime}(2) \\
&=\sum_{a} \int d \vec{x}_{2}\left(\sum_{b} \chi_{b}^{*}(2) U_{b a}^{*}\right) r_{12}^{-1}\left(\sum_{c} \chi_{c}(2) U_{c a}\right) \\
&=\sum_{b c}\left[\sum_{a} U_{b a}^{*} U_{c a}\right] \int d \vec{x}_{2} \chi_{b}^{*}(2) r_{12}^{-1} \chi_{c}(2)\\
&=\sum_{b c}\left[\delta_{b c}\right] \int d \vec{x}_{2} \chi_{b}^{*}(2) r_{12}^{-1} \chi_{c}(2) \\
&=\sum_{b} \int d \vec{x}_{2} \chi_{b}^{*}(2) r_{12}^{-1} \chi_{b}(2)=\sum_{b} J_{b}(1)
\end{aligned}
$$
提取求和指标

用这个关系
$$
\sum _ { a } U _ { b a } ^ { * } U _ { c a } = \sum _ { a } ( U ^ { + } ) _ { a b } U _ { c a } = \sum _ { a } U _ { c a } ( U ^ { + } ) _ { a b } = ( U U ^ { + } ) _ { c b } = \delta _ { cb }
$$
做U变换后fock算符不变

#### 3

$$

$$


$$
\begin{aligned}
\varepsilon_{b a}^{\prime}&= \int d \vec{x}_{1}\left[\chi_{b}^{\prime}(1)\right]^{*} f(1) \chi_{a}^{\prime}(1) \\
&=\sum_{c d} U_{d b}^{*} U_{c a} \int d \vec{x}_{1} \chi_{d}^{*}(1) f(1) \chi_{c}(1) \\
&=\sum_{c d} U_{d b}^{*} \varepsilon_{d c} U_{c a}\\
&=\sum_{c d}\left(U^{+}\right)_{b d} \varepsilon_{d c} U_{c a} \\
&=\left(U^{+} \varepsilon U\right)_{b a}
\end{aligned}
$$

$$
f\left| \chi_{a}\right\rangle=\varepsilon_{a} \left| \chi_{a}\right\rangle
$$

This set of spin orbitals is called the set of canonical (正则）spin orbitals, which are generally be delocalized over an atom (or a molecule)

否则没有轨道能量的概念