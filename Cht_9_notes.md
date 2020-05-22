# Chapter 9: The Chemical Bond: Diatomic Molecules                                                                                                                                  双原子分子的化学键

:scream:

[toc]

## 9.1 The Born-Oppenheimer Approximation Simplifies the Schrödinger Equation for Molecules                                                                                                                     波恩-奥本海默近似简化了薛定谔方程



上标a表示某个电子态
$$
H=\left(-\sum_{i=1}^{N} \frac{1}{2} \nabla_{i}^{2}-\sum_{i=1}^{N} \sum_{k=1}^{M} \frac{z_{A}}{r_{i d}}+\sum_{i=1}^{N} \sum_{j>i}^{N} \frac{1}{r_{i j}}\right)+\sum_{i=1}^{M} \sum_{B>d}^{M} \frac{Z_{A} Z_{B}}{R_{A B}}-\sum_{A=1}^{M} \frac{1}{2 M_{A}} \nabla_{A}^{2}
$$
波恩-奥本海默将电子与原子核的哈密顿分开处理



1 电子薛定谔方程为
$$
H _ { e } \Phi ^ { a } ( \{ x \} , \{ R \} ) = E _ { e l e } ^ { a } ( \{ R \} ) \Phi ^ { a } ( \{ x \} , \{ R \} )
$$

$$
H_e = - \sum _ { i = 1 } ^ { N } \frac { 1 } { 2 } \nabla _ { i } ^ { 2 } - \sum _ { i = 1 } ^ { N } \sum _ { A = 1 } ^ { M } \frac { Z _ { A } } { r _ { i A } } + \sum _ { i = 1 } ^ { N } \sum _ { j > i } ^ { N } \frac { 1 } { r _ { i j } }
$$

明确依赖电子坐标，参数化依赖于核的坐标（第二项）

 电子波函数参数化依赖于核坐标，认为核运动不影响电子



2 核薛定谔方程

核哈密顿：
$$
H _ { N } = - \sum _ { A = 1 } ^ { M } \frac { 1 } { 2 M _ { A } } \nabla _ { A } ^ { 2 } + U ^ { a } ( \{ R \} )
$$

$$
U ^ { a } ( \{ R \} ) = E _ { e l e } ^ { a } ( \{ R \} ) + \sum _ { A = 1 } ^ { M } \sum _ { B > A } ^ { M } \frac { z _ { A } Z _ { B } } { R _ { A B } }
$$

势能面

求解核运动方程得到什么信息？反应速率 分子异构化 核坐标变化 分子动力学讲核运动的动力学

BO失效：内转换 系间穿越 磷光 有两个态能量简并

## 9.2 H~2~^+^ Is the Prototypical Species of Molecular-Orbital Theory

分子轨道是原子轨道的线性组合



## 

$$
\begin{aligned}
H_{\mathrm{AA}}&=\left\langle 1 s_{\mathrm{A}}|\hat{H}| 1 s_{\mathrm{A}}\right\rangle \\
&=\int \mathrm{d} \mathbf{r} \operatorname{ls}_{A}^{*}\left(-\frac{1}{2} \nabla^{2}-\frac{1}{r_{A}}-\frac{1}{r_{B}}+\frac{1}{R}\right) 1 s_{A} \\
&=\int \mathrm{d} \mathbf{r} 1 s_{A}^{*}\left(-\frac{1}{2} \nabla^{2}-\frac{1}{r_{A}}\right) 1 s_{A}+\int d \mathbf{r} \operatorname{ls}_{A}^{*}\left(-\frac{1}{r_{B}}+\frac{1}{R}\right) 1 s_{A} \\
&=\int \mathrm{d} \mathbf{r} 1 s_{A}^{*} \mathrm{E}_{1 s} 1 s_{A}+J\\
&=\mathrm{E}_{1 s}+J
\end{aligned}
$$

动能项 吸引项 相互作用项 第三行到第四行：1s的哈密顿作用在1s的本征函数上得到E，波函数归一化

其中，库仑积分J被定义为：
$$
J = \int \mathrm{d} r \, 1 s _ { A } ^ { * } \left( - \frac { 1 } { r _ { B } } + \frac { 1 } { R } \right) 1 s _ { A } = - \int \frac { \mathrm{d} r \, 1 s _ { A } ^ { * } 1 s _ { A } } { r _ { B } } + \frac { 1 } { R } = e ^ { - 2 R } \left( 1 + \frac { 1 } { R } \right) \quad ( \geqslant 0 )
$$

$$
\begin{aligned}
H_{\mathrm{AB}} &=\left\langle 1 s_{\mathrm{A}}|\hat{H}| 1 s_{\mathrm{B}}\right\rangle \\
&=\int d \mathbf{r} 1 s_{A}^{*}\left(-\frac{1}{2} \nabla^{2}-\frac{1}{r_{A}}-\frac{1}{r_{B}}+\frac{1}{R}\right) 1 s_{B} \\
&=\int d \mathbf{r} 1 s_{A}^{*}\left(-\frac{1}{2} \nabla^{2}-\frac{1}{r_{B}}\right) 1 s_{B}+\int d \mathbf{r} 1 s_{A}^{*}\left(-\frac{1}{r_{A}}+\frac{1}{R}\right) 1 s_{B} \\
&=\int d \mathbf{r} 1 s_{A}^{*} E_{1 s} 1 s_{B}+\int d \mathbf{r} 1 s_{A}^{*}\left(-\frac{1}{r_{A}}+\frac{1}{R}\right) 1 s_{B}=E_{1 s} S+K
\end{aligned}
$$

