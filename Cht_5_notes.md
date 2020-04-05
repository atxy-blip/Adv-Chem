# Chapter 5: The Harmonic Oscillator and the Rigid Rotator: Two Spectroscopic Models        简谐振子和刚性转子：两种光谱模型

对于双原子分子，振动=>简谐振子，转动=>刚性转子

## 5.1 Reduction of the two-particle problem to 2 one-particle problem                             将两体问题转化为两个单体问题

### Transformation of coordinates                                                                                                       坐标变换

对于质点$m_1,m_2$，其坐标分别为$\vec{r}_1\left(x_1,y_1,z_1\right),\ \vec{r}_2\left(x_2,y_2,z_2\right)$，对于其质心有
$$
\vec{R}:C\left(X,Y,Z\right),\quad \vec{R}=\frac{m_1\vec{r}_1+m_2\vec{r}_2}{m_1+m_2}
$$
对于其相对运动有
$$
\vec{r}:\left(x,y,z\right),\quad \vec{r}=\vec{r}_2-\vec{r}_1
$$
将$\vec{r_2}=\vec{r}+\vec{r_1}$代入质心表达式得
$$
\vec{R}=\frac{m_1\vec{r}_1+m_2\left(\vec{r}+\vec{r}_1\right)}{m_1+m_2}=\vec{r}_1+\frac{m_2}{m_1+m_2}\vec{r}
$$
完成了$x_1,y_1,\ z_1;x_2,y_2,z_2=>X,Y,Z;\ x,y,z$的坐标变换

### Transformation of kinetic energy                                                                                                                                                                                 动能变换

动能计算式为
$$
T=\frac{1}{2}m_1\left|\dot{\vec{r}}_1\right|^2+\frac{1}{2}m_2\left|\dot{\vec{r}}_2\right|^2
$$
由前一节得
$$
\dot{\vec{r}}_1=\dot{\vec{R}}-\frac{m_2}{m_1+m_2}\dot{\vec{r}},\quad \dot{\vec{r}}_2=\dot{\vec{R}}+\frac{m_1}{m_1+m_2}\dot{\vec{r}}
$$
再令$C_1=-\frac{m_2}{m_1+m_2},C_2=\frac{m_1}{m_1+m_2}$，代入动量计算式并展开得
$$
T=\frac{1}{2}\left(m_1+m_2\right)\left|\dot{\vec{R}}\right|^2+\left(m_1C_1+m_2C_2\right)\dot{\vec{R}}\cdot\dot{\vec{r}}+\frac{1}{2}\left(m_1C_1^2+m_2C_2^2\right)\left|\dot{\vec{r}}\right|^2
$$
由定义可知$m_1C_1+m_2C_2=0,\ m_1C_1^2+m_2C_2^2=\frac{m_1m_2}{m_1+m_2}$，再定义总质量$M=m_1+m_2$，==约化质量*(reduced mass)*$\mu=\frac{m_1m_2}{m_1+m_2}$==，最终得到
$$
T=\frac{1}{2}M\left|\dot{\vec{R}}\right|^2+\frac{1}{2}\mu\left|\dot{\vec{r}}\right|^2
$$
动能转化为新的两项，为二分之一的。总质量乘以质心的平动速度的平方加约化质量乘以两点相对运动速度的平方，第一项代表平移，第二项代表相对运动。对于$\vec{r}$，==距离的改变代表振动*(vibration)*，方向的改变代表转动*(rotation)*。==

### The Hamiltonian is the sum of 2 independent terms                                                                                哈密顿算符为两个独立项的和

$$
T=\frac{\left|\dot{\vec{P}}_M\right|^2}{2M}+\frac{\left|\dot{\vec{P}}_\mu\right|^2}{2\mu}
$$

