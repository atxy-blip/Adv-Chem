# Chapter 8: Multielectron Atoms                                                                                                                                                                           第八章：多电子分子

本章将展现量子力学在原子的电子性质上的有力应用:heart_eyes:。

[toc]

## 8.1 Atomic and Molecular Calculations Are Expressed in Atomic Units                                                                                                    使用原子单位表示原子分子计算

原子单位Atomic units：

- Mass: the mass of an electron ($m_e$ )
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

氦原子
$$
\hat { H } = - \frac { \hbar ^ { 2 } } { 2 m _ { e } } \nabla _ { 1 } ^ { 2 } - \frac { \hbar ^ { 2 } } { 2 m _ { e } } \nabla _ { 2 } ^ { 2 } - \frac { 2 e ^ { 2 } } { 4 \pi \varepsilon _ { 0 } } \frac { 1 } { \vec{r} _ { 1 } } - \frac { 2 e ^ { 2 } } { 4 \pi \varepsilon _ { 0 } } \frac { 1 } { \vec{r} _ { 2 } } + \frac { e ^ { 2 } } { 4 \pi \varepsilon _ { 0 } } \cdot \frac { 1 } { r _ { 12 } }
$$

简写为：
$$
\hat { H } = - \frac { 1 } { 2 } \nabla _ { 1 } ^ { 2 } - \frac { 1 } { 2 } \nabla _ { 2 } ^ { 2 } - \frac { 2 } { \vec{r} _ { 1 } } - \frac { 2 } { \vec{r} _ { 2 } } +  \frac { 1 } { r _ { 12 } }
$$

锂原子

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
\Psi _ { 0 } = \psi _ { 1 s } ( \vec { r } _ { 1 } ) \psi _ { 1 s } ( \vec { r } _ { 2 } ) \frac { 1 } { \sqrt { 2 } } [ \alpha ( 1 ) \beta ( 2 ) - \beta ( 1 ) \alpha ( 2 ) ] \\
\psi _ { 1 s } ( \vec { r } _ { i } ) = ( \frac { Z ^ { 3 } } { \pi } ) ^ { \frac { 1 } { 2 } } e ^ { - Z r _ { i } } \\
E = - ( \frac { 27 } { 16 } ) ^ { 2 } E _ { h } = - 2.8477 E _ { h }
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




### The Eigenvalues of $\hat { S } ^ { 2 }$ And $\hat { S } _ { z }$ (in Atomic Units) 原子单位制的本征值

$$
\hat { S } ^ { 2 } Y = s ( s + 1 ) Y \quad s = 0 , \frac { 1 } { 2 } , 1, \frac { 3 } { 2 } , \cdots \\
\hat { S } _ { z } Y = m _ { s } Y \quad m _ { s } = - s , - s + 1 , \cdots , s - 1 , s
$$

s称为粒子的自旋
$$
\hat { S } _ { + } = \hat { S } _ { x } + i \hat { S } _ { y } \quad \hat { S } _ { - } = \hat { S } _ { x } - i \hat { S } _ { y }
$$

$$
\alpha: \left| \frac { 1 } { 2 } , \frac { 1 } { 2 } \right \rangle \quad
\beta: \left| \frac { 1 } { 2 } , - \frac { 1 } { 2 } \right \rangle
$$

第一个是s，第二个是ms Sz本征值
$$
\int \alpha ^ { * } ( \sigma ) \alpha ( \sigma ) d \sigma = \int \beta ^ { * } ( \sigma ) \beta ( \sigma ) d \sigma = 1 \\
\int \alpha ^ { * } ( \sigma ) \beta ( \sigma ) d \sigma = \int \beta ^ { * } ( \sigma ) \alpha ( \sigma ) d \sigma = 0
$$



### Ladder Operators for Electron Spin 电子自旋的梯形算符


