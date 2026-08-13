# 三项十进制拼接平方和问题：临界 G 模板终端商冲刺

## 1. UB1 的启发与 G 系统

本文只研究临界层

\[
(\delta_2,\delta_3)=(-1,1),\qquad N_L=1
\]

中的

\[
\mathrm G:\qquad 2\mid g.
\]

按任务约定，本文暂时接受 T1–T18、K5、CG1–CG6、E4、CKD、CKA、
CKO、OSC 和 UB1，不作全项目统一审计。本文不研究 O、Q，不增加
Gram 模 \(2^j\) 条件，也不返回高斯下降、Vieta 跳跃或一般 Pell 方程。

UB1 在 O 中使用的关键事实是：终端商一旦越过真实十进制上端，
循环恢复就迫使 \(b_2=T/10\)，随后精确 \(2\)-进赋值矛盾。
G 中仍有同一类端点刚性，但尺度不再是固定的 \(Y\)，而是

\[
\boxed{E=\frac{b_1Y}{v}}.
\]

而且越过上端后并不总是矛盾：它会产生一个只存在于 G–B 的刚性边界族。
因此本轮的最终分类是

\[
\boxed{\mathrm{GT4}}.
\]

准确含义如下。

1. 定义
   \[
   \chi=gk-\frac Yv.
   \]
   则 \(\chi\) 总是正偶整数，并满足
   \[
   q\chi=g+\frac{TY}{u},\qquad
   vb_2\chi=b_1TY+b_3.
   \]
2. 对所有 G 候选，\(E=b_1Y/v\) 是整数，并且恰有以下两种情形：
   \[
   E<\chi<10E,
   \]
   或
   \[
   \chi=10E+g,\qquad
   b_2=\frac T{10},\quad q=1,\quad
   T=\frac{10b_1u}{v}.
   \]
3. 第二种情形在 G–A 中由精确 \(2\)-进赋值排除，在 G–C、G–D
   中由 \(c\) 的位置排除，只能留在 G–B 的三个显式边界子室。
4. 因而若定义欧几里得终端状态
   \[
   \boxed{
   J=\left\lfloor\frac{\chi}{E}\right\rfloor
   =\left\lfloor\frac{T}{b_2}\right\rfloor,
   \qquad
   \rho_J=\chi-JE,
   }
   \]
   则全部 E4 剩余室都满足
   \[
   J\in\{1,\ldots,9\},
   \]
   或处于唯一类型的 G–B 上端状态
   \[
   J=10,\qquad \rho_{10}=g.
   \]
   在所有情形中
   \[
   0<\rho_J<E.
   \]

这里“有限终端商化”指有限的欧几里得商状态 \(J\)，不表示
\(\chi\) 本身只取有限多个值。事实上 G–B 的 \(J=10\) 状态存在满足
全部分母窗口、循环方程、K5 支撑和 E4 高阶二进门的无界辅助族。
所以本轮没有关闭 G，没有关闭任何一个完整 E4 剩余室，也没有给
\(a,m,n,\eta,j,\theta_A,\theta_B,\kappa\) 建立统一上界。

全文严格分为三个阶段，每阶段只有三个核心引理：

- 阶段 I：GT-I.1–GT-I.3，终端商正规化；
- 阶段 II：GT-II.1–GT-II.3，整数窗口与端点刚性；
- 阶段 III：GT-III.1–GT-III.3，逐室有限状态化与反例证书。

### 1.1 范围内的 G 正规形与 E4 状态表

记

\[
m=\beta_2\ge2,\qquad n=\beta_3\ge1,
\qquad T=10^m,\qquad Y=10^n,\qquad M=m+n.
\]

G 正规形为

\[
r=1,\qquad
g=2^ag_0,\qquad
u=2^c5^e,\qquad
v=2^d,
\]

\[
a\ge1,\qquad d\in\{0,1\},\qquad cd=0,
\]

其中 \(q,g_0\) 为奇数。再记

\[
s=\nu_2(b_1)\in\{0,1\}.
\]

分母重构与窗口为

\[
\boxed{
b_2=\frac{b_1qu}{v},\qquad
b_3=b_1gu,
}
\tag{1.1}
\]

\[
\boxed{
\frac T{10}\le b_2<T,\qquad
\frac Y{10}\le b_3<Y.
}
\tag{1.2}
\]

循环方程是

\[
\boxed{
g(kq-1)=\frac{TY}{u}+q\frac Yv,
\qquad \gcd(k,10)=1.
}
\tag{1.3}
\]

因为 \(q,k\) 都为奇数，定义

\[
\boxed{
\lambda=\nu_2(kq-1)\ge1,\qquad
kq-1=2^\lambda\omega,\quad\omega\ \text{奇}.
}
\tag{1.4}
\]

E4 的四个循环状态原样为：