写出对应的哈密顿算符，并给相对运动加上势能函数。势函数只与两点距离有关，与质心无关。经过这一变换后，哈密顿算符可拆分为==两项相加==，前一项与R即质心有关，后一项与分子内部xyz有关。该变换是严格的。
$$
\hat{H}=\hat{H}_{\text{tr}}+\hat{H}_{\text{int}},\quad \hat{H}_{\text{tr}}=-\frac{\hbar^2}{2M}{\nabla_R}^2,\quad \hat{H}_{\text{int}}=-\frac{\hbar^2}{2\mu}\nabla^2+V\left(x,y,z\right)
$$
在进行变换之前，势能项与六个变量有关，哈密顿算符无法拆分。
$$
\hat{H}=-\frac{\hbar^2}{2m_1}{\nabla_1}^2-\frac{\hbar^2}{2m_2}{\nabla_2}^2+V\left(x_1,y_1,z_1,x_2,y_2,z_2\right)
$$

> *tr for translational, int for interactive*

###  Schrödinger equation for translational motion and its energy                                                                                                                                                                                平动的薛定谔方程以及能量

如果哈密顿能写成两项相加的形式，波函数能写成两项哈密顿对应的==波函数再相乘==。对应的能量变成==两个运动的能量相加==。
$$
\Psi\left(X,Y,Z,x,y,z\right)=\Lambda\left(X,Y,Z\right)\Psi\left(x,y,z\right),\quad E=E_{\text{tr}}+E_{\text{vr}}
$$
平动运动的薛定谔方程如下。平面波。质心的运动类似于自由粒子，只有动能项，势能项为零。能量总是大于等于0，非量子化。
$$
-\frac{\hbar^2}{2M}{\nabla_R}^2\Lambda\left(X,Y,Z\right)=E_{\text{tr}}\Lambda\left(X,Y,Z\right),\quad \Lambda\left(X,Y,Z\right)=Ae^{i\vec{K}\cdot\vec{R}}
$$

$$
E_{\text{tr}}=\frac{K^2\hbar^2}{2M}\geq0
$$

### Schrödinger equation for relative motion                                                                                                相对运动的薛定谔方程

$$
\left[-\frac{\hbar^2}{2\mu}\nabla^2+V\left(x,y,z\right)\right]\Psi\left(x,y,z\right)=E_{\text{vr}}\Psi\left(x,y,z\right)
$$

该方程包括振动运动和转动运动。对双原子分子有$M=m_1+m_2,\ \mu=\frac{m_1m_2}{m_1+m_2}$，对于氢原子有$M=m_e+m_p,\ \mu=\frac{m_em_p}{m_e+m_p}$，后者的约化质量约为0.98电子质量。

> *vr = vib + rot, represents relative motion*

## 5.2 Rotational Hamiltonian of a diatomic molecule in the rigid rotor approximation                                                                                                                                                                                                                                              刚性转子近似中双原子分子的转动哈密顿算符

### Derivation of the Hamiltonian for the rotation                                                                                                     推导转动哈密顿算符

为了计算方便，将笛卡尔坐标系变换为球极坐标系，有==（变换方式？==
$$
\hat { H } _ { int } = - \frac { \hbar ^ { 2 } } { 2 \mu } \nabla ^ { 2 } + V ( x , y , z ) = - \frac { \hbar ^ { 2 } } { 2 \mu } \left( \frac { \partial ^ { 2 } } { \partial r ^ { 2 } } + \frac { 2 } { r } \frac { \partial } { \partial r } - \frac { 1 } { r ^ { 2 } \hbar ^ { 2 } } \hat { L } ^ { 2 } \right) + V ( r )
$$

$$
\hat { L } ^ { 2 } = - \hbar ^ { 2 } \left[ \frac { 1 } { \sin \theta } \frac { \partial } { \partial \theta } \left( \sin \theta \frac { \partial } { \partial \theta } \right) + \frac { 1 } { \sin ^ { 2 } \theta } \frac { \partial ^ { 2 } } { \partial \varphi ^ { 2 } } \right]
$$

