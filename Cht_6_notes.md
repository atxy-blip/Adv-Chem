# Chapter 6: the Hydrogen Atom                                          第六章：氢原子模型

## 6.1 The Schrödinger Equation for the Hydrogen Atom                                                 氢原子薛定谔方程

氢原子的哈密顿算符为：
$$
\hat{H}=-\frac{\hbar^2}{2m_e}\nabla^2-\frac{e^2}{4\pi\varepsilon_0r}
$$
在球极坐标系中氢原子的薛定谔方程为：
$$
-\frac{\hbar^2}{2m_e}\left[\frac{1}{r^2}\frac{\partial}{\partial{r}}\left(r^2\frac{\partial{\psi}}{\partial{r}}\right)+\frac{1}{r^2\text{sin}\theta}\frac{\partial}{\partial{\theta}}\left(\text{sin}\theta\frac{\partial{\psi}}{\partial{\theta}}\right)+\frac{1}{r^2\text{sin}^2\theta}\frac{\partial^2{\psi}}{\partial{\phi^2}} \right]\\-\frac{e^2}{4\pi\varepsilon_0r}\psi\left(r,\theta,\phi\right)=E\psi\left(r,\theta,\phi\right)
$$
使用代换==$\psi\left(r,\theta,\phi\right)=R\left(r\right)Y\left(\theta,\phi\right)$==得
$$
-\frac{\hbar^2}{R\left(r\right)}\left[\frac{\mathrm{d}}{\mathrm{d}r}\left(r^2\frac{\mathrm{d}R}{\mathrm{d}r}\right)+\frac{2m_{e}r^{2}}{\hbar^2}\left(\frac{e^2}{4\pi\varepsilon_0r}+E\right)R\left(r\right)\right]
\\-\frac{\hbar^2}{Y\left(\theta,\phi\right)}\left[\frac{1}{\text{sin}\theta}\frac{\partial}{\partial{\theta}}\left(\text{sin}\theta\frac{\partial{Y}}{\partial{\theta}}\right)+\frac{1}{\text{sin}^2\theta}\frac{\partial^2{Y}}{\partial{\phi^2}}\right]=0
$$




## 6.2 The Wavefunctions of a Rigid Rotator Are Called Spherical Harmonics                                                                                                                                               刚性转子的波函数

### Legendre's Equation                                                                                                                                               勒让德方程

$$
( 1 - \omega ^ { 2 } ) \frac { \mathrm{d} ^ { 2 } P } {\mathrm{d}  \omega ^ { 2 } } - 2 \omega \frac { \mathrm{d} P } {\mathrm{d} \omega } + \left[ \beta - \frac { m ^ { 2 } } { 1 - \omega ^ { 2 } } \right] P ( \omega ) = 0 \quad m = 0 , \pm 1 , \pm 2
$$



### Spherical Harmonic Functions                                                                                                          球谐函数

$$
\Theta_ { l,m } ( \theta ) = \left[ \frac { 2 l + 1 } { 2 } \frac { ( l - | m | ) ! } { ( l + | m | ) ! } \right] ^ { 1 / 2 } p _ { l } ^ { | m | } ( \cos \theta )
$$

$$
Y _ { l } ^ { m } ( \theta , \phi ) = \Phi ( \phi ) \Theta _ { l , m } ( \theta ) = \frac { 1 } { \sqrt { 2 \pi } } e ^ { i m \phi } \Theta _ { l , m } ( \theta )
$$