\[
\begin{array}{c|c|c}
\text{状态}&\text{参数位置}&\text{循环赋值}\\ \hline
\mathrm{G\!-\!A}&v=2,\ b_1=2,\ c=0&
n=a+\lambda+1\\
\mathrm{G\!-\!B}&v=1,\ c<m&
n=a+\lambda\\
\mathrm{G\!-\!C}&v=1,\ c=m&
a+\lambda=n+\eta\\
\mathrm{G\!-\!D}&v=1,\ c=m+j,\ j>0&
n=j+a+\lambda
\end{array}
\tag{1.5}
\]

其中

\[
\boxed{
\eta=\nu_2\!\left(5^{M-e}+q5^n\right)\ge1.
}
\tag{1.6}
\]

E4 的剩余室为：

\[
\begin{array}{c|l}
\mathrm{A1}&a\ge2,\ \lambda=1,\ n=a+2;\\
\mathrm{A2}&a\ge2,\ \lambda=2a-1,\ n=3a;\\
\mathrm{B},\ 0<c<m&
a\ge2,\ \lambda=1\text{ 或 }2a-1;\\
\mathrm{B},\ c=0,b_1=2&
\lambda=1\text{ 或 }2a;\\
\mathrm{B},\ c=0,b_1=1&
\text{保留 E4 的 }e_1,e_2,h_B,\varepsilon_B\text{ 精确系统};\\
\mathrm{C}&\mathrm{C1},\mathrm{C2},\mathrm{C3};\\
\mathrm{D1}&a\ge2,\ \lambda=1,\ n=j+a+1;\\
\mathrm{D2}&a\ge2,\ \lambda=2a-1,\ n=j+3a-1.
\end{array}
\tag{1.7}
\]

G–C 的三室为

\[
\boxed{
\begin{array}{c|l}
\mathrm{C1}&
\lambda<2\eta+1,\quad 2a>n,\quad a+\lambda=n+\eta;\\
\mathrm{C2}&
a\ge\eta+2,\quad\lambda=2a-1,\quad n=3a-1-\eta;\\
\mathrm{C3}&
a=\eta+1,\quad\lambda=2a-1,\quad n=2a,\quad\kappa=1.
\end{array}
}
\tag{1.8}
\]

所有高阶消去参数继续保留：

\[
\boxed{
\theta_A=
\nu_2\!\left(
99q^2\,5^e5^n-qg_0\,5^e
-2^{m+1}g_05^m
-2^{m+2}q5^M
\right),
}
\tag{1.9}
\]

\[
\boxed{
\theta_B=
\nu_2\!\left(
q5^e(99q5^n-g_0)
-2^{m-c}g_05^m
-2^{m-c+1}q5^M
\right).
}
\tag{1.10}
\]

参数 \(\kappa\ge1\) 仍表示 G–C 等号共振
\(\lambda=2\eta+1\) 时，把 \(\Gamma\) 的括号除去共同最低层后，
两个奇数主项之差的额外二进赋值。本文不会把
\(\eta,\theta_A,\theta_B,\kappa\) 中任何一个设为 \(1\)。

---

## 2. 终端商 \(\chi\)

### 2.0 阶段 I：终端商正规化

### 2.1 核心引理 GT-I.1：H1、H2、整数性与正性

定义

\[
\boxed{
\chi=gk-\frac Yv.
}
\tag{2.1}
\]

由于 \(v\in\{1,2\}\)、\(n\ge1\)，总有 \(Y/v\in\mathbb Z\)，所以
\(\chi\in\mathbb Z\)。由循环方程

\[
gkq-g=\frac{TY}{u}+q\frac Yv
\]

移项得到

\[
\boxed{
q\chi=g+\frac{TY}{u}.
}
\tag{2.2}
\]

右侧为正整数，故

\[
\boxed{\chi\in\mathbb Z_{>0}.}
\tag{2.3}
\]

再乘以 \(b_1u\)，并使用 (1.1)：

\[
b_1qu\chi=b_1gu+b_1TY,
\]

\[
\boxed{
vb_2\chi=b_1TY+b_3.
}
\tag{2.4}
\]

这就是 H2。它不是单纯的循环方程换写：其左侧含真实中分母块
\(b_2\)，右侧余项恰是有真实尾位窗口的 \(b_3\)，所以可以做整数端点分析。

此外，G 中 \(v\mid b_1\)：若 \(v=2\)，则 \(b_1=2\)；若 \(v=1\)
显然成立。因此定义

\[
\boxed{
E=\frac{b_1Y}{v}\in\mathbb Z_{>0},\qquad
R_3=\frac{b_3}{v}\in\mathbb Z_{>0}.
}
\tag{2.5}
\]

由 \(0<b_3<Y\) 得

\[
\boxed{0<R_3<E.}
\tag{2.6}
\]

式 (2.4) 因而正规化为

\[
\boxed{
b_2\chi=ET+R_3.
}
\tag{2.7}
\]

G–A 中 \(E=Y,\ R_3=b_3/2=gu\)，即

