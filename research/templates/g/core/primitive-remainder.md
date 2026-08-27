# 三项十进制拼接平方和问题：临界 \(G\) 模板本原正余数报告

## 1. VA1、GD1 后的 \(G\) 剩余系统

本文只研究临界层

\[
(\delta _2,\delta _3)=(-1,1),\qquad N_L=1
\]

中的偶边模板

\[
\mathrm G:\qquad 2\mid g.
\]

按任务约定，本文暂时接受 T1–T18、K5、CG、E4、GT4、GB2、VA1
和 GD1，不作整个项目的统一独立审计。VA1 已关闭 \(J=10\)，GD1
已关闭

\[
T-Jb_2=0.
\]

所以本文的起始系统恰为

\[
\boxed{
J\in\{1,\ldots ,9\},\qquad
T=Jb_2+r,\qquad 1\le r<b_2,
}
\tag{1.1}
\]

\[
\boxed{
qu\rho=Yr+gu,\qquad
0<\rho<E:=\frac{b_1Y}{v}.
}
\tag{1.2}
\]

这里

\[
T=10^m,\qquad Y=10^n,\qquad m\ge2,\quad n\ge1,
\tag{1.3}
\]

\[
g=2^a5^\varphi g_0,\qquad
q=5^fq_0,\qquad
\gcd(q_0g_0,10)=1,
\tag{1.4}
\]

\[
a\ge1,\qquad
u=2^c5^e,\qquad
v\in\{1,2\},\qquad
v\mid b_1,\qquad
\gcd(u,v)=1,
\tag{1.5}
\]

\[
\boxed{
b_2=\frac{b_1qu}{v},\qquad
b_3=b_1gu,
}
\tag{1.6}
\]

\[
\boxed{
\frac T{10}\le b_2<T,\qquad
\frac Y{10}\le b_3<Y.
}
\tag{1.7}
\]

K5 的条件

\[
\gcd(q,g)=1,\qquad
u\mid TY,\qquad
\operatorname{rad}(u)\mid qg
\tag{1.8}
\]

始终保留。特别地，

\[
f>0\Longrightarrow\varphi=0.
\tag{1.9}
\]

本文严格使用三个阶段，每阶段至多三个核心新引理：

- 阶段 I：GP-I.1–GP-I.3，\(\tau\) 与内容的精确正规化；
- 阶段 II：GP-II.1–GP-II.3，本原行列式、五进关闭与二进饱和界；
- 阶段 III：GP-III.1–GP-III.2，完整判别式与反例攻击。

最终达到的分类是

\[
\boxed{\mathrm{GP3}.}
\tag{1.10}
\]

准确含义是：题设第 6.2 节的整个

\[
\boxed{5\mid q}
\]

五进饱和分支无解。其余正余数状态得到本原内容正规形和精确
\(\tau\)-类型，但没有关闭整个 \(G\)，也没有把剩余参数压成有限集合。

---

## 2. \(\tau\)-正规化

### 2.1 核心引理 GP-I.1：本原欧几里得除法

定义

\[
\boxed{\tau=\gcd(T,b_2).}
\tag{2.1}
\]

因为 \(r=T-Jb_2\)，有 \(\tau\mid r\)。因此存在唯一正整数
\(N,B,s\) 使

\[
\boxed{
T=\tau N,\qquad b_2=\tau B,\qquad r=\tau s.
}
\tag{2.2}
\]

代入 \(T=Jb_2+r\)，得到

\[
\boxed{
N=JB+s,\qquad1\le s<B.
}
\tag{2.3}
\]

由 \(\tau=\gcd(T,b_2)\)，

\[
\gcd(N,B)=1.
\]

再由 \(s=N-JB\)，

\[
\boxed{
\gcd(N,B)=\gcd(s,B)=1.
}
\tag{2.4}
\]

GT4 的正常余数恒等式为

\[
b_2\rho=Er+\frac{b_3}{v}.
\tag{2.5}
\]

这里 \(b_3/v\) 确为整数，因为 \(v\mid b_1\) 且
\(b_3=b_1gu\)。代入 (2.2)：

\[
\tau B\rho=\tau Es+\frac{b_3}{v}.
\]

所以

\[
\boxed{\tau\mid\frac{b_3}{v}.}
\tag{2.6}
\]

定义

\[
\boxed{
D=\frac{b_3}{v\tau}\in\mathbb Z_{>0}.
}
\tag{2.7}
\]

约去 \(\tau\) 得到主方程

\[
\boxed{
B\rho-Es=D.
}
\tag{2.8}
\]

由 \(b_3<Y\) 及 \(E=b_1Y/v\)，