对于两个粒子的刚性转子的转动，有==$\left|\vec{r}\right|=r_e$==，值为常数；势能只和距离有关，势函数$V ( x , y , z ) = V ( r ) = 0$；同时对r求导也为零，$- \frac { \hbar ^ { 2 } } { 2 \mu } \left( \frac { \partial ^ { 2 } } { \partial r ^ { 2 } } + \frac { 2 } { r } \frac { \partial } { \partial r } \right) = 0$。化简后最终得到：
$$
\hat{H}_{\text {rot}}=\frac{\hat{L}^{2}}{2 \mu r_{e}^{2}}=\frac{\hat{L}^{2}}{2 I} \quad\left(I=\mu r_{e}^{2}=\frac{m_1m_2}{m_1+m_2}r_{e}^{2}\right)
$$

上式只包括两个变量$\theta,\phi$。其中$I$定义为==转动惯量*(moment of inertia)*==。

### Another way of deriving the rotational Hamiltonian of a diatomic molecule                                                                                                推导转动哈密顿算符的另一种方法

![Fig 5.2](S:\我的资料库\课程\高等物理化学\Cht_5\Fig 5.2.png)

如图5.2，两粒子的速度分别为$v_{1}=r_{1} \omega, \ v_{2}=r_{2} \omega$，根据经典力学计算其动能：
$$
r_1=\frac{m_2}{m_1+m_2}r_{e},\quad C_2=\frac{m_1}{m_1+m_2}r_{e},\quad r_{e}=r_{1}+r_{2}
$$

$$
m_{1} r_{1}^{2}+m_{2} r_{2}^{2}=\frac{m_{1} m_{2}}{m_{1}+m_{2}}r_{e}^{2}=\mu r_{e}^{2}=I
$$

$$
K=\frac{1}{2} m_{1} v_{1}^{2}+\frac{1}{2} m_{2} v_{2}^{2}=\frac{1}{2}\left(m_{1} r_{1}^{2}+m_{2} r_{2}^{2}\right) \omega^{2}=\frac{1}{2} I \omega^{2}=\frac{L^{2}}{2I}\quad \left(L=I\omega\right)
$$

其中$L$为角动量，换成算符就得到刚性转子的哈密顿算符：
$$
\hat{H}_{\text {rot}}=\frac{\hat{L}^{2}}{2 I}
$$
可知$\left[\hat{H}_{\text{rot}}, \hat{L}^{2}\right]=0$，==转动运动的算符和角动量算符的平方是对易的==，两者有共同的本征函数，即一个球谐函数，对此的进一步讨论见第六章。
$$
\hat{L}^{2} Y_{J}^{m}(\theta, \varphi)=J(J+1) \hbar^{2} Y_{J}^{m}(\theta, \varphi), \quad J=0,1,2, \ldots, \quad m=0,\pm 1, \ldots, \pm J
$$
故==转动哈密顿的本征函数是球谐函数==，本征值$E_{\text {rot}}$取值与$m$无关，具有一定的==简并度==。
$$
\hat{H}_{\text {rot}} Y_{J}^{m}(\theta, \varphi)=E_{\text {rot}} Y_{J}^{m}(\theta, \varphi)
$$

$$
E_{\text {rot}}=\frac{J(J+1) \hbar^{2}}{2 I}, \quad g_JJ=2J+1
$$

## 5.3 Vibrational Hamiltonian of a diatomic molecule in the rigid rotor approximation                                                                                                                                                                    刚性转子近似中的振动哈密顿算符

### Vibrational Schrödinger equation                                                                                               振动运动的薛定谔方程

相对运动哈密顿为三项：
$$
\hat{H}_{\mathrm{int}}=-\frac{\hbar^{2}}{2 \mu}\left(\frac{\partial^{2}}{\partial r^{2}}+\frac{2}{r} \frac{\partial}{\partial r}\right)+\frac{1}{2 \mu r^{2}} \hat{L}^{2}+V(r)
$$