\[
b_2\chi=TY+\frac{b_3}{2}.
\]

G–B、C、D 中 \(v=1\)，故 \(E=b_1Y,\ R_3=b_3\)，即

\[
b_2\chi=b_1TY+b_3.
\]

这里没有出现非法的 \((b_1,v)=(1,2)\)：该组合已被 \(v\mid b_1\)
严格排除。

### 2.2 核心引理 GT-I.2：与 \(\lambda\) 的精确字典

由 (1.4) 和 (2.1)，有

\[
\boxed{
q\chi+q\frac Yv-g
=2^{a+\lambda}g_0\omega.
}
\tag{2.8}
\]

等价地，

\[
\boxed{
\frac{q\chi+qY/v-g}{2^{a+\lambda}}
=g_0\omega
\quad\text{为奇整数}.
}
\tag{2.9}
\]

所以不仅有一个模条件，而且有精确最低层：

\[
\boxed{
q\chi\equiv g-q\frac Yv
\pmod{2^{a+\lambda}},
}
\tag{2.10}
\]

并且该差除以 \(2^{a+\lambda}\) 后为奇数。

另一方面，由 (2.2)

\[
\boxed{
q\chi
=2^ag_0+2^{M-c}5^{M-e}.
}
\tag{2.11}
\]

式 (2.8) 把 \(\lambda\) 放入终端商，式 (2.11) 则直接决定
\(\nu_2(\chi)\)。二者联合等价地恢复循环最低层，而不是重新单列
E4 的仿射关系。

### 2.3 核心引理 GT-I.3：\(\chi\) 的精确二进赋值

因 \(q\) 为奇数，由 (2.11) 得：

\[
\boxed{
\nu_2(\chi)=a
\quad\text{在 G–A、G–B、G–D 中恒成立}.
}
\tag{2.12}
\]

证明如下。

- G–A：\(M>a\)；
- G–B：\(M-c>n=a+\lambda>a\)；
- G–D：
  \[
  M-c=n-j=a+\lambda>a.
  \]

G–C 中 \(M-c=n\)，所以

\[
q\chi=2^a g_0+2^n5^{M-e}.
\]

结合

\[
n-a=\lambda-\eta
\tag{2.13}
\]

得到完整三分支：

\[
\boxed{
\nu_2(\chi)=
\begin{cases}
a,&\lambda>\eta,\\
n,&\lambda<\eta,\\
a+\xi_C,&\lambda=\eta,
\end{cases}
}
\tag{2.14}
\]

其中等号室有 \(n=a\)，并定义真实高阶参数

\[
\boxed{
\xi_C=\nu_2\!\left(g_0+5^{M-e}\right)\ge1.
}
\tag{2.15}
\]

因此 C2、C3 中都因 \(\lambda>\eta\) 而满足

\[
\nu_2(\chi)=a;
\]

只有 C1 可以出现 (2.14) 的三个分支。

特别地，

\[
\boxed{\chi\ \text{总为正偶整数}.}
\tag{2.16}
\]

参数 \(\xi_C\) 不是对 E4 的替换；它只记录终端商在 C1 的
\(a=n\) 共振层中新增的奇数和消去。E4 原有的
\(\eta,\kappa\) 仍须同时保留。

---

### 2.4 阶段 II：整数窗口与二进端点

#### 核心引理 GT-II.1：统一下端与上端二分

由

\[
b_2\chi=ET+R_3,\qquad
\frac T{10}\le b_2<T,\qquad0<R_3<E
\]

首先得到严格下端：

\[
\boxed{E<\chi.}
\tag{3.1}
\]

事实上，若 \(\chi\le E\)，则

\[
b_2\chi\le b_2E<ET<ET+R_3,
\]

矛盾。

再按中分母是否命中下端分成两类。

若

\[
b_2>\frac T{10},
\]

则因 \(b_2,T/10\) 为整数，

\[
b_2\ge\frac T{10}+1.
\]

若再有 \(\chi\ge10E\)，则

\[
b_2\chi
\ge
\left(\frac T{10}+1\right)10E
=ET+10E
>ET+R_3,
\]

矛盾。因此

\[
\boxed{
b_2>\frac T{10}
\Longrightarrow
E<\chi<10E.
}
\tag{3.2}
\]

若

\[
b_2=\frac T{10},
\]

则 (2.7) 给出

\[
\boxed{
\chi=10E+\frac{10R_3}{T}>10E.
}
\tag{3.3}
\]

所以 \(\chi=E\) 与 \(\chi=10E\) 两个整数端点都不可能。
并且有精确等价：

\[
\boxed{
\chi<10E\iff b_2>T/10,
\qquad
\chi>10E\iff b_2=T/10.
}
\tag{3.4}
\]

这比单纯的比例带更强：越过上端恰好识别真实分母窗口的唯一整数端点。

#### 核心引理 GT-II.2：上端刚性、\(q=1\) 与精确 \(2,5\)-进

