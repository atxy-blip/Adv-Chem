# Chapter 7: Approximation Methods                                   近似方法

## 7.1 The Variational Method Provides an Upper Bound to the Ground-State Energy of a System

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


$$
\hat { H } | \psi _ { n } \rangle = \varepsilon _ { n } | \psi _ { n } \rangle \quad n = 0,1
$$

$$
\langle \psi _ { n } | \psi _ { n } \rangle = \delta_{\alpha\beta}
$$

本征值$\{ | \psi _ { n } \rangle , n = 0,1,2 , \ldots \}$
$$
\varepsilon _ { 0 } \leq \varepsilon _ { 1 } \leq \varepsilon _ { 2 } \leq \cdots \leq \varepsilon _ { \alpha } \leq \cdots
$$


trial wave function $\varphi$

$$
E _ { \varphi } = \frac { \int \varphi ^ { * } \hat { H } \varphi \mathrm{d} \tau } { \int \varphi ^ { * } \varphi \mathrm{d} \tau } \geq \varepsilon _ { 0 }
$$

> #### Proof
>
> $$
> \varphi =\sum_{n} c_n \psi_n
> $$
>
> $$
> E _ { \varphi } = \frac { \int \varphi ^ { * } \hat { H } \varphi \mathrm{d} \tau } { \int \varphi ^ { * } \varphi \mathrm{d} \tau }
> = \frac { \int \sum _ { n } c _ { n } ^ { * } \psi _ { n } ^ { * } \hat { H } \sum _ { m } c _ { m } \psi _ { m } \mathrm{d} \tau } { \int \sum _ { n } c _ { n } ^ { * } \psi _ { n } ^ { * } \sum _ { m } c _ { m } \psi _ { m } \mathrm{d} \tau } = \frac { \sum _ { n } \sum _ { m } c _ { n } ^ { * } c _ { m } \int \psi _ { n } ^ { * } \hat { H } \psi _ { m } \mathrm{d} \tau } { \sum _ { n } \sum _ { m } c _ { n } ^ { * } c _ { m } \int \psi _ { n } ^ { * } \psi _ { m } \mathrm{d} \tau }
> $$
>
> $$
> \left. { \int \psi _ { n } ^ { * } \hat { H } \psi _ { m } \mathrm{d} \tau = \int \psi _ { n } ^ { * } ( \varepsilon _ { m } \psi _ { m } ) \mathrm{d} \tau = \varepsilon _ { m } \int \psi _ { n } ^ { * } \psi _ { m } \mathrm{d} \tau = \varepsilon _ { m } \delta _ { n m } } \\ 
> { \int \psi _ { n } ^ { * } \psi _ { m } \mathrm{d} \tau = \delta _ { n m } } \right.
> $$
>
> $$
> \left. { E _ { \varphi } = \frac { \sum _ { n } \sum _ { m } c _ { n } ^ { * } c _ { m } \varepsilon _ { m } \delta _ { n m } } { \sum _ { n } \sum _ { m } c _ { n } ^ { * } c _ { m } \delta _ { n m } } = \frac { \sum _ { n } c _ { n } ^ { * } c _ { n } \varepsilon _ { n } } { \sum _ { n } c _ { n } ^ { * } c _ { n } } } \\
> { E _ { \varphi } - \varepsilon _ { 0 } = \frac { \sum _ { n } c _ { n } ^ { * } c _ { n } \varepsilon _ { n } } { \sum _ { n } c _ { n } ^ { * } c _ { n } } - \frac { \varepsilon _ { 0 } \sum _ { n } c _ { n } ^ { * } c _ { n } } { \sum _ { n } c _ { n } ^ { * } c _ { n } } = \frac { \sum _ { n } c _ { n } ^ { * } c _ { n } ( \varepsilon _ { n } - \varepsilon _ { 0 } ) } { \sum _ { n } c _ { n } ^ { * } c _ { n } } \geq 0 } \right.
> $$

$$
E _ { \varphi } (\alpha,\beta,\gamma) \geq \varepsilon _ { 0 }
$$

> #### Example 7.1
>
> 

### Application of the Variational Method to Two-electron Problems