\[
1\le D
<\frac{Y}{v\tau}
\le\frac{E}{\tau}.
\]

故

\[
\boxed{
1\le D<\frac E\tau,\qquad \tau<E.
}
\tag{2.9}
\]

真实尾窗还给出比题设要求更精确的带：

\[
\boxed{
\frac{E}{10b_1\tau}\le D<
\frac{E}{b_1\tau}.
}
\tag{2.10}
\]

最后，

\[
\boxed{
\frac{\rho}{E}-\frac{s}{B}
=\frac{D}{BE}>0.
}
\tag{2.11}
\]

所以 \((s/B,\rho/E)\) 是同一欧几里得单元内的有序有理点，
而不是两个独立余数。

### 2.2 核心引理 GP-I.2：内容因子

由定义，

\[
gB
=g\frac{b_2}{\tau}
=q\frac{b_3}{v\tau}
=qD.
\tag{2.12}
\]

结合 \(\gcd(q,g)=1\)，得到

\[
q\mid B,\qquad g\mid D.
\]

因此存在唯一正整数 \(h\) 使

\[
\boxed{
B=qh,\qquad D=gh.
}
\tag{2.13}
\]

直接与 (1.6) 比较，

\[
\boxed{
h=\frac{b_1u}{v\tau}\in\mathbb Z_{>0},
\qquad
\tau h=\frac{b_1u}{v}.
}
\tag{2.14}
\]

这是 (2.6) 与 \(\gcd(q,g)=1\) 联合后的强化：不仅
\(\tau\mid b_3/v\)，而且

\[
\boxed{\tau\mid\frac{b_1u}{v}.}
\tag{2.15}
\]

把 (2.13) 代入 (2.8)：

\[
h(q\rho-g)=Es.
\]

由 \(\gcd(s,B)=1\) 及 \(h\mid B\)，有 \(\gcd(s,h)=1\)，故

\[
\boxed{h\mid E.}
\tag{2.16}
\]

定义

\[
\boxed{
F=\frac Eh=\frac{\tau Y}{u}\in\mathbb Z_{>0}.
}
\tag{2.17}
\]

于是全部正余数状态统一化为

\[
\boxed{
\begin{aligned}
&B=qh,\qquad D=gh,\qquad E=hF,\\
&N=Jqh+s,\qquad1\le s<qh,\qquad\gcd(s,qh)=1,\\
&q\rho-Fs=g,\qquad0<\rho<hF.
\end{aligned}
}
\tag{2.18}
\]

特别地，若某个正整数同时整除 \(q,F\)，由最后一式它也整除
\(g\)。结合 \(\gcd(q,g)=1\)，

\[
\boxed{\gcd(q,F)=1.}
\tag{2.19}
\]

原始正间隙变为

\[
\boxed{
\frac{\rho}{hF}-\frac{s}{qh}
=\frac{g}{qhF}>0.
}
\tag{2.20}
\]

这里 \(h\) 是单元内容。真正的本原单元是 \(h=1\)，而不是把
\(h=1\) 无条件强加到全部候选。

### 2.3 核心引理 GP-I.3：\(\tau\) 的精确 \(2,5\)-进类型

为避免与余数 \(s\) 重名，记

\[
\sigma=v_2(b_1)\in\{0,1\},\qquad d=v_2(v)\in\{0,1\}.
\]

令

\[
x=\sigma+c-d,\qquad y=e+f.
\tag{2.21}
\]

因为 \(q\) 为奇数，

\[
\boxed{
v_2(\tau)=\alpha:=\min(m,x)
=\min\!\left(m,v_2(b_1)+c-v_2(v)\right).
}
\tag{2.22}
\]

因为 \(b_1/v\) 没有因子 \(5\)，

\[
\boxed{
v_5(\tau)=\beta:=\min(m,e+f).
}
\tag{2.23}
\]

而

\[
v_2\!\left(\frac{b_3}{v}\right)=a+x,\qquad
v_5\!\left(\frac{b_3}{v}\right)=e+\varphi.
\tag{2.24}
\]

式 (2.6) 因而等价于

\[
\alpha\le a+x,\qquad \beta\le e+\varphi.
\tag{2.25}
\]

二进不等式自动成立；五进不等式在 \(f>0\) 时产生真正限制。
此时 (1.9) 给 \(\varphi=0\)，所以

\[
\min(m,e+f)\le e.
\]

若 \(e+f<m\)，左边为 \(e+f>e\)，矛盾；否则左边为 \(m\)，
从而

\[
\boxed{
5\mid q\Longrightarrow e\ge m.
}
\tag{2.26}
\]

这正是题设的 T6，并且证明中不可缺少地使用了
\(\gcd(q,g)=1\) 以推出 \(\varphi=0\)。