假设 \(\chi>10E\)。由 GT-II.1，

\[
b_2=\frac T{10}.
\]

令

\[
\delta_+=\chi-10E\in\mathbb Z_{>0}.
\]

由 (3.3)、(1.1) 得

\[
\delta_+
=\frac{R_3}{b_2}
=\frac{b_3/v}{b_1qu/v}
=\frac gq.
\]

所以 \(q\mid g\)。K5 有 \(\gcd(q,g)=1\)，因此

\[
\boxed{
q=1,\qquad \delta_+=g.
}
\tag{3.5}
\]

再由 \(b_2=T/10\)：

\[
\boxed{
T=\frac{10b_1u}{v},
\qquad
\chi=10E+g.
}
\tag{3.6}
\]

这是 G 中与 UB1 对应的上端刚性。与 O 不同，它只在部分室中产生矛盾。

把

\[
b_1=2^s,\qquad v=2^d,\qquad u=2^c5^e
\]

代入 (3.6)，精确比较 \(2\)-进和 \(5\)-进：

\[
\boxed{
m=1+s+c-d,\qquad m=1+e.
}
\tag{3.7}
\]

在 G–A 中

\[
s=d=1,\qquad c=0,
\]

故 (3.7) 给出 \(m=1\)，与 \(m\ge2\) 矛盾。因此

\[
\boxed{
\mathrm{G\!-\!A}:\quad Y<\chi<10Y.
}
\tag{3.8}
\]

在 \(v=1\) 中，(3.7) 化为

\[
\boxed{
e=m-1,\qquad c=m-1-s.
}
\tag{3.9}
\]

所以：

\[
\boxed{
\begin{array}{c|c|c}
b_1&s&\text{上端状态的必要且精确指数位置}\\ \hline
1&0&c=e=m-1;\\
2&1&c=m-2,\quad e=m-1.
\end{array}
}
\tag{3.10}
\]

这说明上端状态只能位于 G–B：

- \(b_1=1\) 时只能是 \(0<c<m\) 且 \(c=m-1\)；
- \(b_1=2\) 时，若 \(m\ge3\)，只能是 \(0<c<m\) 且 \(c=m-2\)；
- \(b_1=2,c=0\) 时只能有 \(m=2,e=1\)；
- \(b_1=1,c=0\) 会迫使 \(m=1\)，不可能；
- \(c=m\) 或 \(c>m\) 均不可能。

在上端状态中循环方程进一步退化为

\[
\boxed{
g(k-1)=(10b_1+1)Y,
}
\tag{3.11}
\]

故

\[
\boxed{
g\mid(10b_1+1)Y,\qquad
\lambda=n-a.
}
\tag{3.12}
\]

尾分母窗口则变为

\[
\boxed{
\frac YT\le g<\frac{10Y}{T}.
}
\tag{3.13}
\]

这些是上端状态的完整新算术数据；它们没有给 \(m,n,a\) 的绝对上界。

#### 核心引理 GT-II.3：有限终端商状态与非零余数

定义

\[
\boxed{
J=\left\lfloor\frac{\chi}{E}\right\rfloor,\qquad
\rho_J=\chi-JE.
}
\tag{3.14}
\]

另一方面，对 \(T\) 作关于真实中分母 \(b_2\) 的欧几里得除法：

\[
T=J_Tb_2+r_T,\qquad 0\le r_T<b_2.
\tag{3.15}
\]

代入 \(b_2\chi=ET+R_3\)：

\[
\chi=EJ_T+\frac{Er_T+R_3}{b_2}.
\]

由于

\[
0<Er_T+R_3
\le E(b_2-1)+R_3
<Eb_2,
\]

且最后的分数因 \(\chi,EJ_T\) 都是整数而必为整数，得到精确字典

\[
\boxed{
J=J_T=\left\lfloor\frac{T}{b_2}\right\rfloor,
\qquad
\rho_J=\frac{Er_T+R_3}{b_2}\in\{1,\ldots,E-1\}.
}
\tag{3.16}
\]

所以 \(J\) 不是任意人为切出的首位：它同时是 \(\chi/E\) 与
\(T/b_2\) 的共同欧几里得商，\(\rho_J\) 则记录尾块 \(R_3\)
对除法余数的精确修正。

若处于正常带 (3.2)，则

\[
\boxed{
J\in\{1,\ldots,9\},\qquad
0<\rho_J<E.
}
\tag{3.17}
\]

正常带中的精确余数恒等式为

\[
\boxed{
b_2\rho_J=E(T-Jb_2)+R_3.
}
\tag{3.18}
\]

若处于上端状态，则由 GT-II.2

\[
\chi=10E+g.
\]

又因 \(b_3=b_1gu<Y\)，有

\[
0<g<\frac{Y}{b_1u}<E.
\]

所以

\[
\boxed{
J=10,\qquad \rho_{10}=g.
}
\tag{3.19}
\]