把氢原子的电子拉到无穷远得到1s轨道能量

能量是成键反键的唯一判据 相对两个自由原子的能量升高

氢原子吸收光子跑到反键轨道上 两个核逐渐远离

$\psi_+$：成键分子轨道，表示稳定的化学键
$$

$$


$\psi_-$：反键分子轨道，表示两个核之间的排斥相互作用
$$
\Delta E_{-} =
$$

> In the above treatment, we used a linear combination of only two atomic orbitals to obtain two molecular orbitals. This was done solely for simplicity.
>
> We could also use a linear combination such as
> $$
> \psi = c _ { 1 } 1 s _ { A } + c _ { 2 } 1 s _ { B } + c _ { 3 } 2 s _ { A } + c _ { 4 } 2 s _ { B } + c _ { 5 } 2 p _ { z A } + c _ { 6 } 2 p _ { z B }
> $$



## 9.3 A Simple Molecular-Orbital Treatment of H~2~ Places Both Electrons in a Bonding Orbital

我们得到了成键轨道和反键轨道

多原子分子，把他的分子轨道用原子轨道的线性组合表示

求解HFR方程，根据对称性粗糙得到）多电子原子的波函数用slate行列式描述



氢分子取两个独立的氢原子轨道 zeta=1 不完全独立
$$
1 s = ( \zeta ^ { 3 } / \pi ) ^ { 1 / 2 } e ^ { - \zeta } \quad ( \zeta = 1
$$


figure 9.6 解读 

正确解释了氢原子形成化学键



sigma轨道关于原子核连线的轴对称



1sA轨道经过反演得到1sB 相加得到 相减得到负号

2pzA变成2pzB

2p对称面

反演操作2pxA变成-2pxB

2pxA+2pxB变成-2pxA-2pxB

The Overlap Integral Is a Quantitative Measure of the Overlap of Atomic Orbitals Situated on Different Atoms

2个3d轨道组合 dz2dz2头对头sigma 肩并肩pi 面对面 delta

## 9.4 Molecular Orbitals Can Be Ordered According to Their Energies                                                             分子轨道可以根据能量排序



能级顺序

## 9.5 Molecular-Orbital Theory Can Account for the Stability of Homonuclear Diatomic Molecules                                                                                        分子轨道理论可以解释同核双原子分子的稳定性

键级=1/2成键轨道电子数-反键轨道电子数

下标同核对称性 g对称 u是不对称

B2自旋多重度是3 键级为1
$$
K K ( \sigma _ { g } 2 s ) ^ { 2 } ( \sigma _ { u } 2 s ) ^ { 2 } ( \pi _ { u } 2 p _ { x } ) ^ { 1 } ( \pi _ { u } 2 p _ { y } ) ^ { 1 }
$$


> #### Example 9.2
>
> 氧分子S=1三重态基态 顺磁性paramagnetic

键级大键长短

## 9.6 Photoelectron Spectra Support the Existence of Molecular Orbitals                                                                                                                                            光电谱是分子轨道存在的证据

光电子能谱的峰 电离能是分子轨道能量的负值

## 9.7 Molecular-Orbital Theory Also Applies to Heteronuclear Diatomic Molecules                                                                                                                                       使用分子轨道理论预测异核双原子分子的成键

考虑氰根粒子 碳氮电负性接近 用C2组态类比 写出电子组态

反演对称性不成立，反键用*表示
$$
K K ( \sigma 2 s ) ^ { 2 } ( \sigma ^ { * } 2 s ) ^ { 2 } ( \pi 2 p _ { x } ) ^ { 2 } ( \pi 2 p _ { y } ) ^ { 2 } ( \sigma 2 p _ { z } ) ^ { 2 }
$$
HF分子中用2pz成键 2px不能有效重叠 1sH不与1s轨道重叠：成键有三要素 能量不匹配 F的1s轨道能量低
$$
\psi = c_1 1 S_H \pm c_2 2 p_{zF}
$$
F 非键轨道，不参与键级计算



## 9.8 An SCF-LCAO-MO Wave Function Is Determined Self-Consistently

采用许多原子轨道的线性组合得到更好的分子轨道
$$
\psi = c _ { 1 } 1 s _ { A } + c _ { 2 } 1 s _ { B } + c _ { 3 } 2 s _ { A } + c _ { 4 } 2 s _ { B } + c _ { 5 } 2 p _ { z A } + c _ { 6 } 2 p _ { z B } + \cdots
$$
HF方法可以预测键长但不能很好地预测键能

## 9.9 Electronic States of Molecules Are Designated by Molecular Term Symbols

$$
M_L=m_{l1}+m_{l2}+\cdots
$$

找到与哈密顿对易的量来表示状态

## 9.10 Molecular Term Symbols Designate the Symmetry Properties of Molecular Wave Functions

$$
\left|\psi_{1} \alpha \psi_{2} \beta\right|=\left\{\begin{array}{l}
g(g \times g, u \times u) \\
u(g \times u, u \times g)
\end{array}\right\}

$$

## 



## 9.11 Most Molecules Have Excited Electronic States



# Supplementary Material 补充材料

## Introduction to Valence Bond Theory 价键理论简介


$$
\Theta_k= \prod _ { i , j } \frac { 1 } { \sqrt { 2 } } [ \alpha ( i ) \beta ( j ) - \alpha ( j ) \beta ( i ) ] \prod _ { i } \alpha ( k )
$$