在原子单位中使用如下关系
$$
\hat { S } _ { + } | s , m _ { s } \rangle = \sqrt { ( s - m _ { s } ) ( s + m _ { s } + 1 ) } | s , m _ { s } + 1 \rangle \\ 
\hat { S } _ { - } | s , m _ { s } \rangle = \sqrt { ( s + m _ { s } ) ( s - m _ { s } + 1 ) } | s , m _ { s } - 1 \rangle
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
\hat { M } ^ { 2 } = ( \hat { M } _ { 1 } + \hat { M } _ { 2 } ) \cdot ( \hat { M } _ { 1 } + \hat { M } _ { 2 } ) 
= \hat { M } _ { 1 } ^ { 2 } + \hat { M } _ { 2 } ^ { 2 } + \hat { M } _ { 1 } \cdot \hat { M } _ { 2 } + \hat { M } _ { 2 } \cdot \hat { M } _ { 1 }
$$

由于$\hat { M } _ { 1 }, \hat { M } _ { 2 }$相互对易
$$
\begin{aligned}
\hat { M } ^ { 2 } &= \hat { M } _ { 1 } ^ { 2 } + \hat { M } _ { 2 } ^ { 2 } + 2 \hat { M } _ { 1 } \cdot \hat { M } _ { 2 } \\
 &= \hat { M } _ { 1 } ^ { 2 } + \hat { M } _ { 2 } ^ { 2 } + 2 ( \hat { M } _ { 1 x } \hat { M } _ { 2 x } + \hat { M } _ { 1 y } \hat { M } _ { 2 y } + \hat { M } _ { 1 z } \hat { M } _ { 2 z } ) \\
& = \hat { M } _ { 1 } ^ { 2 } + \hat { M } _ { 2 } ^ { 2 } + 2 \hat { M } _ { 1 } \hat { M } _ { 2 z } + \hat { M } _ { 1 } \hat { M } _ { 2 } + \hat { M } _ { 1 } \hat { M } _ { 2 + }
\end{aligned}
$$



### 2 The angular-momentum commutation relations 角动量互易关系

$$
\left [ \hat{M}_y, \hat{M}_z \right ] = i \hbar \hat{M}_x;\quad
\left [ \hat{M}_z, \hat{M}_x \right ] = i \hbar \hat{M}_y;\quad
\left [ \hat{M}_x, \hat{M}_y \right ] = i \hbar \hat{M}_z \\ 
\left [ \hat{M}^2, \hat{M}_x \right ]=\left [ \hat{M}^2, \hat{M}_y \right ]=\left [ \hat{M}^2, \hat{M}_z \right ]=0
$$

> #### Proof
>
> $$
> \begin{aligned}
> \left [ \hat { M } _ { x } , \hat { M } _ { y } \right ] &= \left [ \hat { M } _ { 1 x } + \hat { M } _ { 2 x } , \hat { M } _ { 1 y } + \hat { M } _ { 2 y } \right ] \\
> & = \lfloor \hat { M } _ { 1 x } , \hat { M } _ { 1 y } + \hat { M } _ { 2 y } \rfloor + \lfloor \hat { M } _ { 2 x } , \hat { M } _ { 1 y } + \hat { M } _ { 2 y } \rfloor \\
> & = [ \hat { M } _ { 1 x } , \hat { M } _ { 1 y } ] + [ \hat { M } _ { 1 x } , \hat { M } _ { 2 y } ] + [ \hat { M } _ { 2 x } , \hat { M } _ { 1 y } ] + [ \hat { M } _ { 2 x } , \hat { M } _ { 2 y } ] \\
> & = i \hbar \hat { M } _ { 1 z } + i \hbar \hat { M } _ { 2 z } \\
> & = i \hbar ( \hat { M } _ { 1 z } + \hat { M } _ { 2 z } ) \\ 
> &= i \hbar \hat { M }
> \end{aligned}
> $$
>

因此可以同时确定平方和分量

此外还有
$$
 [ \hat { M } _ { 1 } ^ { 2 } , \hat { M } _ { z } ] = 0 \quad [ \hat { M } _ { 2 } ^ { 2 } , \hat { M } _ { z } ] = 0 \quad [ \hat { M } _ { 1 } ^ { 2 } , \hat { M } ^ { 2 } ] = 0 \\ [ \hat { M } _ { 2 } ^ { 2 } , \hat { M } ^ { 2 } ] = 0 \quad \hat { M } _ { 1 } ^ { 2 } , \hat { M } _ { 2 } ^ { 2 } = 0 