因此全部 G 候选都被压入十个欧几里得终端商状态：

\[
\boxed{
J\in\{1,\ldots,10\},
}
\tag{3.20}
\]

其中 \(J=10\) 只允许 GT-II.2 的 G–B 刚性边界。

对靠近上端的正常状态，令

\[
\delta_-=10E-\chi>0.
\]

则

\[
\boxed{
b_2\delta_-=E(10b_2-T)-R_3,
}
\tag{3.21}
\]

并且 \(b_2>T/10\)。对靠近下端的状态，令

\[
\delta_0=\chi-E>0,
\]

则

\[
\boxed{
b_2\delta_0=E(T-b_2)+R_3.
}
\tag{3.22}
\]

所以两个邻近端点都保留了尾块余项 \(R_3\)；本文没有把 \(b_3\)
删去，也没有用纯大小关系代替整数余数。

---

## 3. G–A

### 3.1 核心引理 GT-III.1：A1、A2 的九状态化

G–A 中

\[
v=b_1=2,\qquad u=5^e,\qquad
E=Y,\qquad R_3=\frac{b_3}{2}=gu.
\]

GT-II.2 已排除上端状态，故

\[
\boxed{
Y<\chi<10Y.
}
\tag{4.1}
\]

于是 A1、A2 都唯一落入

\[
\boxed{
\chi=JY+\rho_J,\qquad
J\in\{1,\ldots,9\},\quad0<\rho_J<Y,
}
\tag{4.2}
\]

\[
\boxed{
b_2\rho_J=Y(T-Jb_2)+\frac{b_3}{2}.
}
\tag{4.3}
\]

两室分别为

\[
\begin{array}{c|c|c|c}
\text{室}&\lambda&n&\nu_2(\chi)=\nu_2(\rho_J)\\ \hline
\mathrm{A1}&1&a+2&a\\
\mathrm{A2}&2a-1&3a&a.
\end{array}
\tag{4.4}
\]

最后一列成立是因为

\[
\nu_2(JY)\ge n>a=\nu_2(\chi).
\]

所以余数的最低层恰由

\[
R_3=gu
\]

提供，而 \(Y(T-Jb_2)\) 的赋值更高。这与 H2 完全相容，没有新的矛盾。

A1 的高阶条件仍是

\[
a=2\Longrightarrow\theta_A=3,\qquad
a\ge3\Longrightarrow\theta_A=2.
\]

终端商状态没有控制 \(\theta_A\)，也没有限制无界的 \(a,m,e,q,g_0\)。
因此 A1、A2 的最终结果都是九个有限商状态，不是完整排除或参数上界。

---

## 4. G–B

### 4.1 正常九状态与唯一上端状态

G–B 中

\[
v=1,\qquad E=b_1Y,\qquad R_3=b_3,\qquad n=a+\lambda>a.
\]

正常状态为

\[
\boxed{
\chi=Jb_1Y+\rho_J,\qquad
J\in\{1,\ldots,9\},\quad0<\rho_J<b_1Y,
}
\tag{5.1}
\]

\[
\boxed{
b_2\rho_J=b_1Y(T-Jb_2)+b_3,
\qquad
\nu_2(\rho_J)=a.
}
\tag{5.2}
\]

若出现 \(J=10\)，则完整刚性数据是

\[
\boxed{
q=1,\quad b_2=T/10,\quad
T=10b_1u,\quad
\chi=10b_1Y+g,
}
\tag{5.3}
\]

\[
\boxed{
e=m-1,\qquad c=m-1-\nu_2(b_1),
}
\tag{5.4}
\]

\[
\boxed{
g(k-1)=(10b_1+1)Y,\qquad
\rho_{10}=g,\qquad \nu_2(\rho_{10})=a.
}
\tag{5.5}
\]

逐子室得到：

\[
\boxed{
\begin{array}{c|c}
\text{G--B 子室}&\text{终端商结果}\\ \hline
0<c<m,\ b_1=1&
J=1,\ldots,9;\ \text{或 }J=10,\ c=e=m-1;\\
0<c<m,\ b_1=2&
J=1,\ldots,9;\ \text{或 }J=10,\ c=m-2,\ e=m-1,\ m\ge3;\\
c=0,\ b_1=2&
J=1,\ldots,9;\ \text{或 }J=10,\ m=2,\ e=1;\\
c=0,\ b_1=1&
J=1,\ldots,9\ \text{且无上端状态}.
\end{array}
}
\tag{5.6}
\]

最后一格等价地写成：

\[
\boxed{
c=0,\ b_1=1\Longrightarrow J\in\{1,\ldots,9\}.
}
\tag{5.7}
\]

E4 在 \(0<c<m\) 中的
\[
\lambda=1\quad\text{或}\quad2a-1,
\]
在 \(c=0,b_1=2\) 中的
\[
\lambda=1\quad\text{或}\quad2a,
\]
以及 \(c=0,b_1=1\) 的 \(e_1,e_2,h_B,\varepsilon_B\) 共振系统，
都没有被终端商删除。参数 \(\theta_B\) 也必须原样保留。