由 (2.14)、(2.17)，内容指数和本原竖尺度为

\[
\boxed{
h=2^{x-\alpha}5^{e-\beta},
}
\tag{2.27}
\]

\[
\boxed{
v_2(F)=\alpha+n-c,\qquad
v_5(F)=\beta+n-e.
}
\tag{2.28}
\]

这些指数均非负。另一方面

\[
\boxed{
N=2^{m-\alpha}5^{m-\beta}.
}
\tag{2.29}
\]

所以 \(\tau\)-状态不再是任意赋值组合，而是由有限个
\((x-\alpha,e-\beta)\) 类型控制。

---

## 3. 本原欧几里得单元

### 3.1 阶段 II 核心引理 GP-II.1：本原核心与有限内容提升

题设优先要求的核心条件

\[
\tau=\frac{b_1u}{v}
\tag{3.1}
\]

与

\[
h=1
\]

完全等价。此时 (2.18) 化为

\[
\boxed{
B=q,\qquad D=g,\qquad E=F,
}
\tag{3.2}
\]

\[
\boxed{
N=Jq+s,\qquad
1\le s<q,\qquad
\gcd(s,q)=1,
}
\tag{3.3}
\]

\[
\boxed{
q\rho-Es=g,\qquad0<\rho<E.
}
\tag{3.4}
\]

从而

\[
\boxed{
Es\equiv-g\pmod q,\qquad
q\rho\equiv g\pmod E,
}
\tag{3.5}
\]

\[
\boxed{
\frac{\rho}{E}-\frac{s}{q}
=\frac{g}{qE}>0.
}
\tag{3.6}
\]

先验地

\[
\gcd(q,E)
=5^{\min(f,n)}
\]

只能是 \(5\)-幂。但 (3.4) 说明任何 \(\gcd(q,E)\) 都整除
\(g\)，故再由 \(\gcd(q,g)=1\) 得

\[
\boxed{\gcd(q,E)=1,\qquad5\nmid q.}
\tag{3.7}
\]

因此 \(s\) 在 \(1,\ldots ,q-1\) 中至多有一个可能值，
\(\rho\) 在 \(1,\ldots ,E-1\) 中也至多有一个可能值。若存在，

\[
s\equiv-gE^{-1}\pmod q,\qquad
\rho=\frac{Es+g}{q}.
\tag{3.8}
\]

特别地 \(q=1\) 与 \(1\le s<q\) 矛盾，所以本原正余数核心中
\(q\ge3\)。

当 \(h>1\) 时，行列式仍是同一个本原方程

\[
q\rho-Fs=g,
\tag{3.9}
\]

但 \((s,\rho)\) 位于 \(h\) 倍矩形

\[
0<s<qh,\qquad0<\rho<hF.
\]

由于 (3.9) 的任意两个整数解之差为

\[
(s,\rho)\longmapsto(s+\ell q,\rho+\ell F),
\]

该矩形内至多有 \(h\) 个提升。因 \(h\) 本身仍可无界，这不是
GP4 意义下的有限状态集。

行列式为 \(g\)，一般并非 \(1\)。所以 (3.6) 不是 Farey 相邻关系，
也不能把 \(g>1\) 擅自降为单位面积。

---

## 4. 五进饱和分支

### 4.1 核心引理 GP-II.2：\(5\mid q\) 整体无解

假设

\[
5\mid q,\qquad f\ge1.
\]

由 (2.26)，

\[
e\ge m,\qquad \beta=v_5(\tau)=m.
\tag{4.1}
\]

由 \(\gcd(q,F)=1\)，而 \(5\mid q\)，必须

\[
v_5(F)=0.
\]

利用 (2.28)，

\[
0=\beta+n-e=m+n-e,
\]

故

\[
\boxed{e=m+n.}
\tag{4.2}
\]

另一方面 \(\gcd(q,g)=1\) 给 \(\varphi=0\)。于是

\[
5\mid u,\qquad
\operatorname{rad}(u)\mid qg
\]

在素数 \(5\) 处由 \(5\mid q\) 完整承担；G 模板已有
\(2\mid g\)，所以 K5 支撑门也已逐素数核对。该支撑门不会允许
因子 \(5\) 同时转移到 \(g\)，因为这会违反 \(\gcd(q,g)=1\)。
现在

\[
v_5(b_2)=e+f=m+n+f,
\]

\[
v_5(b_3)=e+\varphi=m+n.
\]

因此

\[
b_2b_3
\ge5^{\,2(m+n)+f}
>5^{\,2(m+n)}
>2^{m+n}5^{m+n}
=TY.
\tag{4.3}
\]

但两个严格上窗给出