第一项跟$r$有关，第二项与$\theta,\psi$有关，分别作用在不同的变量上，其线性组合$\hat{H}_{\text{int}}, \hat{L}^{2}$互相对易，亦即$\left[\hat{H}_{\text{int}}, \hat{L}^{2}\right]=0$。
$$
\hat{L}^{2}=-{\hbar}^{2}\left[\frac{1}{\sin\theta}\frac{\partial}{\partial \theta}\left(\sin\theta\frac{\partial}{\partial \theta}\right)+\frac{1}{\sin^2\theta}\frac{\partial^{2}}{\partial \phi^{2}}\right]
$$

> $\left[ {\hat {A}},{\hat {B}} \right] \stackrel {def}{=} {\hat {A}}{\hat {B}}-{\hat {B}}{\hat {A}}$
>
> 如果上式等于零，则称$\hat {A},\hat {B}$是***对易***的，即意味着$\hat {A},\hat {B}$两个算符的运算顺序***可以调换***。反之则称**非对易**的，运算顺序不可以调换。
>
> 假设$\left[ {\hat {A}},{\hat {B}} \right]= 0 $，则称这两种可观察量为“相容可观察量”。假设两种可观察量为*不相容可观察量*，则由于*不确定原理*，绝无法制备出这两种可观察量在任意精确度内的量子系统。

通过对易，可知相对运动的哈密顿和角动量算符的平方具有共同的本征函数，因此可以将相对运动的本征函数$\Psi(r,\theta, \varphi)$写成与空间部分$r$有关的$\psi(r)$和与角度部分$\theta,\psi$有关的球谐函数的乘积，即==$\Psi(r,\theta, \varphi)=\psi(r) Y_{J}^{m}(\theta, \varphi)$==。在相对运动的薛定谔方程中代入$\hat{H}_{\mathrm{int}},\Psi(r,\theta, \varphi)$，将与算符无关的项看作常数提出，进行简化可以得到：
$$
\hat{H}_{\mathrm{int}} \Psi(r, \theta, \varphi)=E_{\text{vr}} \Psi(r, \theta, \varphi)
$$

$$
\begin{aligned}

&-\frac{\hbar^{2}}{2 \mu}\left(\frac{\partial^{2} \psi(r)}{\partial r^{2}}+\frac{2}{r} \frac{\partial \psi(r)}{\partial r}\right) Y_{J}^{m}(\theta, \varphi)+\frac{\psi(r)}{2 \mu r^{2}} {\hat{L}}^{2} Y_{J}^{m}(\theta, \varphi)+{V}({r}) \psi(r) Y_{J}^{m}(\theta, \varphi) \\
&=E_{\text{vr}} \psi(r) Y_{J}^{m}(\theta, \varphi)
\end{aligned}
$$
运用角动量算符平方的本征值关系$\hat{L}^{2} Y_{J}^{m}(\theta, \varphi)=J(J+1) \hbar^{2} Y_{J}^{m}(\theta, \varphi)$在方程两边约去球谐函数$Y_{J}^{m}(\theta, \varphi)$，得到的新方程只和$\psi(r)$有关：
$$
-\frac{\hbar^{2}}{2 \mu}\left(\frac{\partial^{2} \psi(r)}{\partial r^{2}}+\frac{2}{r} \frac{\partial \psi(r)}{\partial r}\right)+\frac{J(J+1) \hbar^{2}}{2 \mu r^{2}} \psi(r) +{V}({r}) \psi(r) 
=E_{\text{vr}} \psi(r)
$$
再令$f(r)=r\psi(r)$，两边求二阶导数：
$$
\frac{\partial^{2} \psi(r)}{\partial r^{2}}+\frac{2}{r} \frac{\partial \psi(r)}{\partial r}=\frac{1}{r} \frac{\partial^{2} f(r)}{\partial r^{2}}
$$

使用这一关系进一步化简薛定谔方程得：
$$
-\frac{\hbar^{2}}{2 \mu} \frac{\mathrm{d}^{2} f(r)}{\mathrm{d} r^{2}}+\frac{J(J+1) \hbar^{2}}{2 \mu r^{2}} f(r)+V(r) f(r)=E_{\text{vr}} f(r)
$$