### 4.2 上端状态的无界辅助族

上端状态不是空的前置形式。对任意

\[
n\ge3
\]

取

\[
\boxed{
\begin{gathered}
m=2,\quad T=100,\quad Y=10^n,\\
b_1=2,\quad v=1,\quad q=1,\quad u=5,\quad c=0,\\
g=6\cdot10^{n-2},\quad
a=n-1,\quad g_0=3\cdot5^{n-2},\\
k=351.
\end{gathered}
}
\tag{5.8}
\]

则

\[
b_2=10=\frac T{10},\qquad
b_3=6\cdot10^{n-1},
\]

满足两个真实分母窗口，并且

\[
g(k-1)=21Y=\frac{TY}{u}+Y.
\]

此外

\[
\lambda=\nu_2(350)=1,\qquad
n=a+1,
\]

\[
\chi=gk-Y=20Y+g,
\]

所以它恰落在 G–B、\(c=0,b_1=2\)、\(J=10\) 状态。
K5 支撑也成立：

\[
u\mid TY,\qquad
\operatorname{rad}(u)=5\mid g,\qquad
\gcd(q,g)=1.
\]

高阶参数不是任意略去的。把 (5.8) 代入 (1.10)：

\[
\boxed{
\theta_B
=\nu_2\!\left(7060\cdot5^{n-2}\right)
=2,
}
\tag{5.9}
\]

正好命中 E4 对 \(a\ge2,\lambda=1,c=0,b_1=2\) 的要求。

还可取真实分子块

\[
\boxed{
(a_1,a_2,a_3)=(5,1,Y+1).
}
\tag{5.10}
\]

它们满足三个分子窗口和逐项既约。对应

\[
\Gamma=1412Y^2>0.
\]

三个 \(W\) 的最低层逐例为：

\[
\begin{array}{c|c}
n&(\nu_2(W_{12}),\nu_2(W_{13}),\nu_2(W_{23}))\\ \hline
3&(6,4,7)\\
4&(8,8,5)\\
n\ge5&(2n,n+2,n+1).
\end{array}
\tag{5.11}
\]

所以对全部 \(n\ge3\)

\[
\nu_2(W_{12}^2+W_{13}^2+W_{23}^2)
=2n+2
=\nu_2(\Gamma).
\tag{5.12}
\]

这是一族满足真实十进制定义、循环方程、分母与分子窗口、逐项既约、
K5 支撑、\(\theta_B\) 及 E4 三平方赋值门的辅助数据。
本文不声称它满足完整等式

\[
t^2\Gamma=W_{12}^2+W_{13}^2+W_{23}^2,
\]

所以它不是原题解。它严格证明：终端商端点、E4 高阶二进门和真实窗口的
联合不能排除 G–B 的 \(J=10\) 状态，也不能给 \(n\) 上界。

---

## 5. G–C

### 5.1 核心引理 GT-III.2：C1、C2、C3 的九状态化

G–C 中

\[
v=1,\qquad c=m,\qquad
E=b_1Y,\qquad R_3=b_3.
\]

若出现 \(J=10\)，GT-II.2 会强迫

\[
c=m-1-\nu_2(b_1)<m,
\]

与 \(c=m\) 矛盾。因此 C1、C2、C3 均只有正常状态：

\[
\boxed{
\chi=Jb_1Y+\rho_J,\qquad
J\in\{1,\ldots,9\},\qquad
0<\rho_J<b_1Y,
}
\tag{6.1}
\]

\[
\boxed{
b_2\rho_J=b_1Y(T-Jb_2)+b_3.
}
\tag{6.2}
\]

终端商的精确赋值由

\[
n-a=\lambda-\eta
\]

决定：

\[
\boxed{
\nu_2(\chi)=
\begin{cases}
a,&\lambda>\eta,\\
n,&\lambda<\eta,\\
a+\xi_C,&\lambda=\eta.
\end{cases}
}
\tag{6.3}
\]

特别地，

\[
\boxed{
\mathrm{C2},\mathrm{C3}:\quad
\nu_2(\chi)=a.
}
\tag{6.4}
\]

为了不在 C1 中遗漏 \(\chi\) 与 \(Jb_1Y\) 的第二次高阶消去，令

\[
h_\chi=\nu_2(\chi),\qquad
h_J=n+\nu_2(b_1J).
\]

则

\[
\boxed{
\nu_2(\rho_J)=
\begin{cases}
\min(h_\chi,h_J),&h_\chi\ne h_J,\\
h_\chi+\zeta_{C,J},&h_\chi=h_J,
\end{cases}
}
\tag{6.5}
\]

其中等号室的

\[
\zeta_{C,J}\ge1
\]

定义为两个归一化奇数之差的真实额外赋值。式 (6.5) 是精确恒等式，
不是把高阶消去假定为 \(1\)。