$$
四个算符有共同本征函数，写作$| j _ { 1 } j _ { 2 } J M _ { J } \rangle$，根据对易关系式推出本征值
$$
\hat { M } _ { 1 } ^ { 2 } | j _ { 1 } j _ { 2 } J M _ { j } \rangle = j _ { 1 } ( j _ { 1 } + 1 ) | j _ { 1 } j _ { 2 } J M _ { J } \rangle \\
\hat { M } _ { 2 } ^ { 2 } | j _ { 1 } j _ { 2 } J M _ { J } \rangle = j _ { 2 } ( j _ { 2 } + 1 ) | j _ { 1 } j _ { 2 } J M _ { J } \rangle \\
\hat { M } ^ { 2 } | j _ { 1 } j _ { 2 } J M _ { J } \rangle = J ( J + 1 ) | j _ { 1 } j _ { 2 } J M _ { J } \rangle \quad J = 0 , \frac { 1 } { 2 } , 1, \cdots \\
\hat { M } _ { z } | j _ { 1 } j _ { 2 } J M _ { J } \rangle = M _ { J } | j _ { 1 } j _ { 2 } J M _ { J } \rangle \quad M _ { J } = - J , - J + 1 , \cdots , J
$$




$$
\begin{aligned}
\hat { M } _ { z } | j _ { 1 } j _ { 2 } J M _ { J } \rangle &= M _ { J } \sum _ { m _ { 1 } , m _ { 2 } } c ( j _ { 1 } j _ { 2 } J M _ { J } ; m _ { 1 } m _ { 2 } ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle \\
&= \sum _ { m _ { 1 } , m _ { 2 } } c ( j _ { 1 } j _ { 2 } J M _ { J } ; m _ { 1 } m _ { 2 } ) M _ { J } | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle \\
\hat { M } _ { z } | j _ { 1 } j _ { 2 } J M _ { j } \rangle &= \hat { M } _ { z } \sum _ { m _ { 1 } , m _ { 2 } } c ( j _ { 1 } j _ { 2 } J M _ { j } ; m _ { 1 } m _ { 2 } ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle \\
&= ( \hat { M } _ { 1 z } + \hat { M } _ { 2 z } ) \sum _ { m _ { 1 } , m _ { 2 } } c ( j _ { 1 } j _ { 2 } J M _ { j } ; m _ { 1 } m _ { 2 } ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle \\
&= \sum _ { m _ { 1 } , m _ { 2 } } c ( j _ { 1 } j _ { 2 } J M _ { j } ; m _ { 1 } m _ { 2 } ) ( m _ { 1 } + m _ { 2 } ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle
\end{aligned}
$$
$M_J=m_1+m_2$

### 3 The eigenvalues and eigenfunctions of $\hat { M } ^ { 2 }, \hat { M } _ { z }$ 角动量算符的本征值和本征函数

$| j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle$

本征函数为$| j _ { 1 } j _ { 2 } J M _ { J } \rangle$
$$
| j _ { 1 } j _ { 2 } J M _ { J } \rangle = \sum _ { m _ { 1 } , m _ { 2 } , m _ { 1 } + m _ { 2 } = M _ { 1 } } c ( j _ { 1 } j _ { 2 } J M _ { J } ; m _ { 1 } m _ { 2 } ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle
$$
线性组合多个状态，得到想要的本征值函数

$( j _ { 1 } j _ { 2 } J M _ { J } ; m _ { 1 } m _ { 2 } )$ Clebsch-Gordan(CG)系数

展开表达式
$$
\begin{aligned}
\hat { M } _ { z } | j _ { 1 } j _ { 2 } J M _ { j } \rangle 
&= M _ { j } \sum _ { m _ { 1 } , m _ { 2 } } c ( j _ { 1 } j _ { 2 } J M _ { j } ; m _ { 1 } m _ { 2 } ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle \\ &= \sum c ( j _ { 1 } j _ { 2 } J M _ { j } ; m _ { 1 } m _ { 2 } ) M _ { J } | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle 
\end{aligned}
$$

$$
\begin{aligned} 
\hat { M } _ { z } | j _ { 1 } j _ { 2 } J M _ { j } \rangle &= \hat { M } _ { z } \sum _ { m _ { 1 } , m _ { 2 } } c ( j _ { 1 } j _ { 2 } J M _ { j } ; m _ { 1 } m _ { 2 } ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle \\ 
&= ( \hat { M } _ { 1 z } + \hat { M } _ { 2 } ) \sum _ { m _ { 1 } m _ { 2 } } c ( j _ { 1 } j _ { 2 } J M _ { j } ; m _ { 1 } m _ { 2 } ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle \\
&= \sum _ { m _ { 1 } , m _ { 2 } } c ( j _ { 1 } j _ { 2 } J M _ { j } ; m _ { 1 } m _ { 2 } ) ( m _ { 1 } + m _ { 2 } ) | j _ { 1 } m _ { 1 } \rangle | j _ { 2 } m _ { 2 } \rangle
\end{aligned}
$$

$M _ { J } = m _ { 1 } + m _ { 2 }$

$J=j_1+j_2,j_1+j_2-1,\cdots,|j_1-j_2|$

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
> 确立最小值 总状态数$(2j_1+1)(2j_2+1)$
> $$
> ( 2 j _ { 1 } + 1 ) ( 2 j _ { 2 } + 1 ) = \sum _ { J = J _ { \min } } ^ { J _ { \max } } ( 2 J + 1 ) = ( J _ { \max } + 1 ) ^ { 2 } - J _ { \min } ^ { 2 }
> $$
>
> $$
> J _ { \min } ^ { 2 } = (j_1-j_2)^ { 2 } \quad \Rightarrow \quad J _ { \min } = |j_1-j_2|
> $$
>
> 

### 4 How to construct the eigenfunctions 如何构建本征函数

$$
( 2 j _ { 1 } + 1 ) ( 2 j _ { 2 } + 1 ) = \sum _ { J = J _ { \min } } ^ { J _ { \max } } ( 2 J + 1 ) = ( J _ { \max } + 1 ) ^ { 2 } - J _ { \min } ^ { 2 }
$$

#### The Top State in the First Column



#### The Top State in the Second Column

$$
| j _ { 1 } + j _ { 2 } - 1 , j _ { 1 } + j _ { 2 } - 1 \rangle = \sqrt { \frac { j _ { 1 } } { j _ { 1 } + j _ { 2 } } } | j _ { 1 } j _ { 1 } \rangle | j _ { 2 } ( j _ { 2 } - 1 ) \rangle - \sqrt { \frac { j _ { 2 } } { j _ { 1 } + j _ { 2 } } } | j _ { 1 } ( j _ { 1 } - 1 ) \rangle | j _ { 2 } j _ { 2 } \rangle
$$

### 5 Eigenvalues and eigenfunctions of two–electron spin functions



> #### Example 8.2



## 8.5 Wave Functions Must Be Antisymmetric in the Interchange of Any Two Electrons                                                                                                                                                                                         在任意两个电子的交换中波函数必须是反对称的

$$
\left. { \psi ( 1,2 ) = 1 s ( 1 ) \alpha ( 1 ) 1 s ( 2 ) \beta ( 2 ) \equiv 1 s \alpha ( 1 ) 1 s \beta ( 2 ) } \\ 
{ \psi ( 2,1 ) = 1 s \alpha ( 2 ) 1 s \beta ( 1 ) } \right.
$$



$$
\left. { \Psi _ { 1 } ( 1,2 ) = \psi ( 1,2 ) + \psi ( 2,1 ) = 1 s \alpha ( 1 ) 1 s \beta ( 2 ) + 1 s \alpha ( 2 ) 1 s \beta ( 1 ) } \\ 
{ \Psi _ { 2 } ( 1,2 ) = \psi ( 1,2 ) - \psi ( 2,1 ) = 1 s \alpha ( 1 ) 1 s \beta ( 2 ) - 1 s \alpha ( 2 ) 1 s \beta ( 1 ) } \right.
$$