氦原子哈密顿
$$
\left. { \hat { H } = ( - \frac { \hbar ^ { 2 } } { 2 m _ { e } } \nabla _ { 1 } ^ { 2 } - \frac { 2 e ^ { 2 } } { 4 \pi \varepsilon _ { 0 } } \frac { 1 } { r _ { 1 } } ) + ( - \frac { \hbar ^ { 2 } } { 2 m _ { e } } \nabla _ { 2 } ^ { 2 } - \frac { 2 e ^ { 2 } } { 4 \pi \varepsilon _ { 0 } } \frac { 1 } { r _ { 2 } } ) + \frac { e ^ { 2 } } { 4 \pi \varepsilon _ { 0 } } \cdot \frac { 1 } { r _ { 12 } } }\\  \\{ = \hat { H } _ { H } ( 1 ) + \hat { H } _ { H } ( 2 ) + \frac { e ^ { 2 } } { 4 \pi \varepsilon _ { 0 } } \cdot \frac { 1 } { r _ { 12 } } } \right.
$$

$$
\begin{aligned}
E ( Z ) &= \int \Psi _ { 0 } ( x _ { 1 } , x _ { 2 } ) \hat { H } \Psi _ { 0 } ( x _ { 1 } , x _ { 2 } ) d x _ { 1 } d x _ { 2 } \\ 
&= \int \Omega ( \sigma _ { 1 } , \sigma _ { 2 } ) \Omega ( \sigma _ { 1 } , \sigma _ { 2 } ) d \sigma _ { 1 } d \sigma _ { 2 } \int \varphi _ { 0 } ( r _ { 1 } , r _ { 2 } ) \hat { H } \varphi _ { 0 } ( r _ { 1 } , r _ { 2 } ) d r _ { 1 } d r _ { 2 } \\
&= 1 \times \int \varphi _ { 0 } ( \vec{r} _ { 1 } , \vec{r} _ { 2 } ) \hat { H } \varphi _ { 0 } ( \vec{r} _ { 1 } , \vec{r} _ { 2 } ) d r _ { 1 } d r _ { 2 } \\
&= \frac { m _ { e } e ^ { 4 } } { 16 \pi ^ { 2 } \varepsilon _ { 0 } ^ { 2 } \hbar ^ { 2 } } ( Z ^ { 2 } - \frac { 27 } { 8 } Z )
\end{aligned}
$$


## 7.2 A Trial Function That Depends Linearly on the Variational Parameters Leads to a Secular Determinant

$$
| \Phi \rangle = \sum_{i=1}^{N} c _ { i } | \psi _ { i } \rangle
$$

$\{| \psi _ { i } \rangle\}$
$$
\langle \Phi | \Phi \rangle = \sum _ { i j } c _ { i } c _ { j } \langle \psi _ { i } | \psi _ { j } \rangle = \sum _ { i j } c _ { i } c _ { j } S _ { i j }
$$

$$
\langle \Phi | \hat { H } | \Phi \rangle = \sum _ { i j } c _ { i } \langle \psi _ { i } | \hat { H } | \psi _ { j } \rangle c _ { j } = \sum _ { i j } c _ { i } c _ { j } H _ { i j }
$$

$$
\langle \psi _ { i } | \hat { H } | \psi _ { j } \rangle = H _ { i j } = H _ { j i } , \quad \langle \psi _ { i } | \psi _ { j } \rangle = S _ { i j } = S _ { j i }
$$


$$
E = \frac { \langle \Phi | \hat { H } | \Phi \rangle } { \langle \Phi | \Phi \rangle } = \frac { \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } H _ { i j } } { \sum _ { j = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } S _ { i j } } \\
\sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } H _ { i j } = E \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } S _ { i j } \\
$$

$$
\frac { \partial } { \partial c _ { k } } \left( \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } H _ { i j } \right) = \frac { \partial E } { \partial c _ { k } } \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } S _ { i j } + E \frac { \partial } { \partial c _ { k } } \left( \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } S _ { i j } \right)
$$


$$
\frac { \partial } { \partial c _ { k } } ( \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } H _ { i j } ) = E \frac { \partial } { \partial c _ { k } } ( \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } S _ { i j } )
$$