因此：

- C1 被压成九个 \(J\) 状态，但仍保留
  \(\eta,\xi_C,\zeta_{C,J}\)；
- C2 被压成九个 \(J\) 状态，仍保留无界的 \(a,\eta,m\)；
- C3 被压成九个 \(J\) 状态，且仍须保留 \(\kappa=1\) 的完整来源，
  不能把它从 Gram 共振中删去。

终端商没有给 \(\eta\) 或 \(\kappa\) 上界，也没有关闭 C1、C2、C3。

---

## 6. G–D

### 6.1 核心引理 GT-III.3：D1、D2 的九状态化

G–D 中

\[
v=1,\qquad c=m+j>m,\qquad
E=b_1Y,\qquad R_3=b_3.
\]

上端状态会强迫 \(c=m-1-s<m\)，故不可能。因此

\[
\boxed{
\chi=Jb_1Y+\rho_J,\qquad
J\in\{1,\ldots,9\},\quad
0<\rho_J<b_1Y,
}
\tag{7.1}
\]

\[
\boxed{
b_2\rho_J=b_1Y(T-Jb_2)+b_3.
}
\tag{7.2}
\]

D1、D2 分别满足

\[
\begin{array}{c|c|c|c}
\text{室}&\lambda&n&\nu_2(\chi)=\nu_2(\rho_J)\\ \hline
\mathrm{D1}&1&j+a+1&a\\
\mathrm{D2}&2a-1&j+3a-1&a.
\end{array}
\tag{7.3}
\]

因为 \(n>a\)，有

\[
\nu_2(Jb_1Y)>a,
\]

故余数赋值确为 \(a\)。但 \(j,m,a\) 仍可无界；终端商只给九个
离散商状态。

## 7. 整数端点与赋值

### 7.1 全部剩余室的端点—状态表

\[
\boxed{
\begin{array}{c|c|c|c}
\text{E4 剩余室}&E&J\text{ 状态}&J=10\text{ 的可能性}\\ \hline
\mathrm{A1}&Y&1,\ldots,9&\text{不可能}\\
\mathrm{A2}&Y&1,\ldots,9&\text{不可能}\\
\mathrm{B},\ 0<c<m&b_1Y&1,\ldots,10&
\begin{array}{l}
b_1=1:\ c=e=m-1\\
b_1=2:\ c=m-2,\ e=m-1
\end{array}\\
\mathrm{B},\ c=0,b_1=2&2Y&1,\ldots,10&
m=2,\ e=1\\
\mathrm{B},\ c=0,b_1=1&Y&1,\ldots,9&\text{不可能}\\
\mathrm{C1}&b_1Y&1,\ldots,9&\text{不可能}\\
\mathrm{C2}&b_1Y&1,\ldots,9&\text{不可能}\\
\mathrm{C3}&b_1Y&1,\ldots,9&\text{不可能}\\
\mathrm{D1}&b_1Y&1,\ldots,9&\text{不可能}\\
\mathrm{D2}&b_1Y&1,\ldots,9&\text{不可能}
\end{array}
}
\tag{7.4}
\]

所有正常状态都有

\[
0<\rho_J<E,\qquad
b_2\rho_J=E(T-Jb_2)+R_3.
\]

所有 \(J=10\) 状态都有

\[
q=1,\quad b_2=T/10,\quad
\rho_{10}=g,\quad
g(k-1)=(10b_1+1)Y.
\]

这就是 G 的完整有限终端商状态化。

---

## 8. 主动反例攻击

### 8.1 \(\chi\) 是否一定为整数

是。\(v\in\{1,2\}\) 且 \(Y=10^n\)，所以 \(Y/v\in\mathbb Z\)。
式 (2.2) 又证明 \(q\chi\) 为正整数；定义本身已给
\(\chi\in\mathbb Z\)。

### 8.2 \(Y/v\) 是否一定为整数

是。唯一非平凡情形 \(v=2\) 中 \(n\ge1\)，故 \(2\mid Y\)。

### 8.3 是否把 \(b_1/v\) 非法当作整数

没有。G 正规化先给 \(v\mid b_1\)。当 \(v=2\) 时必有 \(b_1=2\)；
\((b_1,v)=(1,2)\) 根本不属于候选空间。

### 8.4 是否复制 O 中“终端商为奇数”的结论

没有。G 中

\[
\nu_2(\chi)\ge1,
\]

所以 \(\chi\) 总为偶数。A、B、D 的赋值恰为 \(a\)，C 的精确例外见
(2.14)。

### 8.5 是否遗漏 \(b_3\) 余项

没有。全文使用

\[
R_3=b_3/v,\qquad0<R_3<E,
\]

并在 (3.18)、(3.21)、(3.22) 中保留它。正是 \(0<R_3<E\)
排除了所有整数倍端点。

### 8.6 窗口严格端点是否写对

是。真实窗口是