令$r={r}_{e}+x$，==$x$为振动中相对平衡位置${r}_{e}$的位移==，定义$\chi(x)=f(r_e+x)=r\psi(r)$，易知：
$$
\frac{\mathrm{d}^{2} f(r)}{\mathrm{d} r^{2}}=\frac{\mathrm{d}}{\mathrm{d} r}\left(\frac{\mathrm{d} f(r)}{\mathrm{d} r}\right)=\frac{\mathrm{d}}{\mathrm{d} x}\frac{\mathrm{d} x}{\mathrm{d} r}\left(\frac{\mathrm{d} f(r_e+x)}{\mathrm{d} x}\frac{\mathrm{d} x}{\mathrm{d} r}\right)=\frac{\mathrm{d}^{2} \chi(x)}{\mathrm{d} x^{2}}
$$

> e in ${r}_{e}$ represents *equilibrium*

代入得：
$$
-\frac{\hbar^{2}}{2 \mu} \frac{\mathrm{d}^{2} \chi(x)}{\mathrm{d} x^{2}}+\frac{J(J+1) \hbar^{2}}{2 \mu\left(x+r_{e}\right)^{2}} \chi(x)+V\left(x+r_{e}\right) \chi(x)=E_\text{vr} \chi(x)
$$

设位移远小于平衡键长，==$x\ll{r}_{e}$==，引入刚性转子近似有：
$$
\frac{J(J+1) \hbar^{2}}{2 \mu\left(x+r_{e}\right)^{2}} \approx \frac{J(J+1) \hbar^{2}}{2 \mu r_{e}^{2}}=\frac{J(J+1) \hbar^{2}}{2 I}=E_{\text {rot}}
$$

振动薛定谔方程最终化简如下。通过以上推导，我们将相对运动的哈密顿分解为转动项和振动项，实现了两者的分别处理。
$$
-\frac{\hbar^{2}}{2 \mu} \frac{\mathrm{d}^{2} \chi(x)}{\mathrm{d} x^{2}}+V\left(x+r_{e}\right) \chi(x)=(E_\text{vr}-E_\text{rot}) \chi(x)=E_\text{vib} \chi(x)
$$

## 5.4 The harmonic oscillator is a good model for the vibrational motion of a diatomic molecule                                                                                                                              简谐振子模型与双原子分子相当符合

### Harmonic oscillator potential                                                                                                                                                                    简谐振子势

根据势函数图像，$r={r}_{e}$为极小值，$r\rightarrow +\infty$时趋向一个确定值。

在${r}_{e}$附近对势函数作泰勒展开得：
$$
V\left(x+r_{e}\right)=V\left(r_{e}\right)+\left(\frac{d V}{d x}\right)_{x=0} x+\frac{1}{2}\left(\frac{d^{2} V}{d x^{2}}\right)_{x=0} x^{2}+\cdots
$$

取极小值点为能量零点，$V\left(r_{e}\right)=0$，在该点一阶导数等于零，$\left(\frac{d V}{d x}\right)_{x=0} =0$，令$k=\left(\frac{d^{2} V}{d x^{2}}\right)_{x=0}$，得到近似关系，为一条抛物线：
$$
V\left(x+r_{e}\right) \approx \frac{1}{2} k x^{2}
$$

该近似称为简谐振子势，即势函数在平衡位置附近为简谐振子势。再将此形式代入上一节得到的双原子分子振动运动的薛定谔方程中：
$$
\left[-\frac{\hbar^{2}}{2 \mu} \frac{\mathrm{d}^{2}}{\mathrm{d} x^{2}}+\frac{1}{2} k x^{2}\right] \chi(x)=E_{\text {vib}} \chi(x)
$$

### Classical harmonic oscillator                                                                                                                                                                                                                                                      经典力学中的简谐振子