\[
b_2b_3<TY,
\tag{4.4}
\]

矛盾。所以

\[
\boxed{
5\mid q\Longrightarrow\text{无正余数候选}.
}
\tag{4.5}
\]

该关闭同时覆盖 E4 的 A、B、C、D 全部室，不依赖固定 \(r\)、
固定 \(J\) 或有限搜索。

从此以后所有剩余候选都满足

\[
\boxed{\gcd(q,10)=1.}
\tag{4.6}
\]

再由 K5 支撑门，

\[
e>0\Longrightarrow5\mid g.
\tag{4.7}
\]

需要区分：本文关闭的是题设第 6.2 节的 \(q\)-驱动五进饱和支
\(5\mid q\)。在 \(5\nmid q\) 中，仍可有 \(e\ge m\) 和
\(v_5(\tau)=m\)；这些是 \(u\)-自身的五进饱和，未被 (4.5)
误报为已关闭。

### 4.2 剩余五进类型

由 (4.6) 有 \(f=0\)。结合 \(0\le e\le m+n\)，全部剩余
五进类型恰为

\[
\boxed{
\begin{array}{c|c|c|c}
\text{类型}&\beta=v_5(\tau)&v_5(h)&v_5(F)\\ \hline
\mathrm{F_-}:0\le e<m&e&0&n\\
\mathrm{F_0}:e=m&m&0&n\\
\mathrm{F_+}:m<e\le m+n&m&e-m&m+n-e
\end{array}}
\tag{4.8}
\]

所以 \(u\)-自身的五进溢出量

\[
\ell=e-m
\]

若为正，必满足统一有效界

\[
\boxed{1\le\ell\le n.}
\tag{4.9}
\]

---

## 5. 二进饱和分支

### 5.1 核心引理 GP-II.3：精确室表与统一指数关系

二进饱和指

\[
v_2(\tau)=m.
\tag{5.1}
\]

由 (2.22)，这等价于 \(x=\sigma+c-d\ge m\)。E4 四个位置逐格
给出：

\[
\boxed{
\begin{array}{c|c|c|c|c}
\text{E4 位置}&(b_1,v,c)&\alpha&v_2(h)&v_2(F)\\ \hline
\mathrm A&(2,2,0)&0&0&n\\
\mathrm B&(1,1,c<m)&c&0&n\\
\mathrm B&(2,1,0\le c\le m-2)&c+1&0&n+1\\
\mathrm B_{\rm sat}&(2,1,m-1)&m&0&n+1\\
\mathrm C_1&(1,1,m)&m&0&n\\
\mathrm C_2&(2,1,m)&m&1&n\\
\mathrm D_1&(1,1,m+j)&m&j&n-j\\
\mathrm D_2&(2,1,m+j)&m&j+1&n-j
\end{array}}
\tag{5.2}
\]

表中的 \(\mathrm C_1,\mathrm C_2\) 只区分 \(b_1=1,2\)，不要与
E4 的 C1、C2、C3 共振室编号混淆。

所以真正二进饱和的 E4 位置恰为：

1. \(b_1=2,v=1,c=m-1\) 的 B 边界；
2. \(c=m\) 的全部 C 室；
3. \(c=m+j>m\) 的全部 D 室。

A 室及其余 B 室二进不饱和。

在任何二进饱和状态中，

\[
b_3=b_1gu
=2^{\sigma+a+c}5^{e+\varphi}g_0
\ge2^{a+m}.
\]

由 \(b_3<Y=10^n\)，得到

\[
\boxed{
m+a<n\log_2 10,
}
\tag{5.3}
\]

即

\[
\boxed{
m\le\left\lceil n\log_2 10\right\rceil-a-1.
}
\tag{5.4}
\]

这比单用 \(\tau<E\) 得到的

\[
m<n\log_2 10+1
\]

更强。它是统一有效指数关系，但不是 \(m<n+O(1)\)；纯二进大小
比较自然产生系数 \(\log_2 10\)。

对 D 室还可使用

\[
c=m+j,\qquad n=j+a+\lambda
\]

精化。此时

\[
\sigma+a+c=m+n-\lambda+\sigma,
\]

故

\[
\boxed{
m<\lambda-\sigma+n\log_2 5.
}
\tag{5.5}
\]

这些关系没有给 \(m,n,a,j\) 的绝对上界，也没有与 A、B、C、D
的仿射关系产生统一矛盾。因此本文不声称关闭整个二进饱和分支。

---

## 6. E4 各室与 \(\tau\)-类型

### 6.1 继承的 E4 室原样保留

令

\[
\lambda=v_2(kq-1)\ge1,\qquad M=m+n.
\tag{6.1}
\]