\[
T/10\le b_2<T.
\]

下端允许等号，而上端严格。结果是：

- \(b_2>T/10\) 对应 \(E<\chi<10E\)；
- \(b_2=T/10\) 对应 \(\chi=10E+g\)；
- \(\chi=E\) 与 \(\chi=10E\) 都不可能。

### 8.7 是否忘记 E4 高阶参数

没有。A1 继续保留 \(\theta_A\)，B 继续保留 \(\theta_B\) 及
\(e_1,e_2,h_B,\varepsilon_B\)，C 继续保留 \(\eta,\kappa\)。
终端商的 C1 等号室还新增了不可任意固定的 \(\xi_C,\zeta_{C,J}\)。

### 8.8 是否用有限搜索支持无界结论

没有。所有带状、端点与有限状态结论都由整数恒等式证明。
第 5.2 节是对全部 \(n\ge3\) 的显式无限辅助族，不是有限样本。

### 8.9 辅助族是否满足真实十进制定义

是。第 5.2 节逐项满足：

\[
b_2=10\in[T/10,T),\qquad
b_3=6\cdot10^{n-1}\in[Y/10,Y),
\]

\[
a_2=1\in[10^{m-2},10^{m-1}),\qquad
a_3=Y+1\in[Y,10Y),
\]

以及三个逐项既约条件、真实 \(U=TY/u\)、\(V=Y/v\)、循环方程和
K5 支撑。它明确只承担“现有终端商与 E4 门不能关闭该状态”的反例功能，
没有被表述为原题解。

---

## 9. 最终分类 GT1–GT6

本轮达到

\[
\boxed{
\mathrm{GT4}:\quad
\text{G 的全部 E4 剩余室被压成有限终端商状态}.
}
\]

这里的有限对象是

\[
(\text{E4 室},J),\qquad J\in\{1,\ldots,10\},
\]

并附带：

- \(J\le9\) 时的非零余数恒等式 (3.18)；
- \(J=10\) 时的刚性系统 (3.5)–(3.13)。

为什么不是 GT1：

- G–A、B、C、D 都仍有开放室。

为什么不是 GT2：

- 本轮没有关闭 E4 的任一完整剩余赋值室；
- 只排除了各室中的上端状态，或把它压到显式 B 边界。

为什么不是 GT3：

- 没有得到 \(a,m,n,\eta,j\) 或任何高阶消去参数的统一绝对上界；
- 第 5.2 节给出 \(n\) 无界的端点辅助族。

为什么达到 GT4：

- 所有十个题设指定室都只有九个正常商状态；
- 其中三个 B 子室至多再有一个 \(J=10\) 状态；
- \(J=10\) 不是模糊的“附近情形”，而是
  \[
  q=1,\ b_2=T/10,\ T=10b_1u,\ \rho_{10}=g
  \]
  的完整整数端点系统。

为什么不是 GT5：

- 终端商机制没有整体失效；它确实完成了全 G 的有限商状态化；
- 但第 5.2 节证明它单独不能继续关闭 B 的上端状态。

为什么高于 GT6：

- 结果不只是局部比例窗；
- 它给出覆盖全部 E4 剩余室的有限欧几里得状态、非零余数恒等式和
  唯一上端刚性分类。

需要特别强调：

\[
\boxed{
\mathrm{GT4}\ \text{不等于 }\chi\text{ 的取值有限，也不等于 G 已有限参数化}.
}
\]

每个 \(J\) 状态内，\(\rho_J,E,Y\) 仍可随 \(n\) 增长。

---

## 10. 临界层最新状态

在本轮约定的研究边界内，临界层 \(N_L=1\) 的状态更新为：

1. \(2\mid r\)：已关闭；
2. O：UB1 已关闭 \(10Y<c<11Y\) 上端带；本轮不返回其余 O 区域；
3. Q：保持 CKD–E4 的无界移动系数系统，本轮未研究；
4. G：E4 的 A、B、C、D 室全部完成终端商有限状态化：
   \[
   J=1,\ldots,9,
   \]
   并只在 G–B 保留刚性
   \[
   J=10
   \]
   边界。

G 的下一层完整候选仍须同时满足：

\[
\text{终端商状态}
+\text{E4 全部高阶门}
+\text{真实分子窗口}
+\text{逐项既约}
+\text{完整 Gram 等式}
+\text{双拼接主方程}.
\]

终端商状态没有替代这些门。当前最小停止点是

\[
\boxed{
\begin{gathered}
\text{G 已从无界的 }\chi\text{ 比例问题压成有限 }J\text{ 状态；}\\
\text{唯一越过十进制上端的状态是 G--B 的 }q=1\text{ 边界；}\\
\text{该边界存在通过全部现有前置门的无界辅助族；}\\
\text{因此本轮止于 GT4，不宣称 G 已关闭或参数已统一有界。}
\end{gathered}
}
\]

全文停止；不研究 O、Q，不等待“继续”。