$$
E \frac { \partial } { \partial c _ { k } } ( \sum _ { i = 1 } ^ { N } \sum _ { j = 1 } ^ { N } c _ { i } c _ { j } S _ { i j } ) = E ( \sum _ { i = 1 } ^ { N } c _ { i } S _ { i k } + \sum _ { j = 1 } ^ { N } c _ { j } S _ { k j } )
$$

$$
\sum _ { i = 1 } ^ { N } c _ { i } H _ { i k } + \sum _ { j = 1 } ^ { N } c _ { j } H _ { i j } = E ( \sum _ { i = 1 } ^ { N } c _ { i } S _ { i k } + \sum _ { j = 1 } ^ { N } c _ { j } S _ { k j } )
$$

$$
\sum _ { i = 1 } ^ { N } c _ { i } H _ { i k } = E \sum _ { i = 1 } ^ { N } c _ { i } S _ { i k }
$$

$$
\sum _ { i = 1 } ^ { N } ( H _ { i a } - E S _ { i k } ) c _ { i } = 0 \quad ( k = 1,2 , \cdots , N )
$$


$$
\begin{vmatrix}
{ H _ { 11 } - E S _ { 11 } } & { H _ { 1N } - E S _ { 1N } } &\cdots & { H _ { 1N } - E S _ { 1N } } \\ 
{ H _ { 12 } - E S _ { 12 } } & { H _ { 22 } - E S _ { 22 } } &\cdots & { H _ { 2N } - E S _ { 2N } } \\
\vdots &\vdots &\ddots &\vdots \\
{ H _ { 1N } - E S _ { 1N } } & { H _ { 2N } - E S _ { 2N } } &\cdots & { H _ { NN } - E S _ { NN } }
\end{vmatrix} = 0
$$
secular determinant ( 久期行列式


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

$$
Hc=ESc
$$

$$
\vec{C} = \begin{pmatrix} { c _ { 1 } } &{ c _ { 2 } } &\cdots &{ c _ { N } } \end{pmatrix} =
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

$$
HC=SC\varepsilon
$$



## 7.3 Trial Functions Can Be Linear Combination of Functions that Also Contain Variational Parameters
$$
\phi=\sum_{j=1}^{N}c_jf_j
$$

氢原子
$$
\phi=\sum_{j=1}^{N}c_je^{-\alpha_jr^2}
$$

## 7.4 Perturbation Theory Expresses the Solution to One Problem in Terms of Another Problem Solved Previously


$$
H = H _ {0} + \lambda \nu \\
E _ { i } = E _ { i } ^ { ( 0 ) } + \lambda E _ { i } ^ { ( 1 ) } + \lambda ^ { 2 } E _ { i } ^ { ( 2 ) } + \cdots \\
| \Phi _ { i } \rangle = | \psi _ { i } ^ { ( 0 ) } \rangle + \lambda | \psi _ { i } ^ { ( 1 ) } \rangle + \lambda ^ { 2 } | \psi _ { i } ^ { ( 2 ) } \rangle + \cdots
$$

$$
\langle i | \Phi _ { i } \rangle = \langle i | i \rangle + \lambda \langle i | \psi _ { i } ^ { ( 1 ) } \rangle + \cdots = 1
$$

$$
( H _ { 0 } + \lambda v ) ( | i \rangle + \lambda | \psi _ { i } ^ { ( 1 ) } \rangle + \lambda ^ { 2 } | \psi _ { i } ^ { ( 2 ) } \rangle + \cdots ) \\ 
= ( E _ { i } ^ { ( 0 ) } + \lambda E _ { i } ^ { ( 1 ) } + \lambda ^ { 2 } E _ { i } ^ { ( 2 ) } + \cdots ) ( | i \rangle + \lambda | \psi _ { i } ^ { ( 1 ) } \rangle + \cdots )
$$


$$
\langle n | ( E _ { i } ^ { ( 0 ) } - H _ { 0 } ) | \psi _ { i } ^ { ( 1 ) } \rangle = \langle n | v - E _ { i } ^ { ( 1 ) } | i \rangle = \langle n | v | i \rangle ( n \neq i )
$$