四个循环位置为

\[
\boxed{
\begin{array}{c|c|c}
\text{位置}&\text{定义}&\text{循环赋值}\\ \hline
\mathrm A&v=2,\ b_1=2,\ c=0&n=a+\lambda+1\\
\mathrm B&v=1,\ c<m&n=a+\lambda\\
\mathrm C&v=1,\ c=m&a+\lambda=n+\eta\\
\mathrm D&v=1,\ c=m+j,\ j>0&n=j+a+\lambda
\end{array}}
\tag{6.2}
\]

其中

\[
\boxed{
\eta=v_2(5^{M-e}+q5^n)\ge1.
}
\tag{6.3}
\]

E4 的剩余室为

\[
\boxed{
\begin{array}{c|l}
\mathrm{A1}&a\ge2,\ \lambda=1,\ n=a+2;\\
\mathrm{A2}&a\ge2,\ \lambda=2a-1,\ n=3a;\\
\mathrm B,\ 0<c<m&
a\ge2,\ \lambda=1\text{ 或 }2a-1;\\
\mathrm B,\ c=0,b_1=2&
\lambda=1\text{ 或 }2a;\\
\mathrm B,\ c=0,b_1=1&
\text{保留 }e_1,e_2,h_B,\varepsilon_B\text{ 的精确系统};\\
\mathrm C&\mathrm{C1},\mathrm{C2},\mathrm{C3};\\
\mathrm{D1}&a\ge2,\ \lambda=1,\ n=j+a+1;\\
\mathrm{D2}&a\ge2,\ \lambda=2a-1,\ n=j+3a-1.
\end{array}}
\tag{6.4}
\]

C 的三个共振室原样为

\[
\boxed{
\begin{array}{c|l}
\mathrm{C1}&
\lambda<2\eta+1,\quad2a>n,\quad a+\lambda=n+\eta;\\
\mathrm{C2}&
a\ge\eta+2,\quad\lambda=2a-1,\quad n=3a-1-\eta;\\
\mathrm{C3}&
a=\eta+1,\quad\lambda=2a-1,\quad n=2a,\quad\kappa=1.
\end{array}}
\tag{6.5}
\]

其中 \(\kappa\) 仍是 \(\lambda=2\eta+1\) 时 Gram 最低层两个奇主项
之差的真实额外二进赋值，不能被固定为 \(1\)，除非进入 E4 已证明的
C3 室。

A1、B 的高阶参数继续定义为

\[
\boxed{
\theta_A=
v_2\!\left(
99q^2\,5^e5^n-qg_0\,5^e
-2^{m+1}g_05^m
-2^{m+2}q5^M
\right),
}
\tag{6.6}
\]

\[
\boxed{
\theta_B=
v_2\!\left(
q5^e(99q5^n-g_0)
-2^{m-c}g_05^m
-2^{m-c+1}q5^M
\right).
}
\tag{6.7}
\]

特别地，

\[
\mathrm{A1}:\quad
a=2\Rightarrow\theta_A=3,\qquad
a\ge3\Rightarrow\theta_A=2.
\tag{6.8}
\]

在 \(0<c<m,\lambda=1\) 中继续保留：

\[
\begin{array}{c|c}
a=2,\ c=m-1&\theta_B=2\\
a=2,\ c\le m-2&\text{精确共振门}\\
a\ge3,\ c=m-1&\theta_B=3\\
a\ge3,\ c\le m-2&\theta_B=2.
\end{array}
\tag{6.9}
\]

在 \(c=0,b_1=2\) 中，

\[
\lambda=1\Rightarrow
\theta_B=
\begin{cases}
1,&a=1,\\
2,&a\ge2,
\end{cases}
\qquad
\lambda>1\Rightarrow\lambda=2a.
\tag{6.10}
\]

对唯一未完全线性化的 \(c=0,b_1=1\) 室，令
\(e_i=v_2(a_i)\)。当 \(\lambda>1\) 时保留

\[
\begin{aligned}
v_2(W_{12})
&=a+v_2(2^{M+e_2}\!\cdot\mathrm{odd}
-2^{n+1+e_1}\!\cdot\mathrm{odd}),\\
v_2(W_{13})
&=v_2(2^M\!\cdot\mathrm{odd}
-2^{2a+e_1}\!\cdot\mathrm{odd}),\\
v_2(W_{23})
&=v_2(2^{n+1}\!\cdot\mathrm{odd}
-2^{2a+e_2}\!\cdot\mathrm{odd}),
\end{aligned}
\tag{6.11}
\]

并以 \(h_B\) 表示三者最小值、以
\(\varepsilon_B\in\{0,1\}\) 表示最小项个数造成的平方和修正：