$$
Y _ { l } ^ { m } ( \theta , \phi ) = \left[ \frac { ( 2 l + 1 ) } { 4 \pi } \frac { ( l - m | ) ! } { ( l + | m | ! ! } \right] p _ { l } ^ { | m | } ( \cos \theta ) e ^ { i m \phi }
$$

$$
\int _ { 0 } ^ { \pi } \mathrm{d} \theta \sin \theta \int _ { 0 } ^ { 2 \pi } \mathrm{d} \phi Y _ { 1 } ^ { m } ( \theta , \phi ) ^ { * } Y _ { n } ^ { k } ( \theta , \phi ) = \delta _ { ln } \delta _ { m k }
$$



### Spherical Harmonic Functions Are the Eigenfunctions of the Square of the Angular Momentum                                                                                                                                     球谐函数是角动量平方的特征值函数

## 6.3 Orbital Angular Momentum of a One-Particle System                                                                                                          单粒子轨道角动量算符

$$
\vec{L}=\vec{r}\times\vec{p}
$$

z方向的本征值
$$
L_z=m\hbar, \quad m=-l,...,0,1,...,l
$$
xy方向和z方向没有区别

### Relations between angular momentum operators                                                                                                          角动量算符之间的关系

笛卡尔坐标系中有
$$
\hat{L}_x = - i \hbar \left( y\frac{\partial}{\partial{z}}-z\frac{\partial}{\partial{y}} \right),\quad
\hat{L}_y = - i \hbar \left( z\frac{\partial}{\partial{x}}-x\frac{\partial}{\partial{z}} \right),\quad
\hat{L}_z = - i \hbar \left( x\frac{\partial}{\partial{y}}-y\frac{\partial}{\partial{x}} \right)
$$

$$
\hat{L}^2=\hat{L}_x^2+\hat{L}_y^2+\hat{L}_z^2
$$

> #### 从笛卡尔坐标系到球坐标系的变量代换
>
> $$
> \begin{cases}
> x=r\sin\theta\cos\phi \\
> y=r\sin\theta\sin\phi \\
> z=r\cos\theta 
> \end{cases}
> \quad\Rightarrow\quad
> \begin{cases}
> r=\sqrt{x^2+y^2+z^2} \\
> \theta=\arccos\frac{z}{\sqrt{x^2+y^2+z^2}} \\
> \phi=\arctan\frac{y}{x}
> \end{cases}
> $$
>
> 注意$\theta,\phi$的定义，$\theta\in\left[0,\pi\right],\phi\in[0,2\pi]$

球坐标系中

$$
\hat{L}_z = -i\hbar\frac{\partial}{\partial{\phi}}
$$

$$
\left [ \hat{L}_y, \hat{L}_z \right ] = i \hbar \hat{L}_x;\quad
\left [ \hat{L}_z, \hat{L}_x \right ] = i \hbar \hat{L}_y;\quad
\left [ \hat{L}_x, \hat{L}_y \right ] = i \hbar \hat{L}_z \\ 
\left [ \hat{L}^2, \hat{L}_x \right ]=\left [ \hat{L}^2, \hat{L}_y \right ]=\left [ \hat{L}^2, \hat{L}_z \right ]=0
$$

> #### 交换子的运算关系
>
> $$
> \left[{\hat  {A}},{\hat  {B}}\right]=-\left[{\hat  {B}},{\hat  {A}}\right] \\ 
> \left[{\hat {A}},{\hat {B}}+{\hat {C}}\right]=\left[{\hat {A}},{\hat {B}}\right]+\left[{\hat {A}},{\hat {C}}\right],\quad \left[{\hat {A}}+{\hat {B}},{\hat {C}}\right]=\left[{\hat {A}},{\hat {C}}\right]+\left[{\hat {B}},{\hat {C}}\right] \\ 
> \left[{\hat {A}},{\hat {B}}{\hat {C}}\right]=\left[{\hat {A}},{\hat {B}}\right]{\hat {C}}+{\hat {B}}\left[{\hat {A}},{\hat {C}}\right],\quad \left[{\hat {A}}{\hat {B}},{\hat {C}}\right]=\left[{\hat {A}},{\hat {C}}\right]{\hat {B}}+{\hat {A}}\left[{\hat {B}},{\hat {C}}\right] \\ 
> \left[{\hat  {A}},{\hat  {A}}^{n}\right]=0,\quad n=1,2,3\cdots \\ 
> \left[k{\hat  {A}},{\hat  {B}}\right]=\left[{\hat  {A}},k{\hat  {B}}\right]=k\left[{\hat  {A}},{\hat  {B}}\right] \\ 
> \left[{\hat  {A}},\left[{\hat  {B}},{\hat  {C}}\right]\right]+\left[{\hat  {C}},\left[{\hat  {A}},{\hat  {B}}\right]\right]+\left[{\hat  {B}},\left[{\hat  {C}},{\hat  {A}}\right]\right]=0
> $$
>



球极坐标中三个分量的表达形式 $\hbar = \frac{h}{2\pi}$

$Y_l^m\left ( \theta,\phi \right )$是角动量平方的本征值函数

角动量长度量子化
$$
\left |\vec{L} \right | = \hbar \sqrt{l \left(l+1 \right)}
$$
上式的值大于l

m=-l到l l=1三个值

$Y_{1}^{-1}\left ( \theta,\phi \right )$不是$\hat{L}_x$的本征值函数

6个对易关系式 角动量平方值 大小 在某个方向分量值，另外两个方向不知道

Fig. 6.4 确定到锥面

6.1讨论题 对 使用约化质量
$$
\hat{H}=-\frac{\hbar^{2}}{2\mu_{e}}\nabla^2+\frac{1}{4\pi\epsilon_0r}
$$





角动量平方的本征值函数是球谐函数

球谐函数不是$\hat{L}_x$的本征值函数，应该是$Y_l^m\left ( \theta,\phi \right )$不同m取值线性组合

## 6.4 Hydrogen Atomic Orbitals Depend upon Three Quantum Numbers

$$
-\frac{\hbar^{2}}{2 m_{e} r^{2}} \frac{d}{d r}\left(r^{2} \frac{d R}{d r}\right)+\left[\frac{\hbar^{2} l(l+1)}{2 m_{e} r^{2}}-\frac{e^{2}}{4 \pi \varepsilon_{0} r}-E\right] R(r)=0
$$

解本征值方程得到能量公式：
$$
E_{n}=-\frac{m_{e} e^{4}}{8 \varepsilon_{0}^{2} h^{2} n^{2}}=-\frac{Ze^{2}}{8 \pi \varepsilon_{0} a_{0} n^{2}} \quad n=1,2, \cdots
$$
玻尔半径为：
$$
a_{0}=\frac{\varepsilon_{0} h^{2}}{\pi m_{e} e^{2}}
$$


Laguerre polynomials

 



### Radial wave functions   

$$
R_{n l}=-\left\{\frac{(n-l-1) !}{2 n[(n+l) !]^{3}}\right\}^{1 / 2}\left(\frac{2}{n a_{0}}\right)^{l+3 / 2} r^{l} e^{-r / n a_{0}} L_{n+1}^{2 l+1}\left(\frac{2 r}{n a_{0}}\right) \quad 
\begin{cases}
n=1,2, \cdots \\
l=0,1, \cdots, n-1
\end{cases}
$$

### Hydrogen atomic wave functions                                                                                                                     氢原子波函数

$$
\Psi(r,\theta,\phi)=R_{nl}(r)Y_{l}^{m}(\theta,\phi)
$$
三个量子数 每个的物理意义
$$
\begin{aligned}
 n&=1,2,3, \cdots && \text{principal}\\
 l&=0,1,2, \cdots, n-1&& \text{angular momentum}\\
 m&=-l,-l+1, \cdots, l-1, l && \text{magnetic}
\end{aligned}
$$
哈密顿 角动量平方 角动量z分量 三个两两对易，可以同时准确测得能量、角动量和角动量z分量
$$
\left[\hat{H}, \hat{L}^{2}\right]=0; \quad
\left[\hat{L}^{2}, \hat{L}_{z}\right]=0; \quad
\left[\hat{H}, \hat{L}_{z}\right]=0
$$
波函数是==正交归一*(orthonormal)*==的：
$$
\int_{0}^{\infty} \mathrm{d} r r^{2}\int_{0}^{\pi} \mathrm{d} \theta \sin \theta \int_{0}^{2 \pi} \mathrm{d} \phi \psi_{n^{\prime}l^{\prime}m^{\prime}}^{*}(r, \theta, \phi) \psi_{n lm }(r, \theta, \phi)=\delta_{n n^{\prime}} \delta_{l l^{\prime}} \delta_{m m^{\prime}}
$$

> #### Kronecker delta
>
> $$
> \delta _{ij}= {\begin{cases} 1 &(i=j)\\ 0 &(i\neq j) \end{cases}}
> $$

${n = n^{\prime}},\ {l =l^{\prime}},\ {m= m^{\prime}}$归一，否则正交
$$
\sigma=\frac{Zr }{a_{0}} \quad a_{0}=\frac{\varepsilon_{0} h^{2}}{\pi m_{e} e^{2}}
$$

$$
\begin{aligned}
n&=1 &\quad l&=0 &m&=0 &  \psi_{100}&=\frac{1}{\sqrt{\pi}}\left(\frac{Z}{ a_{0}}\right)^{\frac{3}{2}} e^{-\sigma} \\
n&=2&\quad l&=0 &m&=0 &\psi_{200}&=\frac{1}{4 \sqrt{2\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} (2-\sigma) e^{-\frac{\sigma }{2}} \\
&& l&=1 &m&=0 & \psi_{210}&=\frac{1}{4\sqrt{2\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} \sigma e^{-\frac{\sigma }{2}} \cos \theta \\
&&&&m&=\pm1 & \psi_{21\pm1}&=\frac{1}{8\sqrt{\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} \sigma e^{-\frac{\sigma}{2}}\sin \theta e^{\pm i \phi} \\
n&=3&\quad l&=0 &m&=0 &\psi_{300}&=\frac{1}{81 \sqrt{3\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}}(27-18\sigma+2\sigma^2) e^{-\frac{\sigma}{3}} \\
&& l&=1 &m&=0 & \psi_{310}&=\frac{\sqrt{2}}{81\sqrt{\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} (6-\sigma)\sigma e^{-\frac{\sigma}{3} } \cos \theta \\
&&&&m&=\pm1 & \psi_{31\pm1}&=\frac{1}{81 \sqrt{\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} (6-\sigma)\sigma e^{-\frac{\sigma}{3}} \sin \theta e^{\pm i \phi}\\
&& l&=2 &m&=0 & \psi_{320}&=\frac{1}{81\sqrt{6\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} \sigma^2 e^{-\frac{\sigma}{3}} (3\cos^2 \theta -1) \\
&&&&m&=\pm1 & \psi_{3d1\pm1}&=\frac{\sqrt{2}}{81\sqrt{\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} \sigma^2 e^{-\frac{\sigma}{3}} \sin \theta \cos \theta e^{\pm i \phi}\\
&&&&m&=\pm2 & \psi_{32\pm2}&=\frac{1}{162 \sqrt{\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} \sigma^2 e^{-\frac{\sigma }{3}} \sin^2 \theta e^{\pm2 i \phi}
\end{aligned}
$$

波函数可以代表氢原子和类氢离子

氢原子简并度$g_j=\sum_{l=1}^{n-1}(2l+1)=n^2$

2 1 1 2 1 -1 复函数波函数

$\sum_{m=-2}^{2}\psi_{32m}^2=\text{constant}$，3d轨道的总概率密度球对称

> 3d0的角动量z分量是0

## 6.5 s Orbitals Are Spherically Symmetric                                                                                                 s轨道呈球对称

氢原子和类氢离子的波函数被称为轨道*(orbital)*

### Radial distribution function

$$
p(r) =\left[R_{n l}(r)\right]^{2} r^{2} \int_{0}^{2 \pi} \int_{0}^{\pi}\left|Y_{l}^{m}(\theta, \phi)\right|^{2} \sin \theta \mathrm{d} \theta \mathrm{d} \phi 
\xlongequal {\text{normalize}}\left[R_{n l}(r)\right]^{2} r^{2}
$$

$p(r) =\left[R_{n l}(r)\right]^{2} r^{2}$被称为径向分布函数
$$
\int_{0}^{\infty} p(r) \mathrm{d} r=\int_{0}^{\infty} R_{n l}^{2}(r) r^{2} \mathrm{d} r=1
$$


> #### Example 6.4
>
> $$
> R_{10}(r)=\frac{2}{a_{0}^{3 / 2}} e^{-r / a_{0}}
> $$
>
> $$
> P=\int_{0}^{a_{0}} R_{10}^{2}(r) r^{2} \mathrm{d} r=\frac{4}{a_{0}^3} \int_{0}^{a_{0}} e^{-2 r / a_{0}} r^{2} \mathrm{d} r \\ \xlongequal {x=2 r / a_{0}}\frac{1}{2} \int_{0}^{2} e^{-2 x} x^{2} \mathrm{d} x = -\frac{1}{2}\left|_{0}^{2} (x^2+2x+2)e^{-x} \right|= 0.323
> $$
>
> 电子只有32.3%的概率出现在玻尔半径内

原子半径的定义？众说纷纭

### Number of nodes in the radial distribution function of different orbitals

径向部分的节面$(n-l-1)$ 一个电子不能出现的球面

> #### Example 6.5
>
> $$
> \langle r \rangle=\int_{0}^{\infty} \mathrm{d} r \int_{0}^{\pi} \mathrm{d}  \theta \int_{0}^{2 \pi} \mathrm{d}  \phi \psi_{nlm}^{*} r\psi_{nlm }r^{2}\sin \theta=4\pi\int_{0}^{\infty} \psi_{nlm}^{*} r^{3}\psi_{nlm}\mathrm{d} r
> $$
>
> 最可几概率出现在玻尔半径上，在玻尔半径这个球面上电子出现概率最大
>
> 平均距离为1.5个玻尔半径

## 6.6 There Are Three P Orbitals for Each Value of the Principal Quantum Number, n>=2


$$
\begin{aligned}
l&=0 &\quad m&=0 &\psi_{200}&=\psi_{2 s} &  \psi_{2 s}&=\frac{1}{\sqrt{\pi}}\left(\frac{Z}{2 a_{0}}\right)^{\frac{3}{2}}\left(1-\frac{Z r}{2 a_{0}}\right) e^{\frac{-Zr }{ 2 a_{0}}} \\
l&=1&\quad m&=1 & \psi_{211}&=\psi_{2 p_{+1}} &\psi_{2 p_{+1}}&=\frac{1}{8 \sqrt{\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{5}{2}} r e^{\frac{-Zr }{ 2 a_{0}}} \sin \theta e^{i \phi} \\
&& m&=0 &\psi_{210}&=\psi_{2 p_{0}} & \psi_{2 p_{0}}&=\frac{1}{\sqrt{\pi}}\left(\frac{Z}{2 a_{0}}\right)^{\frac{5}{2}} r e^{\frac{-Zr }{ 2 a_{0}}} \cos \theta \\
&& m& =-1 &\psi_{21-1}&=\psi_{2 p_{-1}}& \psi_{2 p_{-1}}&=\frac{1}{8 \sqrt{\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{5}{2}} r e^{\frac{-Zr}{ 2 a_{0}}} \sin \theta e^{-i \phi}
\end{aligned}
$$

### Real hydrogen atomic wave functions                                                                                                           实氢原子波函数

重新组合
$$
\begin{aligned} 
\psi_{2 p_{x}} &=\frac{1}{\sqrt{2}}\left(\psi_{2 p_{-1}}+\psi_{2 p_{1}}\right) \\
&=\frac{1}{4 \sqrt{2 \pi}}\left(\frac{Z}{a_{0}}\right)^{5 / 2} r e^{-Z r / 2 a_{0}} \sin \theta \cos \phi \\ 
&=\frac{1}{4 \sqrt{2 \pi}}\left(\frac{Z}{a_{0}}\right)^{5 / 2} x e^{-2 r / 2 a_{0}}
\\ 
\psi_{2 p_{y}} &=\frac{1}{\sqrt{2} i}\left(\psi_{2 p_{1}}-\psi_{2 p_{-1}}\right)=\frac{1}{4 \sqrt{2 \pi}}\left(\frac{Z}{a_{0}}\right)^{5 / 2}
{y e^{-2 r / 2 a_{0}}} \\
\psi_{2 p_{z}} &=\psi_{2 p_{0}}=\frac{1}{\sqrt{\pi}}\left(\frac{Z}{2 a_{0}}\right)^{5 / 2} z e^{-2 \pi / 2 a_{0}} 
\end{aligned}
$$

$\hat{L}_{z} \psi_{2 p_{x}} \neq k \psi_{2 p_{x}}$重新组合后不是lz的本征函数 还是l2的本征函数，长度确定
$$
C=\frac{\sqrt{2}}{81 \sqrt{\pi}}\left(\frac{Z}{a_{0}}\right)^{7 / 2} e^{-Zr / 3 a_{0}}  \\
\begin{aligned}
\psi_{3 d_{xy}}&=\left(\frac{1}{\sqrt{2} i}\right)\left(\psi_{3 d_{2}}-\psi_{3 d_{-2}}\right)&=&C(xy) \\
\psi_{3 d_{x^{2}-y^{2}}}&=\left(\frac{1}{\sqrt{2}}\right)\left(\psi_{3 d_{2}}+\psi_{3 d_{-2}}\right) &=&C\left(x^{2}-y^{2}\right)\\
\psi_{3 d_{z^2}}&=\psi_{3 d_{0}} &=&C\left(3 z^{2}-1\right)\\
\psi_{3 d_{xz}}&=\left(\frac{1}{\sqrt{2}}\right)\left(\psi_{3 d_{1}}+\psi_{3 d_{-1}}\right) &=&C(x z)\\
\psi_{3 d_{y_{z}}}&=\left(\frac{1}{\sqrt{2} i}\right)\left(\psi_{3 d_{1}}-\psi_{3 d_{-1}}\right) &=&C(y z)
\end{aligned}
$$

$3d_{z^2}$的lz=0，$3d_{xy}$测量lz得到\pm 2\hbar 概率系数的平方50% 平均值0 3dxy测量lz得到$\pm \hbar$
$$
\begin{aligned}
n&=1 &\quad l&=0&  \psi_{1s}&=\frac{1}{\sqrt{\pi}}\left(\frac{Z}{ a_{0}}\right)^{\frac{3}{2}} e^{-\sigma} \\
n&=2&\quad l&=0&\psi_{2s}&=\frac{1}{4 \sqrt{2\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} (2-\sigma) e^{-\frac{\sigma }{2}} \\
&& l&=1& \psi_{2 p_{z}}&=\frac{1}{4\sqrt{2\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} \sigma e^{-\frac{\sigma }{2}} \cos \theta \\
&&&& \psi_{2 p_{x}}&=\frac{1}{4\sqrt{2\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} \sigma e^{-\frac{\sigma }{2}} \sin \theta \cos \phi \\
&&&& \psi_{2 p_{y}}&=\frac{1}{4 \sqrt{2\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} \sigma e^{-\frac{\sigma }{2}} \sin \theta \sin \phi \\
n&=3&\quad l&=0&\psi_{3s}&=\frac{1}{81 \sqrt{3\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}}(27-18\sigma+2\sigma^2) e^{-\frac{\sigma}{3}} \\
&& l&=1& \psi_{3 p_{z}}&=\frac{\sqrt{2}}{81\sqrt{\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{5}{2}} (6-\sigma)\sigma e^{-\frac{\sigma}{3} } \cos \theta \\
&&&& \psi_{3 p_{x}}&=\frac{\sqrt{2}}{81 \sqrt{\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} (6-\sigma)\sigma e^{-\frac{\sigma}{3}} \sin \theta \cos \phi\\
&&&& \psi_{3 p_{y}}&=\frac{\sqrt{2}}{81 \sqrt{\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} (6-\sigma)\sigma e^{-\frac{\sigma}{3}} \sin \theta \sin \phi\\
&& l&=2& \psi_{3d_{z^2}}&=\frac{1}{81\sqrt{6\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} \sigma^2 e^{-\frac{\sigma}{3}} (3\cos^2 \theta -1) \\
&&&& \psi_{3d_{xz}}&=\frac{\sqrt{2}}{81\sqrt{\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} \sigma^2 e^{-\frac{\sigma }{3}} \sin \theta \cos \theta \cos \phi\\
&&&& \psi_{3d_{yz}}&=\frac{\sqrt{2}}{81\sqrt{\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} \sigma^2 e^{-\frac{\sigma }{3}} \sin \theta \cos \theta \sin \phi\\
&&&& \psi_{3d_{x^2-y^2}}&=\frac{1}{81 \sqrt{2\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} \sigma^2 e^{-\frac{\sigma }{3}} \sin^2 \theta \cos2\phi\\ 
&&&& \psi_{3d_{xy}}&=\frac{1}{81 \sqrt{2\pi}}\left(\frac{Z}{a_{0}}\right)^{\frac{3}{2}} \sigma^2 e^{-\frac{\sigma }{3}} \sin^2 \theta \sin2\phi
\end{aligned}
$$


### Nodal surfaces of real hydrogen atomic wave functions

\psi部分变化
$$
\tilde{\psi}_{n l m}=R_{n l}(r) S_{l m}(\theta) f(\phi)
$$

节面个数$|m |$

\theta常数 夹角为90°是平面 其余是锥面

径向部分$R_{n l}(r)$ 球面

### Angular parts of a few real hydrogen orbitals

$$
\begin{aligned}l&=0 & s&=\frac{1}{\sqrt{4 \pi}} \\
l&=1 & p_{x}&=\sqrt{\frac{3}{4 \pi}} \sin \theta \cos \phi \\ 
&& p_{y}&=\sqrt{\frac{3}{4 \pi}} \sin \theta \sin \phi \\
&& p_{z}&=\sqrt{\frac{3}{4 \pi}} \cos \theta \\
l&=2 &d_{x^{2}-y^{2}} &=\frac{1}{4} \sqrt{\frac{15}{\pi}} \sin ^{2} \theta \cos (2 \phi) \\ 
&& d_{z^{2}} &=\frac{1}{4} \sqrt{\frac{5}{\pi}}\left(3 \cos ^{2} \theta-1\right) \\
&& d_{x y} &=\frac{1}{4} \sqrt{\frac{15}{\pi}} \sin ^{2} \theta \sin 2 \phi \\ 
&& d_{x z} &=\frac{1}{4} \sqrt{\frac{15}{\pi}} \sin 2 \theta \cos \phi \\ 
&& d_{y z} &=\frac{1}{4} \sqrt{\frac{15}{\pi}} \sin 2 \theta \sin \phi \end{aligned}
$$

电子云密度图

轮廓图



## 6.7 The Zeeman Effect

1896

外加磁场会导致谱线分裂

电子做轨道运动，产生磁矩
$$
\vec{m}_{L}=-\frac{e}{2 m_{e}} \vec{L}
$$

相互作用势 标量
$$
V=-\vec{m}_{L} \cdot \vec{B}=\frac{e}{2 m_{e}} \vec{L} \cdot \vec{B}
$$

$$
V = \frac { e } { 2 m _ { e } } B ( L _ { x } \vec { i } + L _ { y } \vec { j } + L _ { z } \vec { k } ) \cdot \vec { k } = \frac { e } { 2 m _ { e } } B L _ { z } = \beta _ { e } \hbar ^ { - 1 } B L
$$



玻尔磁子

外加磁场后哈密顿发生变化
$$
\hat{H}_B=\beta_e\hat{L} _ { z }\hbar ^ { - 1 } B
$$

$$
E = - \frac { Ze ^ { 2 } } { 8 \pi \varepsilon _ { 0 } a _ { 0 } n ^ { 2 } } + \beta _ { e } B m
$$
总哈密顿和主量子数n和磁量子数m有关，m=0能级相等

原本d轨道五重简并，加上磁场后产生五个能级

## 6.8 The Schrödinger Equation for the Helium Atom Can Be Solved Exactly

两个电子以上的体系，几个电子的体系，可以得到相对精确的答案
$$
\begin{aligned}
&\left(-\frac{\hbar^{2}}{2 M} \nabla^{2}-\frac{\hbar^{2}}{2 m_{e}} \nabla_{1}^{2}-\frac{\hbar^{2}}{2 m_{e}} \nabla_{2}^{2}\right) \psi\left(\vec{R}, \vec{r}_{1}, \vec{r}_{2}\right)+\\
&\left(-\frac{2 e^{2}}{4 \pi \varepsilon_{0}\left|\vec{R}-\vec{r}_{1}\right|}-\frac{2 e^{2}}{4 \pi \varepsilon_{0}\left|\vec{R}-\vec{r}_{2}\right|}+\frac{e^{2}}{4 \pi \varepsilon_{0}\left|\vec{r}_{1}-\vec{r}_{2}\right|}\right) \psi\left(\vec{R}, \vec{r}_{1}, \vec{r}_{2}\right)\\
&=E \psi\left(\vec{R}, \vec{r}_{1}, \vec{r}_{2}\right)
\end{aligned}
$$

orz

$$
\begin{aligned}
&-\frac{\hbar^{2}}{2 m_{e}}\left(\nabla_{1}^{2}+\nabla_{2}^{2}\right) \psi\left(\vec{r}_{1}, \vec{r}_{2}\right)-\frac{2 e^{2}}{4 \pi \varepsilon_{0}}\left(\frac{1}{r_{1}}+\frac{1}{r_{2}}\right) \psi\left(\vec{r}_{1}, \vec{r}_{2}\right) \\
&+\frac{e^{2}}{4 \pi \varepsilon_{0}\left|\mathbf{r}_{1}-\mathbf{r}_{2}\right|} \psi\left(\vec{r}_{1}, \vec{r}_{2}\right)=E \psi\left(\vec{r}_{1}, \vec{r}_{2}\right)
\end{aligned}
$$

第三项涉及两个电子之间的相互作用 真难

Hiroshi Nakatsuji

## Supplementary material                                                                                                                   补充材料

### The ladder operator method for angular momentum                                                                      用梯形算符求解角动量

使用代数而非解析的方法

兼顾轨道角动量和自旋角动量
$$
\hat{M}_{z}Y=bY \quad \hat{M}^{2}Y=CY
$$

#### 1

假定自旋角动量的对易关系如下
$$
\left[\hat{M}_{x}, \hat{M}_{y}\right]=i\hbar\hat{M}_{z}; \quad
\left[\hat{M}_{y}, \hat{M}_{z}\right]=i\hbar\hat{M}_{x}; \quad
\left[\hat{M}_{z}, \hat{M}_{x}\right]=i\hbar\hat{M}_{y}; \quad \\
\left[\hat{M}_{x}, \hat{M}_{x}\right]=
\left[\hat{M}_{y}, \hat{M}_{y}\right]=
\left[\hat{M}_{z}, \hat{M}_{z}\right]=0
$$

波函数不知道，记为Y

#### 2

梯形算符：上升算符$\hat{M}_{+}=\hat{M}_{x}+i \hat{M}_{y}$，下降算符$\hat{M}_{-}=\hat{M}_{x}-i \hat{M}_{y}$
$$
\hat{M}_{x} \hat{M}_{y}= \\
\hat{M}_{y} \hat{M}_{x}=
$$

#### 3

$$
\hat{M}_{+} \hat{M}_{z}Y=\hat{M}_{+}bY
$$

上升算符是Y的 使本征值增加$\pm k\hbar$

#### 4

$$
\hat{M}^{2}\left( \hat{M}_{\pm}^{k}Y\right)=C\left( \hat{M}_{\pm}^{k}Y\right)
$$
#### 5

本征值有界

厄密性质
$$
\langle{A}^{2}\rangle=\int\psi^{*}\hat{A}\left(\hat{A}\psi\right)\mathrm{d}\tau=\int\left(\hat{A}\psi\right)\left(\hat{A}\psi\right)^{*}\mathrm{d}\tau=\int\left|\hat{A}\psi\right|^2\mathrm{d}\tau \geq 0
$$


> #### Hermitian 本征值为实数
>
> $$
> \int\psi^{*}\hat{A}\psi\mathrm{d}\tau=a \\
> \int\psi\hat{A}^{*}\psi^{*}\mathrm{d}\tau=a^{*} \\
> \int\psi^{*}\hat{A}\psi\mathrm{d}\tau=\int\psi\hat{A}^{*}\psi^{*}\mathrm{d}\tau
> $$



$$
\langle Y_{k} |\hat{M}_{x}^{2 }|Y_{k} \rangle\geq 0
$$

$$
C=b_{max}^2+\hbar b_{max}
$$

$$
\hat{M}_{-}Y_{min}=0
$$

$$
b_{max}=-b_{min}\quad b_{max}=b_{min}-\hbar
$$


$$
b=-j\hbar,(-j+1)\hbar,\cdots,(j-1)\hbar,j\hbar
$$

#### 6 $\hat{M}^{2},\hat{M}_{z}$的本征值

$$
\hat{M}^{2}Y=j(j+1)\hbar^{2}Y \ j=0,\frac{1}{2},1,\frac{3}{2},\cdots \\
\hat{M}_{z}Y=m_{j}\hbar Y
$$

自旋角动量可以是半整数

#### 7

$d_{+}=\hbar\sqrt{(j+m)(j-m+1)}$
$$
\hat{M}_{-}|j,m \rangle=\hbar\sqrt{(j+m)(j-m+1)}|j,m-1 \rangle
$$

$$
Y=|jm \rangle
$$

### Determinants                                                                                                                                                       行列式

#### 1 Determinants and cofactors                                                                                                                          行列式和代数余子式

$$
A=\det(A)=\begin{vmatrix}
{ a _ { 11 } } & \cdots & { a _ { 1N } } \\ 
\vdots & \ddots & \vdots \\ 
{ a _ { N1 } } & \cdots & { a _ { NN } }
\end{vmatrix}=\sum_{i=1}^{N!}(-1)^{p_i}\hat{p}_{i} {a _ { 11 } }{ a _ { 12 } }\cdots{ a _ { NN } }
$$


$$
\begin{vmatrix}
x_{11} & x_{12}  & \cdots   & x_{1m}   \\
x_{21} & x_{22}  & \cdots   & x_{2m}  \\
\vdots & \vdots  & \ddots   & \vdots  \\
x_{n1} & x_{n2}  & \cdots\  & x_{nm}  \\
\end{vmatrix}
$$

$$
D = \begin{vmatrix}
{ a _ { 11 } } & { a _ { 12 } } & { a _ { 13 } } \\ 
{ a _ { 21 } } & { a _ { 22 } } & { a _ { 23 } } \\ 
{ a _ { 31 } } & { a _ { 32 } } & { a _ { 33 } }
\end{vmatrix}
$$

#### 2 Properties of determinants

#### 3 Cramer's rule

$$
\begin{cases}
{ a _ { 11 } } x+ { a _ { 12 } }y =  d _ { 1 } \\ 
{ a _ { 21 } } x+ { a _ { 22 } }y =  d _ { 2 }
\end{cases}
$$

$$
D = \begin{vmatrix}
{ a _ { 11 } } & { a _ { 12 } } \\ 
{ a _ { 21 } } & { a _ { 22 } } 
\end{vmatrix} \quad 
x=\frac{\begin{vmatrix}
{ d _ { 1 } } & { a _ { 12 } } \\ 
{ d _ { 2 } } & { a _ { 22 } } 
\end{vmatrix}}{\begin{vmatrix}
{ a _ { 11 } } & { a _ { 12 } } \\ 
{ a _ { 21 } } & { a _ { 22 } }
\end{vmatrix}} \quad 
y=\frac{\begin{vmatrix}
{ a _ { 11 } } & { d _ { 1 } }  \\ 
{ a _ { 21 } } & { d _ { 2 } } 
\end{vmatrix}}{\begin{vmatrix}
{ a _ { 11 } } & { a _ { 12 } } \\ 
{ a _ { 21 } } & { a _ { 22 } }
\end{vmatrix}}
$$

###  3d angular part by matplotlib

<div align=center><img src=".\figures\3d Angular Part 181850195.png" alt="3d Angular Part" style="zoom:72%;"/>


```python
#================
#  Yu XIONG, 2020
#================

import matplotlib.pyplot as plt
from matplotlib import cm
import numpy as np
from mpl_toolkits.mplot3d import Axes3D  # noqa: F401 unused import

theta, phi = np.linspace(0, np.pi, 1000), np.linspace(0, 2 * np.pi, 1000)
THETA, PHI = np.meshgrid(theta, phi)

C = np.sqrt(15 / np.pi) / 4

# set up a 3x2 figure 
fig = plt.figure(figsize=plt.figaspect(0.66))

#===============
#  First subplot
#===============
# set up the axes
ax = fig.add_subplot(2, 3, 1, projection='3d')

# d_z^2
R = C * (3 * np.cos(THETA)**2 - 1)

X = R * np.sin(THETA) * np.cos(PHI)
Y = R * np.sin(THETA) * np.sin(PHI)
Z = R * np.cos(THETA)

plt.title(r"$3d_{z^2}$")
plot = ax.plot_surface(X, Y, Z,
    linewidth=0, antialiased=True, alpha=0.6)

#===============
# Second subplot
#===============
# set up the axes
ax = fig.add_subplot(2, 3, 2, projection='3d')

# d_zx
R = C * np.cos(PHI) * np.sin(THETA * 2)

X = R * np.sin(THETA) * np.cos(PHI)
Y = R * np.sin(THETA) * np.sin(PHI)
Z = R * np.cos(THETA)

plt.title(r"$3d_{xz}$")
plot = ax.plot_surface(X, Y, Z,
    linewidth=0, antialiased=True, alpha=0.6)

#===============
#  Third subplot
#===============
# set up the axes
ax = fig.add_subplot(2, 3, 3, projection='3d')

# d_yz
R = C * np.sin(PHI) * np.sin(THETA * 2)

X = R * np.sin(THETA) * np.cos(PHI)
Y = R * np.sin(THETA) * np.sin(PHI)
Z = R * np.cos(THETA)

plt.title(r"$3d_{yz}$")
plot = ax.plot_surface(X, Y, Z,
    linewidth=0, antialiased=True, alpha=0.6)

#===============
# Fourth subplot
#===============
# set up the axes
ax = fig.add_subplot(2, 3, 4, projection='3d')

# d_x^2-y^2
R = C * np.cos(2 * PHI) * (np.sin(THETA)**2)

X = R * np.sin(THETA) * np.cos(PHI)
Y = R * np.sin(THETA) * np.sin(PHI)
Z = R * np.cos(THETA)

plt.title(r"$3d_{x^2-y^2}$")
plot = ax.plot_surface(X, Y, Z,
    linewidth=0, antialiased=True, alpha=0.6)

#===============
#  Fifth subplot
#===============
# set up the axes
ax = fig.add_subplot(2, 3, 5, projection='3d')

# d_xy
R = C * np.sin(2 * PHI) * (np.sin(THETA)**2)

X = R * np.sin(THETA) * np.cos(PHI)
Y = R * np.sin(THETA) * np.sin(PHI)
Z = R * np.cos(THETA)

plt.title(r"$3d_{xy}$")
plot = ax.plot_surface(X, Y, Z,
    linewidth=0, antialiased=True, alpha=0.6)

plt.show()
```

>### MATLAB
>
>```matlab
>theta = linspace(-pi/2,pi/2);
>phi = linspace(0,2*pi);
>[phi2,theta2] = meshgrid(phi,theta);
>dxy = 0.25*sqrt(15/pi)*sin(theta2+pi/2).^2.*sin(2*phi2);
>[x,y,z] = sph2cart(phi2,theta2,dxy);
>surf(x,y,z)
>```