质量忽略不计的轻质小球，弹力服从胡克定律：
$$
f=-k(l-l_0)=-kx
$$
力也可以表示为势函数对位移求导的负值，$f=-\frac{\mathrm{d}V}{\mathrm{d} x}$，移项两边进行不定积分：
$$
V(x)=-\int{f(x)\mathrm{d} x}=-\int{(-kx)\mathrm{d} x}=\frac{1}{2} k x^{2}+\text{constant}
$$
取平衡位置为势能零点，常数项为零，可以得到经典力学中简谐振子的势函数：
$$
V(x)=\frac{1}{2} k x^{2}
$$

$$
x(t)=C\sin(\omega t+\phi)\quad w=\sqrt{\frac{k}{m}}
$$

### Schrödinger equation for a harmonic oscillator

再考虑动能，可以得到简谐振子的哈密顿：
$$
E = T + V = \frac { 1 } { 2 } m \left( \frac { \mathrm{d} x } { \mathrm{d} t } \right) ^ { 2 } + \frac { 1 } { 2 } k x ^ { 2 } = \frac {  { p } _ { x } ^ { 2 } } { 2 m } + \frac { 1 } { 2 } k x ^ { 2 }
$$
据此可以得到简谐振子的哈密顿并写出薛定谔方程，并与双原子分子的振动薛定谔方程进行比较：
$$
\begin{aligned}
\left[ - \frac{ \hbar ^ { 2 } }{ 2 m } \frac{\mathrm{d}^{2}}{\mathrm{d} x^{2}} + \frac { 1 } { 2 } k x ^ { 2 } \right] \chi ( x ) &= E \chi ( x ) \\
\left[ - \frac{ \hbar ^ { 2 } }{ 2 \mu } \frac{\mathrm{d}^{2}}{\mathrm{d} x^{2}} + \frac { 1 } { 2 } k x ^ { 2 } \right] \chi ( x ) &= E_{\text{vib}} \chi ( x )
\end{aligned}
$$
两者的区别仅在于后者使用约化质量$\mu$。
$$

$$

> ### Example 5.1
>
> Morse potential:
> $$
> V ( x ) = D ( 1 - e ^ { - \beta (l-l_0)} ) ^ { 2 }
> $$
> $x=l-l_{0}$：
> $$
> V ( x ) = D ( 1 - e ^ { - \beta x } ) ^ { 2 }
> $$
> Where $D,B$  are parameters. The parameter $D$ is the dissociation energy of the molecule (relative to the minimum of $V(l)$) and $B$ is a measure of the curvature of  $V(l)$ at its minimum.
>
> $x={0}$：
> $$
> V ( 0 ) = 0, \quad \left( \frac { \mathrm{d} V } { \mathrm{d} x } \right) _ { x = 0 } = \left\{ 2 D \beta ( e ^ { - \beta x } - e ^ { - 2 \beta x } ) \right\} _ { x = 0 } = 0
> $$
> $$
> \left( \frac { \mathrm{d}^2 V } { \mathrm{d} x^2 } \right) _ { x = 0 } = \left\{ -2 D \beta ( \beta e ^ { - \beta x } - 2\beta e ^ { - 2 \beta x } ) \right\} _ { x = 0 } = 2 D \beta^2
> $$
> Therefore,
> $$
> V ( x )=2 D \beta^2x^2+\cdots
> $$
> Comparing this result with $V(x)=\frac{1}{2} k x^{2}$ gives
> $$
> k=2 D \beta^2
> $$

## 5.5 Energy levels of a rigid rotator                                                                                     刚性转子的能级

在前几节中我们得到了刚性转子的薛定谔方程：
$$
-\frac{h^{2}}{2 I}\left[\frac{1}{\sin \theta} \frac{\partial}{\partial \theta}\left(\sin \theta \frac{\partial}{\partial \theta}\right)+\frac{1}{\sin ^{2} \theta} \frac{\partial^{2}}{\partial \varphi^{2}}\right] Y(\theta, \varphi)=E_{\text {rot}} Y(\theta, \varphi)
$$