\[
\boxed{
2a+\lambda+1=2h_B+\varepsilon_B.
}
\tag{6.12}
\]

当 \(\lambda=1\) 时保留

\[
\boxed{
2(a+1)+\theta_B=2h_B+\varepsilon_B.
}
\tag{6.13}
\]

GT4 在 C1 中新增的 \(\xi_C,\zeta_{C,J}\) 也不被本报告删除；
它们仍分别记录 \(\lambda=\eta\) 及
\(\chi\) 与 \(Jb_1Y\) 同赋值时的二次高阶消去。

### 6.2 有限精确 \(\tau\)-类型

二进表 (5.2) 与五进表 (4.8) 的笛卡尔组合，给出至多

\[
\boxed{8\times3=24}
\]

个精确内容类型。每一类型中的
\(\alpha,\beta,v_2(h),v_5(h),v_2(F),v_5(F)\) 均由表中公式唯一给出，
不再保留任意赋值组合。

特别地，

\[
\boxed{
\tau=\frac{b_1u}{v}
}
\]

恰发生在：

1. A 的全部状态；
2. B 的全部状态；
3. C 中 \(b_1=1\) 的状态；
4. 同时满足 \(e\le m\)。

这里已经使用 \(5\mid q\) 分支被关闭，所以 \(f=0\)。

二进溢出只发生在 C 的 \(b_1=2\) 行与 D；五进溢出只发生在
\(\mathrm F_+\) 的 \(e>m\) 行。没有一个仍存活的饱和室仅凭
\(\tau<E\) 自动矛盾；真正被窗口关闭的是第 4 节的
\(5\mid q\) 整个分支。

---

## 7. 完整球面—拼接判别式

### 7.1 核心引理 GP-III.1：单元坐标下的完整判别式

完整 G 球面与分子拼接为

\[
\boxed{
(gua_1)^2+(gva_2)^2+a_3^2=t^2,
}
\tag{7.1}
\]

\[
\boxed{
Y(a_1T+10a_2)+a_3=kt.
}
\tag{7.2}
\]

令

\[
\mathcal S=g^2\bigl((ua_1)^2+(va_2)^2\bigr),
\qquad
H=a_1T+10a_2.
\tag{7.3}
\]

消去 \(t\)，得到

\[
(k^2-1)a_3^2-2YH\,a_3+k^2\mathcal S-Y^2H^2=0.
\tag{7.4}
\]

因此

\[
\boxed{
\mathcal D=Y^2H^2-(k^2-1)\mathcal S
}
\tag{7.5}
\]

必须满足

\[
\boxed{\mathcal D=w^2,\qquad w\in\mathbb Z_{\ge0},}
\tag{7.6}
\]

\[
\boxed{
a_3=\frac{YH\pm kw}{k^2-1}
\in\mathbb Z_{>0},
}
\tag{7.7}
\]

以及

\[
Y\le a_3<10Y,\qquad
\gcd(a_3,b_3)=1.
\tag{7.8}
\]

同时仍须保留

\[
(a_1,b_1)\in
\{(1,1),\ldots,(8,1)\}
\cup\{(5,2),(7,2),(9,2),(11,2),(13,2)\},
\tag{7.8a}
\]

\[
10^{m-2}\le a_2<10^{m-1},\qquad
\gcd(a_2,b_2)=1.
\tag{7.8b}
\]

现在代入本原单元。由

\[
\chi=gk-\frac Yv=JhF+\rho
\]

定义

\[
\boxed{
K_0:=gk=\frac Yv+JhF+\rho.
}
\tag{7.9}
\]

又

\[
T=\tau N=\tau(Jqh+s).
\tag{7.10}
\]

因此判别式精确化为

\[
\boxed{
\mathcal D
=Y^2\bigl(a_1\tau(Jqh+s)+10a_2\bigr)^2
-(K_0^2-g^2)
\bigl((ua_1)^2+(va_2)^2\bigr).
}
\tag{7.11}
\]

等价地，作为 \(a_1,a_2\) 的二次型，

\[
\boxed{
\begin{aligned}
\mathcal D={}&
\bigl(Y^2T^2-(K_0^2-g^2)u^2\bigr)a_1^2\\
&+20Y^2T\,a_1a_2\\
&+\bigl(100Y^2-(K_0^2-g^2)v^2\bigr)a_2^2.
\end{aligned}}
\tag{7.12}
\]

式 (7.11)–(7.12) 保留了 \(J,\tau\)-类型、正行列式
\(q\rho-Fs=g\)、球面和分子拼接的全部耦合，没有把判别式平方误写成
充分条件。

### 7.2 核心引理 GP-III.2：固定低模与符号攻击的停止点

因为 \(k\) 为奇数，

\[
v_2(k^2-1)\ge3.
\]

又 \(a=v_2(g)\ge1\)，所以

\[
v_2((k^2-1)\mathcal S)\ge5.
\]

而 \(Y^2H^2\) 至少被 \(2^{2n+2}\) 整除，\(n\ge1\)。故

\[
\boxed{\mathcal D\equiv0\pmod{16}.}
\tag{7.13}
\]

因此模 \(4\)、模 \(8\) 对整个正余数系统都是自动平方类，不能关闭
任何完整 E4 室。奇素数模数仍依赖移动的
\((q,g,h,F,a_1,a_2)\)，没有从继承系统中出现一个固定的统一
二次非剩余类。

判别式也不在某个 \((J,\tau\text{-类型})\) 上统一为负。继承的
G–A 辅助数据

\[
\begin{gathered}
m=2,\quad n=4,\quad
b_1=v=2,\quad q=3,\quad g=100,\quad u=5,\quad k=717,\\
b_2=15,\quad b_3=1000
\end{gathered}
\tag{7.14}
\]

满足真实分母窗口、K5 支撑、循环方程和 E4 的 A1 高阶门
\(\theta_A=3\)。其正余数单元为

\[
\boxed{
J=6,\ r=10,\ \tau=5,\ N=20,\ B=3,\ s=2,
}
\tag{7.15}
\]

\[
\boxed{
E=F=10000,\quad
\rho=6700,\quad D=g=100,\quad h=1,
}
\tag{7.16}
\]

且

\[
3\cdot6700-10000\cdot2=100.
\]

取合法首、中分子块

\[
a_1=5,\qquad a_2=1,
\]

则

\[
\boxed{
\mathcal D=22776386480000>0.
}
\tag{7.17}
\]

所以不能用 \(\mathcal D<0\) 关闭 A1 或全部本原核心。该具体值满足

\[
\mathcal D\equiv2\pmod3,
\]

故不是平方；若改取同一分母状态中的 \(a_2=2\)，则
\(\mathcal D\equiv0\pmod3\)。这也说明模 \(3\) 的非剩余证书不是
同一 \((J,\tau)\) 状态上的统一门。

该辅助数据不是原题解：它正是在完整平方判别式处失败。它只承担
反驳“正行列式会自动给出统一负判别式或固定模障碍”的功能。

---

## 8. 新定理与主动反例攻击

### 8.1 本轮新定理

本轮得到以下覆盖全部正余数状态的新结构。

1. **欧几里得正规形**
   \[
   T=\tau N,\quad b_2=\tau B,\quad r=\tau s,\quad
   N=JB+s,\quad\gcd(s,B)=1.
   \]
2. **内容分解**
   \[
   B=qh,\quad D=gh,\quad E=hF,\quad
   q\rho-Fs=g,\quad\gcd(q,F)=1.
   \]
3. **有限精确赋值型**
   所有存活状态落入第 4、5、6 节的有限
   \((v_2(h),v_5(h),v_2(F),v_5(F))\) 类型。
4. **完整分支关闭**
   \[
   \boxed{5\mid q\text{ 整体无解}.}
   \]
5. **二进饱和统一界**
   \[
   m+a<n\log_2 10,
   \]
   D 室还有 (5.5) 的精化。

### 8.2 十项反例攻击

1. **\(\tau\) 是否整除 \(r\)：**  
   是，因为 \(r=T-Jb_2\) 且 \(\tau\mid T,b_2\)。

2. **是否正确推出 \(\gcd(s,B)=1\)：**  
   是，
   \[
   \gcd(s,B)=\gcd(N-JB,B)=\gcd(N,B)=1.
   \]

3. **\(b_3/v\) 是否为整数：**  
   是，因为 \(v\mid b_1\)。

4. **是否把 \(\tau\mid b_3/v\) 错强为 \(b_2\mid b_3/v\)：**  
   没有。数据 (7.14) 中
   \[
   \tau=5\mid500=b_3/v,
   \qquad15=b_2\nmid500.
   \]

5. **\(5\mid q\) 时是否使用 \(\gcd(q,g)=1\)：**  
   是。它先给 \(\varphi=0\)，再给 T6；随后
   \(\gcd(q,F)=1\) 才迫使 \(e=m+n\)。

6. **是否把 \(h=1\) 当成全部状态：**  
   没有。C 的 \(b_1=2\)、D 和 \(e>m\) 都产生显式非平凡内容。

7. **是否把正行列式误写成单位行列式：**  
   没有。一般原始行列式为 \(D=gh\)，本原行列式仍为 \(g\)，
   数据 (7.14) 中 \(D=g=100\)。