它的本征函数是一个与$\theta,\varphi$有关的球谐函数，能级公式如下：
$$
\hat{H}_{\text {rot}} Y_{J}^{m}(\theta, \varphi)=E_{\text {rot}} Y_{J}^{m}(\theta, \varphi)  \quad J=0,1,2,\cdots \quad m=0,\pm 1, \ldots, \pm J
$$

$$
E_{\text {rot}}=\frac{\hbar^2}{2I}J\left(J+1\right) \quad J=0,1,2,\cdots
$$

可见：

1. 转动能级是量子化的；

2. $(E_{\text {rot}})_{J=0}=0$，没有零点转动能；

3. 对于每一个确定的$J$，$m$可以取$-J$到$J$共$2J+1$个值，简并度为$g_J=2J+1$。

## 5.6 Rotational spectrum of a diatomic molecule                                                                                  双原子分子的转动能级

### Rotational transitions occur in the microwave region

电磁辐射可以使刚性转子从一个态转变为另一个。通过量子力学计算可以得出跃迁能否发生。

选择律：

1. 跃迁只发生在相邻能级，$\Delta J=\pm 1$
2. 分子具有永久的偶极矩，同核双原子分子不满足此条

在吸收过程中，能级为：
$$
\begin{aligned}
\Delta E &=E_{J+1}-E_{J}=\frac{\hbar^{2}}{2 I}[(J+1)(J+2)-J(J+1)] \\
&=\frac{\hbar^{2}}{I}(J+1)=\frac{h^{2}}{4 \pi^{2} I}(J+1)=h \nu
\end{aligned}
$$

可以得到频率和波数：
$$
{\nu}=2{B}(J+1)  \quad J=0,1,2,\cdots \quad {B}=\frac{h}{8\pi^2I} \\
\tilde{\nu}=2\tilde{B}(J+1)  \quad J=0,1,2,\cdots \quad \tilde{B}=\frac{h}{8\pi^2cI}
$$

其中$B$称为分子的转动常数，$\tilde{B}$称为分子的
$$
\Delta{\nu}=2{B}(J+2)-2{B}(J+1)=2{B} \\
\Delta\tilde{\nu}=2\tilde{B}(J+2)-2\tilde{B}(J+1)=2\tilde{B}
$$

转动光谱是由一系列间隔等差的线组成的。通过吸收频率的间隔可以计算出双原子分子的键长。
$$
{B}=\frac{h}{8\pi^2I} \Rightarrow {I}=\frac{h}{8\pi^2B} \Rightarrow r_{e}=\sqrt{\frac{I}{\mu}}=\sqrt{\frac{h}{8\pi^2B\mu}}
$$


## 5.7 Energy levels of a quantum-mechanical harmonical oscillator                                                                                  量子力学的简谐振子的能级

$$
-\frac{\hbar^{2}}{2 u} \frac{d^{2} \psi}{d x^{2}}+\frac{1}{2} k x^{2} \psi(x)=E \psi(x)
$$

$$
\frac{d^{2} \psi}{d x^{2}}+\frac{2 u}{\hbar^{2}}\left(E-\frac{1}{2} k x^{2}\right) \psi(x)=0
$$

$$
E_\nu=\hbar\sqrt{\frac{k}{\mu}}\left(\nu+\frac{1}{2}\right)
$$

具有大小为$E_0=\frac{\hbar}{2}\sqrt{\frac{k}{\mu}}$的零点能

## 5.8 The harmonic oscillator accounts for the infrared spectrum of a diatomic molecule                                                                                                                                                                    简谐振子 双原子分子的红外光谱

$\Delta E = E _ { n + 1 } - E _ { n } = \hbar \sqrt{\frac{k}{\mu}}$
$$
\nu _ { \text{obs}} = \frac { 1 } { 2 \pi } \sqrt{\frac{k}{\mu}}\quad \text { or } \quad \tilde { \nu } _ {\text{obs}} = \frac { 1 } { 2 \pi c } \sqrt{\frac{k}{\mu}} ( \text{cm} ^ { - 1 } )
$$