8. **是否错误调用 Farey 相邻理论：**  
   没有。只有行列式 \(1\) 才是标准相邻情形；本文保留 \(g>1\)。

9. **是否在无界参数未控制时有限搜索：**  
   没有。本轮的分支关闭完全由整除、赋值和窗口乘积完成。
   (7.14) 只是显式反例攻击，不承担全局证明。

10. **辅助数据是否满足真实门：**  
    (7.14) 满足真实十进制分母窗、K5 支撑、循环方程、正余数条件
    和 E4 的 A1 高阶门；它明确在判别式平方处失败，没有冒充原题解。

---

## 9. 最终分类 GP1–GP6

本轮达到

\[
\boxed{
\mathrm{GP3}:
\quad
\text{题设第 6.2 节的全部 }5\mid q
\text{ 五进饱和状态关闭}.
}
\tag{9.1}
\]

决定性链条是

\[
\boxed{
\begin{gathered}
B\rho-Es=D,\quad gB=qD,\quad\gcd(q,g)=1\\
\Longrightarrow
B=qh,\ D=gh,\ E=hF,\ \gcd(q,F)=1;\\
5\mid q
\Longrightarrow
\varphi=0,\ e\ge m,\ v_5(F)=0
\Longrightarrow e=m+n;\\
e=m+n
\Longrightarrow
b_2b_3>TY,
\end{gathered}}
\tag{9.2}
\]

与真实窗口 \(b_2b_3<TY\) 矛盾。

为什么不是 GP1：

- A、B、C、D 中仍有 \(5\nmid q\) 的正余数开放状态。

为什么不是 GP2：

- 本轮关闭的是横跨各 E4 室的完整 \(5\mid q\) 分支，没有关闭 A、B、
  C 或 D 中的整个一室。

为什么这里的 GP3 不应误读：

- 已关闭的是题设专门命名的 \(5\mid q,\ e\ge m\) 五进饱和分支；
- \(5\nmid q\) 时仍允许 \(e\ge m\)，即
  \(u\)-自身造成的 \(v_5(\tau)=m\)。

为什么不是 GP4：

- 虽然 \(\tau\)-类型有限，内容 \(h\)、指数 \(m,n,a,e\) 仍可无界；
- 每个内容层至多 \(h\) 个提升，不是统一有限个本原单元点。

为什么高于 GP5：

- 除了本原缺陷结构，还严格关闭了一个完整无界分支。

没有找到合法原题解。

---

## 10. \(G\) 模板最新状态

结合 VA1、GD1 与本轮 GP3，临界 \(G\) 的最新剩余系统为

\[
\boxed{
\begin{gathered}
J\in\{1,\ldots,9\},\qquad
T=\tau(Jqh+s),\\
1\le s<qh,\qquad
\gcd(s,qh)=1,\\
\gcd(q,10)=1,\qquad
q\rho-Fs=g,\\
0<\rho<hF,\qquad
\gcd(q,F)=1,\\
h=\frac{b_1u}{v\tau},\qquad
F=\frac{\tau Y}{u},\qquad
E=hF.
\end{gathered}}
\tag{10.1}
\]

它还必须同时满足：

1. 第 6 节原样保留的 E4 A、B、C、D 室及
   \(\lambda,\eta,\theta_A,\theta_B,\kappa\) 和全部高阶消去门；
2. 真实分母窗口和十三种首块；
3. 真实分子窗口与三个逐项既约条件；
4. 完整判别式 (7.5)–(7.8)。

本原核心恰为

\[
\boxed{
h=1:
\quad
\tau=\frac{b_1u}{v},\quad
B=q,\quad D=g,\quad
q\rho-Es=g.
}
\tag{10.2}
\]

非本原状态则是同一行列式在 \(h\) 倍矩形中的至多 \(h\) 个提升。
当前尚未控制

\[
\boxed{
h,\ m,\ n,\ a,\ e,\ q,\ g_0,
\quad\text{以及按室出现的 }\eta,j,e_2
\text{和高阶消去参数}.
}
\tag{10.3}
\]

因此本轮的准确停止点是：

\[
\boxed{
\begin{gathered}
G\text{ 的正余数层已获得真正的本原内容—行列式正规形};\\
5\mid q\text{ 的完整无界分支已由窗口乘积关闭};\\
二进饱和层得到统一有效指数关系，但仍开放};\\
完整球面—拼接判别式没有产生统一符号或固定低模关闭};\\
\text{故最终分类为 GP3，而不是整个 }G\text{ 无解}.
\end{gathered}}
\]

全文到此停止；不研究 O、Q，不返回 \(J=10\) 或 \(r=0\)。