$$
k=\left(2\pi c\tilde { \nu } _ {\text{obs}}\right)^2u
$$

u reduced mass force constant

## 5.9 Wave function of the harmonic oscillator                                                                                  简谐振子的波函数

$$
\psi _ { n } ( x ) = N _ { n } H _ { n } ( \alpha ^ {\frac{ 1 }{ 2 }} x ) e ^{- \frac{  \alpha x ^ { 2 }} { 2 }} \quad \alpha =  \sqrt{\frac { k \mu } { \hbar ^ { 2 } } }
$$

Hermite厄密多项式
$$
\begin{aligned}
H_0(\xi)&=1 &H_1(\xi)&=2\xi\\
H_2(\xi)&=4\xi^2-2 &H_3(\xi)&=8\xi^3-12\xi\\
H_4(\xi)&=16\xi^4-48\xi^2+12 &H_5(\xi)&=32\xi^5-160\xi^3+120\xi
\end{aligned}
$$
归一化常数
$$
N_n=\frac{1}{\sqrt{2^{n}n!}}\left( \frac { \alpha } { \pi } \right) ^ { \frac{ 1 }{ 4 } }
$$
波函数
$$
\begin{aligned}
&\psi _ { 0 } ( x ) = \left( \frac { \alpha } { \pi } \right) ^ { \frac{ 1 }{ 4 } } e ^ { - \frac{  \alpha x ^ { 2 }} { 2 } } &
&\psi _ { 1 } ( x ) = \left( \frac { 4\alpha ^ { 3 } } {  \pi } \right) ^ { \frac{ 1 }{ 4 } } x e ^ { - \frac{  \alpha x ^ { 2 }} { 2 } } \\
&\psi _ { 2 } ( x ) = \left( \frac { \alpha  } { 4 \pi } \right) ^ { \frac{ 1 }{ 4 } } ( 2 \alpha x ^ { 2 } - 1 ) e ^ { - \frac{  \alpha x ^ { 2 }} { 2 } } &
&\psi _ { 3 } ( x ) = \left( \frac { \alpha ^ { 3 } } { 9 \pi } \right) ^ { \frac{ 1 }{ 4 } } ( 2 \alpha x ^ { 3 } - 3 x ) e ^ { - \frac{  \alpha x ^ { 2 }} { 2 } }
\end{aligned}
$$

算符
$$
\hat{K}(x)=- \frac{ \hbar ^ { 2 } }{ 2 \mu } \frac{\mathrm{d}^{2}}{\mathrm{d} x^{2}} \quad \hat{V}(x)=\frac { 1 } { 2 } k x ^ { 2 }
$$

$$
\left \langle K \right \rangle = \left \langle V \right \rangle
$$

> #### Gamma function & Gauss integer
>
> $\Gamma$函数可以通过欧拉第二类积分定义：
> $$
> \Gamma (n)=\int _{0}^{\infty }{\frac {t^{n-1}}{\mathrm {e} ^{t}}}{\mathrm{d} t} \\
> \Gamma(n + 1) = n \Gamma(n) \\
> \Gamma\left(\frac{1}{2}\right)=\sqrt {\pi }, \quad \Gamma(1)=1
> $$
> 对于整数$n$有：
> $$
> \Gamma(n + 1)=n!
> $$
> 高斯积分:
> $$
> \int _{-\infty }^{\infty }e^{-x^{2}}dx={\sqrt {\pi }} \\
> \int_{0}^{\infty}x^ne^{-\alpha{x}^2}\mathrm{d}x=\frac{\Gamma\left(\frac{n+1}{2}\right)}{2\alpha^{\frac{n+1}{2}}}
> $$
>



## Supplementary materials                                                                                                                                         补充材料

### The Vibrations of Polyatomic Molecules

多原子分子：
$$
E_{vib}=\sum_{j=1}^{N_{vib}}h\nu_{j}\left ( n_{j}+ \frac{1}{2}\right )
$$


对于三原子非线性分子水有$N_{vib}=3\times 3-6=3$



