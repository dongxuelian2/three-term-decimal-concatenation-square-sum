# 三项十进制拼接平方和问题：临界 G 模板 A2 低 \(\varphi\) 浅深度负根报告

日期：2026-08-06（Asia/Tokyo）

本文严格研究

\[
\boxed{
G_{\mathrm{prim}},\qquad
\gamma=1,\qquad
\mathrm{A2},\qquad
a\ge3,\qquad
1\le\varphi<a,
}
\]

中的浅深度负根区域

\[
\boxed{
\mathcal L_{\mathrm{sh},-}:
\quad
\sigma=-1,
\qquad
2\varphi\ge3(a-\varphi).
}
\tag{0.1}
\]

接受 PR6、SD6、GA2-6、GE2-1、GAL-2 与 GALS\((+)\)-3 中相容的
完整终端系统；不研究浅正根、真正深区、高 \(\varphi\) 的
\(\mathcal F_{P-}\)、B、C、\(\gamma>1\)、非本原 C2/C5、Q 或严格层。

本轮得到以下严格结论。

1. 模 \(\Lambda\) 的负根 Möbius involution 完全退化为标准仿射反射
   \(\tau\mapsto\langle\theta-\tau\rangle_\Lambda\)，并分成两个互斥
   进位室；逐位 Hensel 树完全消失。
2. 唯一固定点违反精确负根门。全部通过五进根门的状态组成非平凡
   二循环；终端奇偶门可在一个二循环中保留零端、一端或两端，本文给出
   精确判别和两个反射室的精确计数公式。
3. 全部局部量均成为 \((a,\Delta,J,\tau)\) 的闭式整数；第一次二进下降
   把仿射参数唯一写成 \(y=Mz-A_\tau\)，并得到正缺陷正规形
   \[
   2^\delta10^\mu=zr-\mathcal D_\tau.
   \]
4. 每个固定 \((a,\Delta,h,J,\tau)\) 的全部指数至多是一条
   \(\operatorname{ord}_r(10)\)-同余类；严格大小门将其截成一条完整
   有限同余段，每个指数唯一恢复 \(z,y,q,s,N,L\)。
5. 共轭和差给出 \(q=r\) 不可能、\(v_2(q+r)=1\)、
   \(v_5(q+r)=0\)、\(v_5(q-r)=2\varphi\) 及
   \(v_2(q-r)\ge2a+1\)，但 \(q-r\) 的符号不能仅由进位室统一决定。
6. 第二 Bezout 坐标给出两个固定行列式 \(2\)、精确 gcd 字典和模
   \(M^2\) 的高位消去；然而它严格恒等于第一次下降，没有形成独立
   关闭门。
7. \(\kappa=0\) 仍是一条无界射线；二进、五进同层消去均有完整字典，
   但没有统一矛盾、平方分解或绝对参数边界。

因此准确分类为

\[
\boxed{
\mathrm{GALS(-)\text{-}3}:
\quad
\text{involution 完全仿射化，得到双坐标下降和每状态唯一有限指数段，}
\text{但仍有无界残余。}
}
\tag{0.2}
\]

没有找到合法原题六元组，也没有发现 GALS\((+)\)-3、GAL-2、GE2-1、
GA2-6、PR6 或 SD6 的继承错误。

---

## 1. 参数、浅深度恒等式与负根数据

定义

\[
\boxed{\Delta=a-\varphi\ge1.}
\tag{1.1}
\]

浅深度条件等价于

\[
2(a-\Delta)\ge3\Delta
\iff
5\Delta\le2a
\iff
\boxed{1\le\Delta\le\left\lfloor\frac{2a}{5}\right\rfloor.}
\tag{1.2}
\]

置

\[
\boxed{
M=2^{2a},\qquad
C=5^{2\varphi},\qquad
\Lambda=5^{3\Delta},\qquad
B=MC.
}
\tag{1.3}
\]

再定义

\[
\boxed{
\kappa=2\varphi-3\Delta=2a-5\Delta\ge0,
\qquad
K=M5^\kappa.
}
\tag{1.4}
\]

因为 \(\kappa+3\Delta=2\varphi\)，严格得到

\[
\boxed{
C=\Lambda5^\kappa,
\qquad
B=K\Lambda.
}
\tag{1.5}
\]

尾窗为

\[
h\in\mathcal H(a),
\qquad
e=2a+\Delta+h.
\tag{1.6}
\]

记

\[
\boxed{\delta=\Delta+h,\qquad e=2a+\delta.}
\tag{1.7}
\]

负根低二进 Bezout 数据为

\[
\boxed{x=\left\langle2C^{-1}\right\rangle_M,}
\tag{1.8}
\]

\[
\boxed{Cx=2+Mc,}
\tag{1.9}
\]

\[
\boxed{
\rho=Cx-1=1+Mc,
\qquad
\eta=cx.
}
\tag{1.10}
\]

GAL-2 已给出并可直接复核

\[
0<x<M,qquad0<c<C,qquad0<\rho<B,
\tag{1.11}
\]

\[
\boxed{\rho^2=1+B\eta.}
\tag{1.12}
\]

由于 \(C=\Lambda5^\kappa\)，还有

\[
\boxed{\rho=\Lambda5^\kappa x-1,}
\tag{1.13}
\]

从而

\[
\rho\equiv-1\pmod\Lambda,
\qquad
\rho^2\equiv1\pmod\Lambda.
\tag{1.14}
\]

全部真实局部状态必须满足

\[
\boxed{
0\le\tau<\Lambda,
\qquad
x+M\tau\equiv2\text{ 或 }3\pmod5,
}
\tag{1.15}
\]

\[
\boxed{
c+J+\tau\equiv1\pmod2,
\qquad
J\in\{1,\ldots,9\}.
}
\tag{1.16}
\]

本文不会从 (1.15) 擅自推出 \(\tau\ne0\)：负根中 \(\tau=0\) 可以通过
精确根门，必须保留。

---

## 2. Möbius involution 的严格仿射退化

GAL-2 的负根 involution 为

\[
\lambda_\tau
=
\left\langle
-(\eta+\rho\tau)(\rho+B\tau)^{-1}
\right\rangle_\Lambda.
\tag{2.1}
\]

由 \(\Lambda\mid B\)，

\[
\rho+B\tau\equiv\rho\pmod\Lambda.
\]

又因 \(\rho^2\equiv1\pmod\Lambda\)，\(\rho\) 是模 \(\Lambda\) 的单位，且

\[
\boxed{\rho^{-1}\equiv\rho\pmod\Lambda.}
\tag{2.2}
\]

定义唯一标准平移数字

\[
\boxed{
\theta
=
\left\langle-\eta\rho^{-1}\right\rangle_\Lambda
=
\left\langle-\eta\rho\right\rangle_\Lambda.
}
\tag{2.3}
\]

由 \(\rho\equiv-1\pmod\Lambda\)，

\[
-\eta\rho\equiv\eta\pmod\Lambda,
\]

所以

\[
\boxed{\theta=\langle\eta\rangle_\Lambda.}
\tag{2.4}
\]

将 (2.2)–(2.4) 代回 (2.1)，得到模同余

\[
\lambda_\tau\equiv\theta-\tau\pmod\Lambda.
\]

因为 \(0\le\lambda_\tau<\Lambda\)，严格的双向标准代表公式是

\[
\boxed{
\lambda_\tau=\left\langle\theta-\tau\right\rangle_\Lambda.
}
\tag{2.5}
\]

反向地，(2.5) 直接满足 (2.1) 的定义同余，因此没有放宽 GAL-2 的
Möbius 图。

定义唯一进位位 \(\epsilon_\tau\in\{0,1\}\)，使

\[
\boxed{
\tau+\lambda_\tau
=
\theta+\epsilon_\tau\Lambda.
}
\tag{2.6}
\]

两个互斥反射室为

\[
\boxed{
0\le\tau\le\theta
\Longrightarrow
\epsilon_\tau=0,
\quad
\lambda_\tau=\theta-\tau,
}
\tag{2.7a}
\]

\[
\boxed{
\theta<\tau<\Lambda
\Longrightarrow
\epsilon_\tau=1,
\quad
\lambda_\tau=\theta+\Lambda-\tau.
}
\tag{2.7b}
\]

式 (2.7a) 完整保留 \(\theta=0\)、\(\tau=0\)、\(\tau=\theta\)、
\(\lambda_\tau=0\) 与 \(\epsilon_\tau=0\) 的端点。

反射保持两个室：若 \(\epsilon_\tau=0\)，则
\(\tau+\lambda_\tau=\theta\)，两端均不超过 \(\theta\)；若
\(\epsilon_\tau=1\)，则两端均严格大于 \(\theta\)。因此
\(\epsilon_\lambda=\epsilon_\tau\)。

这已经完全消除 GAL-2 的逐位 Hensel 输出数字。外层仍有
\(\Lambda\) 个标准代表，不能把“无 Hensel 树”误写成叶节点数绝对有界。

---

## 3. 固定点、根门、二循环与精确状态计数

由 \(Mc=Cx-2\) 及 \(\eta=cx\)，模 \(\Lambda\) 有

\[
M\eta=M(cx)\equiv-2x\pmod\Lambda.
\]

结合 \(\theta\equiv\eta\pmod\Lambda\)，得到

\[
\boxed{
\theta\equiv-2xM^{-1}\pmod\Lambda.
}
\tag{3.1}
\]

固定点满足 \(2\tau\equiv\theta\pmod\Lambda\)。因为 \(\Lambda\) 为奇数，
固定点唯一，且其标准代表为

\[
\boxed{
\tau_*
=
\left\langle-xM^{-1}\right\rangle_\Lambda.
}
\tag{3.2}
\]

由 (3.2)，

\[
\boxed{x+M\tau_*\equiv0\pmod\Lambda.}
\tag{3.3}
\]

特别地 \(x+M\tau_*\equiv0\pmod5\)，违反 (1.15)。所以唯一固定点被
精确负根门严格删除。

### 3.1 反射保持精确根门

由 (2.5) 与 (3.1)，

\[
\begin{aligned}
x+M\lambda_\tau
&\equiv x+M(\theta-\tau)\\
&\equiv-(x+M\tau)\pmod\Lambda.
\end{aligned}
\]

因此

\[
\boxed{
x+M\lambda_\tau
\equiv-(x+M\tau)\pmod\Lambda.
}
\tag{3.4}
\]

模 5 时，\(2\) 与 \(3\) 互为相反数，所以 (1.15) 在反射下严格保持，
且两个合法首位数字互换。联合固定点删除，得到

\[
\boxed{
\text{全部通过精确负根门的状态组成唯一的非平凡二循环。}
}
\tag{3.5}
\]

根门本身恰有

\[
2\cdot5^{3\Delta-1}
\]

个有向状态，故有 \(5^{3\Delta-1}\) 个二循环。

### 3.2 奇偶门在二循环中的零、一、二端判别

对同一二循环，(2.6) 给

\[
\tau+\lambda_\tau\equiv\theta+\epsilon_\tau\pmod2.
\tag{3.6}
\]

若 \(\theta+\epsilon_\tau\) 为奇数，二循环两端奇偶相反，所以固定 \(J\)
的门 (1.16) 恰保留一个有向端点。

若 \(\theta+\epsilon_\tau\) 为偶数，二循环两端奇偶相同，所以 (1.16)
或者同时保留两端，或者同时删除两端。准确地，

\[
\boxed{
\begin{array}{c|c}
\theta+\epsilon_\tau\pmod2&\text{二循环通过 (1.16) 的端数}\\ \hline
1&1\\
0&2\text{ 或 }0
\end{array}}
\tag{3.7}
\]

因此不能从固定点被删除跳到“每个二循环自动通过奇偶门”。

### 3.3 两个反射室的精确合法状态数

令 \(d\in\{2,3\}\)，定义模 5 标准根数字

\[
\alpha_d
=
\left\langle M^{-1}(d-x)\right\rangle_5
\in\{0,1,2,3,4\}.
\tag{3.8}
\]

对固定 \(J\)，置

\[
p_J=\langle1-c-J\rangle_2.
\tag{3.9}
\]

再令 \(\beta_{d,J}\in\{0,\ldots,9\}\) 是唯一满足

\[
\beta_{d,J}\equiv\alpha_d\pmod5,
\qquad
\beta_{d,J}\equiv p_J\pmod2
\tag{3.10}
\]

的标准代表。显式地，若 \(\alpha_d\equiv p_J\pmod2\)，则
\(\beta_{d,J}=\alpha_d\)；否则 \(\beta_{d,J}=\alpha_d+5\)。

定义整数计数函数

\[
F(T;\beta)=
\begin{cases}
0,&T<\beta,\\[1mm]
\left\lfloor\dfrac{T-\beta}{10}\right\rfloor+1,&T\ge\beta.
\end{cases}
\tag{3.11}
\]

则两个进位室中同时通过根门和奇偶门的有向状态数准确为

\[
\boxed{
\mathcal N_0(a,\Delta,J)
=
\sum_{d\in\{2,3\}}F(\theta;\beta_{d,J}),
}
\tag{3.12}
\]

\[
\boxed{
\mathcal N_1(a,\Delta,J)
=
\sum_{d\in\{2,3\}}
\left{
F(\Lambda-1;\beta_{d,J})-F(\theta;\beta_{d,J})
\right}.
}
\tag{3.13}
\]

这里 \(\mathcal N_0\) 对应 \(0\le\tau\le\theta\)，
\(\mathcal N_1\) 对应 \(\theta<\tau<\Lambda\)。两个 \(d\) 给出不同的
模 5 类，因此没有重复计数；固定点不通过根门，也无需额外减一。

式 (3.12)–(3.13) 是精确闭式，而不是遍历长度 \(\Lambda\) 的列表。它们也
显示叶节点数一般仍按 \(\Lambda\) 增长。

---

## 4. 两个基础高位数字与一个附加平移量

由 (2.4)，\(\eta-\theta\) 被 \(\Lambda\) 整除。定义

\[
\boxed{
g=\frac{\eta-\theta}{\Lambda}\in\mathbb Z_{\ge0}.
}
\tag{4.1}
\]

再定义

\[
\boxed{
s_*=\frac{\eta+\rho\theta}{\Lambda}.
}
\tag{4.2}
\]

使用 \(\eta=\theta+\Lambda g\) 与
\(\rho=\Lambda5^\kappa x-1\)，得到

\[
\begin{aligned}
\eta+\rho\theta
&=\theta+\Lambda g+(\Lambda5^\kappa x-1)\theta\\
&=\Lambda(g+5^\kappa x\theta).
\end{aligned}
\]

所以

\[
\boxed{s_*=g+5^\kappa x\theta.}
\tag{4.3}
\]

因为 \(\eta>0\)、\(\rho>0\)、\(\theta\ge0\)，(4.2) 的分子为正，故

\[
\boxed{s_*\in\mathbb Z_{\ge1}.}
\tag{4.4}
\]

定义第二个基础数字

\[
\boxed{
t_*=\frac{2x+M\theta}{\Lambda}.
}
\tag{4.5}
\]

式 (3.1) 保证分子被 \(\Lambda\) 整除；分子严格为正，故

\[
t_*\in\mathbb Z_{>0}.
\tag{4.6}
\]

由 \(Cx=2+Mc\) 乘以 \(x\)，

\[
Cx^2=2x+M\eta.
\]

代入 \(C=\Lambda5^\kappa\)、\(\eta=\theta+\Lambda g\)，再除以
\(\Lambda\)，得到第二个基础 Bezout 恒等式

\[
\boxed{
5^\kappa x^2=t_*+Mg.
}
\tag{4.7}
\]

奇偶方面，\(x\) 是 \(2\) 乘以奇数的模 \(M\) 标准代表，故 \(x\) 为偶数。
于是 \(\eta=cx\) 为偶数。由
\(\eta=\theta+\Lambda g\) 且 \(\Lambda\) 为奇数，

\[
g\equiv\theta\pmod2.
\]

式 (4.3) 的第二项为偶数，所以

\[
\boxed{s_*\equiv\theta\pmod2.}
\tag{4.8}
\]

后文还需要一个由相同数据决定的正平移量

\[
\boxed{
\Xi=\Lambda s_*-\theta.
}
\tag{4.9}
\]

由 \(s_*\ge1\)、\(0\le\theta<\Lambda\)，有 \(\Xi\ge1\)。再由
\(\Lambda s_*=\eta+\rho\theta\)、\(\rho-1=Mc\)，

\[
\boxed{
\Xi
=
\eta+(\rho-1)\theta
=
c(x+M\theta)>0.
}
\tag{4.10}
\]

量 \(g,s_*,t_*,\Xi\) 都只依赖 \((a,\Delta)\)，不依赖
\((h,J,\tau)\)。

---

## 5. 全部局部状态的闭式与双向复核

定义

\[
\boxed{V=J\Lambda+\tau,}
\tag{5.1}
\]

\[
\boxed{r=\rho+BV.}
\tag{5.2}
\]

GAL-2 的内层标准量为

\[
s_0
=
\frac{\eta+\rho(\tau+\lambda_\tau)+B\tau\lambda_\tau}{\Lambda}.
\]

使用 (2.6)、(4.2) 与 \(B=K\Lambda\)，得到

\[
\boxed{
s_0
=
s_*+\rho\epsilon_\tau+K\tau\lambda_\tau.
}
\tag{5.3}
\]

定义

\[
\boxed{q_0=\rho+B\lambda_\tau.}
\tag{5.4}
\]

由 \(N_0=Jq_0+s_0\)，

\[
\begin{aligned}
N_0
&=\rho(J+\epsilon_\tau)+s_*
  +JB\lambda_\tau+K\tau\lambda_\tau\\
&=\rho(J+\epsilon_\tau)+s_*
  +K(J\Lambda+\tau)\lambda_\tau.
\end{aligned}
\]

因此

\[
\boxed{
N_0
=
\rho(J+\epsilon_\tau)+s_*+KV\lambda_\tau.
}
\tag{5.5}
\]

### 5.1 终端乘积的独立复核

由 (5.2)、(5.4)，

\[
\begin{aligned}
q_0r-1
&=(\rho+B\lambda_\tau)(\rho+BV)-1\\
&=(\rho^2-1)+B\rho(V+\lambda_\tau)+B^2V\lambda_\tau\\
&=B\{\eta+\rho(V+\lambda_\tau)+BV\lambda_\tau\}.
\end{aligned}
\]

由 \(V=J\Lambda+\tau\) 和内层定义，花括号恰为 \(\Lambda N_0\)。故

\[
\boxed{q_0r=1+B\Lambda N_0.}
\tag{5.6}
\]

同时 (5.3)–(5.5) 直接给

\[
\boxed{N_0=Jq_0+s_0.}
\tag{5.7}
\]

由 \(s_*\ge1\)，(5.3) 给

\[
s_0>0.
\tag{5.8}
\]

置

\[
U=r-JB\Lambda=\rho+B\tau.
\]

因为 \(0<\rho<B\) 且 \(0\le\tau<\Lambda\)，

\[
0<U<B\Lambda.
\]

由 (5.6)–(5.7)，

\[
q_0U=1+B\Lambda s_0.
\]

而 \(q_0U<q_0B\Lambda\)，所以 \(s_0<q_0\)。因此

\[
\boxed{0<s_0<q_0.}
\tag{5.9}
\]

### 5.2 一般仿射恢复

全部自由终端状态唯一写成

\[
\boxed{q=q_0+B\Lambda y,}
\tag{5.10}
\]

\[
\boxed{s=s_0+(\rho+B\tau)y,}
\tag{5.11}
\]

\[
\boxed{N=N_0+ry,}
\tag{5.12}
\]

其中 \(y\in\mathbb Z_{\ge0}\)。这与

\[
qr=1+B\Lambda N,
\qquad
N=Jq+s
\tag{5.13}
\]

严格双向。由 (5.9)、(5.11)，真实状态总有 \(s>0\)；终端窗口再给
\(s<q\)。

---

## 6. 第一次二进下降与正缺陷正规形

真实指数为

\[
\boxed{N=2^e10^\mu,\qquad\mu=m-e\ge0.}
\tag{6.1}
\]

因为 \(e=2a+\delta>2a\)，

\[
\boxed{M\mid N.}
\tag{6.2}
\]

由 \(\rho\equiv1\pmod M\)、\(M\mid K\)，

\[
r\equiv1\pmod M,
\]

\[
N_0\equiv J+\epsilon_\tau+s_*\pmod M.
\]

定义

\[
\boxed{
A_\tau=J+\epsilon_\tau+s_*.
}
\tag{6.3}
\]

由 \(N=N_0+ry\) 模 \(M\)，

\[
\boxed{y\equiv-A_\tau\pmod M.}
\tag{6.4}
\]

所以唯一写成

\[
\boxed{y=Mz-A_\tau,}
\tag{6.5}
\]

其中

\[
\boxed{
z\in\mathbb Z,
\qquad
z\ge z_{\min}^{(0)}
:=
\left\lceil\frac{A_\tau}{M}\right\rceil.
}
\tag{6.6}
\]

因为 \(s_*\ge1\)、\(J\ge1\)，有 \(A_\tau\ge2\)，从而
\(z_{\min}^{(0)}\ge1\)。但本文不把更强下端误写成统一 \(z\ge1\)：
\(A_\tau\) 可以大于 \(M\)。

定义

\[
\boxed{
\Omega_\tau=A_\tau\Lambda-\lambda_\tau.
}
\tag{6.7}
\]

由 \(A_\tau\ge2\)、\(0\le\lambda_\tau<\Lambda\)，

\[
\boxed{\Omega_\tau\ge\Lambda+1>0.}
\tag{6.8}
\]

使用 \(\lambda_\tau=\theta+\epsilon_\tau\Lambda-\tau\) 与 (4.9)，

\[
\begin{aligned}
\Omega_\tau
&=(J+\epsilon_\tau+s_*)\Lambda
 -(\theta+\epsilon_\tau\Lambda-\tau)\\
&=J\Lambda+\tau+(\Lambda s_*-\theta).
\end{aligned}
\]

所以有一个更短的闭式

\[
\boxed{\Omega_\tau=V+\Xi.}
\tag{6.9}
\]

### 6.1 关键下降恒等式

由 (5.5)、(6.3)、\(\rho=1+Mc\) 及 \(B=K\Lambda\)，

\[
\begin{aligned}
N_0-A_\tau r
={}&\rho(J+\epsilon_\tau)+s_*+KV\lambda_\tau\\
&-(J+\epsilon_\tau+s_*)(\rho+K\Lambda V)\\
={}&s_*(1-\rho)+KV(\lambda_\tau-A_\tau\Lambda)\\
={}&-M c s_*-M5^\kappa V\Omega_\tau.
\end{aligned}
\]

因此题设中排版为逗号的项应严格读作乘积，准确恒等式是

\[
\boxed{
N_0-A_\tau r
=
-M c s_*-M5^\kappa V\Omega_\tau.
}
\tag{6.10}
\]

将 (6.5) 代入 \(N=N_0+ry\)，得到

\[
\boxed{
\frac NM
=
zr-cs_*-5^\kappa V\Omega_\tau.
}
\tag{6.11}
\]

定义正缺陷

\[
\boxed{
\mathcal D_\tau
=
cs_*+5^\kappa V\Omega_\tau
=
cs_*+5^\kappa V(V+\Xi)>0.
}
\tag{6.12}
\]

由 \(N/M=2^\delta10^\mu\)，核心指数正规形为

\[
\boxed{
2^\delta10^\mu
=
zr-\mathcal D_\tau.
}
\tag{6.13}
\]

### 6.2 反向充分性

固定一个满足第 1–3 节局部门的

\[
(a,\Delta,h,J,\tau).
\]

任取整数对

\[
z\ge z_{\min}^{(0)},
\qquad
\mu\ge0
\]

满足 (6.13)，定义 \(y=Mz-A_\tau\)。则 \(y\ge0\)，并由 (6.10)
反向得到

\[
N_0+ry=M2^\delta10^\mu=2^e10^\mu.
\]

再由 (5.10)–(5.12) 唯一恢复 \(q,s,N\)，自动满足 (5.13) 与
\(0<s<q\)。所以 (6.13) 与原仿射终端状态严格双向，不只是必要同余。

---

## 7. 终端商、共轭和差与符号分室

GAL-2 中

\[
L=\lambda_\tau+\Lambda y.
\]

代入 (6.5)、(6.7)，得到

\[
\boxed{
L=M\Lambda z-\Omega_\tau.
}
\tag{7.1}
\]

因此

\[
\boxed{
q=\rho+B(M\Lambda z-\Omega_\tau).
}
\tag{7.2}
\]

联合 \(r=\rho+BV\)，

\[
\boxed{
q+r
=
2\rho+B(M\Lambda z-\Omega_\tau+V),
}
\tag{7.3}
\]

\[
\boxed{
q-r
=
B(M\Lambda z-\Omega_\tau-V).
}
\tag{7.4}
\]

由 (7.1)，更透明的符号式为

\[
\boxed{
q-r=B(L-V),
\qquad
L-V=\Lambda(y-J)+(\lambda_\tau-\tau).
}
\tag{7.5}
\]

因此

\[
\boxed{
\begin{array}{c|c}
y\le J-1&q<r\\
y\ge J+1&q>r\\
y=J&\operatorname{sgn}(q-r)=\operatorname{sgn}(\lambda_\tau-\tau)
\end{array}}
\tag{7.6}
\]

若 \(q=r\)，则 \(L=V\)。模 \(\Lambda\) 立即给
\(\lambda_\tau=\tau\)，即 \(\tau\) 是唯一固定点；该点已由精确根门删除。
故

\[
\boxed{q=r\text{ 不可能}.}
\tag{7.7}
\]

令

\[
y_0=Mz_{\min}^{(0)}-A_\tau\in\{0,\ldots,M-1\}.
\tag{7.8}
\]

当 \(z\ge z_{\min}^{(0)}+1\) 时，\(y\ge y_0+M>M-1\ge J+1\)，故
\(q>r\)。所以 \(q<r\) 只可能发生在最小 \(z=z_{\min}^{(0)}\) 上；
它不能先验删除。例如若 \(M\mid A_\tau\)，则最小端有 \(y=0\)，从而
\(L=\lambda_\tau<V\) 及 \(q<r\)。

进位室 \(\epsilon_\tau\) 本身不能统一决定 (7.6)：同一室中的
\(\lambda_\tau-\tau\) 仍随 \(\tau\) 改变，而 \(y_0\) 取决于
\(A_\tau\bmod M\)。

### 7.1 \(q+r\) 的精确赋值

因 \(B\) 被 \(M=2^{2a}\) 整除，且 \(\rho=1+Mc\)，

\[
q+r\equiv2\pmod M.
\]

又因 \(\rho\equiv-1\pmod5\)、\(5\mid B\)，

\[
q+r\equiv-2\pmod5.
\]

所以

\[
\boxed{
v_2(q+r)=1,
\qquad
v_5(q+r)=0.
}
\tag{7.9}
\]

### 7.2 \(q-r\) 的精确五进阶与二进下界

由 (3.4) 模 5，

\[
M(\lambda_\tau-\tau)
\equiv-2(x+M\tau)\not\equiv0\pmod5.
\]

而 \(L-V\equiv\lambda_\tau-\tau\pmod5\)，故

\[
v_5(L-V)=0.
\]

结合 \(B=2^{2a}5^{2\varphi}\)，

\[
\boxed{v_5(q-r)=2\varphi.}
\tag{7.10}
\]

第 9 节将证明 \(L-V\) 为偶数。因此

\[
\boxed{
v_2(q-r)
=
2a+v_2(L-V)
\ge2a+1.
}
\tag{7.11}
\]

现有关系不固定 \(v_2(L-V)\) 的更高阶；同层消去必须保留。

---

## 8. 缺陷互素性、单位塌缩与唯一有限指数段

由 (6.10) 可写成

\[
\boxed{
M\mathcal D_\tau=A_\tau r-N_0.
}
\tag{8.1}
\]

GAL-2 已证明

\[
\gcd(N_0,r)=1,
\qquad
\gcd(M,r)=1.
\]

若素数同时整除 \(\mathcal D_\tau\) 与 \(r\)，由 (8.1) 也整除
\(N_0\)，矛盾。因此

\[
\boxed{\gcd(\mathcal D_\tau,r)=1.}
\tag{8.2}
\]

式 (6.13) 模 \(r\) 给

\[
\boxed{
10^\mu
\equiv
-2^{-\delta}\mathcal D_\tau
\pmod r.
}
\tag{8.3}
\]

### 8.1 离散对数目标的进一步塌缩

由 (5.6)，

\[
B\Lambda N_0\equiv-1\pmod r.
\]

由 (8.1)，

\[
M\mathcal D_\tau\equiv-N_0\pmod r.
\]

消去 \(N_0\)，得到

\[
\boxed{
\mathcal D_\tau
\equiv
(M^2\Lambda^2 5^\kappa)^{-1}
\pmod r.
}
\tag{8.4}
\]

因为

\[
M^2\Lambda^2 5^\kappa
=
2^{4a}5^{6\Delta+\kappa}
=
2^{4a}5^{2a+\Delta},
\]

(8.3) 可改写为

\[
\boxed{
10^\mu
\equiv
-2^{-(4a+\delta)}5^{-(2a+\Delta)}
\pmod r,
}
\tag{8.5}
\]

或等价地

\[
\boxed{
2^{2a+h}10^{\mu+2a+\Delta}
\equiv-1\pmod r.
}
\tag{8.6}
\]

这说明离散对数目标除移动模数 \(r\) 外不再显含 \(J,\tau\)；但它没有
把移动阶 \(\operatorname{ord}_r(10)\) 固定下来。

还应审计 Jacobi 路线。由 \(r\equiv1\pmod8\) 与
\(r\equiv-1\pmod5\)，对正奇数 \(r\) 的广义 Jacobi 符号有

\[
\left(\frac{-1}{r}\right)
=
\left(\frac2r\right)
=
\left(\frac5r\right)
=1.
\]

所以 (8.5) 的右端自动是 Jacobi 二次剩余；这里不存在类似 GA1-1 的统一
Jacobi 矛盾。

### 8.2 唯一指数同余类

令

\[
\boxed{P_r=\operatorname{ord}_r(10).}
\tag{8.7}
\]

若 (8.3) 的右端不属于

\[
\langle10\rangle\subset(\mathbb Z/r\mathbb Z)^\times,
\]

该整个局部状态为空。

若属于，则存在唯一

\[
\mu_0\in\{0,\ldots,P_r-1\}
\]

使全部非负指数解满足

\[
\boxed{\mu\equiv\mu_0\pmod{P_r}.}
\tag{8.8}
\]

每个指数唯一恢复

\[
\boxed{
z=
\frac{\mathcal D_\tau+2^\delta10^\mu}{r}.
}
\tag{8.9}
\]

### 8.3 精确下端

置

\[
y_0=Mz_{\min}^{(0)}-A_\tau\in\{0,\ldots,M-1\}.
\]

定义

\[
\boxed{
D_0=z_{\min}^{(0)}r-\mathcal D_\tau.
}
\tag{8.10}
\]

由 (8.1)，

\[
\begin{aligned}
MD_0
&=Mz_{\min}^{(0)}r-M\mathcal D_\tau\\
&=(A_\tau+y_0)r-(A_\tau r-N_0)\\
&=y_0r+N_0>0.
\end{aligned}
\]

故

\[
\boxed{D_0>0.}
\tag{8.11}
\]

式 (8.9) 满足 \(z\ge z_{\min}^{(0)}\) 当且仅当

\[
2^\delta10^\mu\ge D_0.
\]

定义完全整数化的下端

\[
\boxed{
\mu_{\min}
=
\min\{u\in\mathbb Z_{\ge0}:2^\delta10^u\ge D_0\}.
}
\tag{8.12}
\]

等号端点完整保留。

### 8.4 严格大小门与 \(\mu_{\max}\)

继承大小门为

\[
20\cdot10^m<194029Z^2Y,
\qquad
Z=\frac{B\Lambda}{2},
\qquad
Y=10^{3a},
\qquad
m=e+\mu.
\tag{8.13}
\]

置

\[
\mathscr X=194029Z^2Y,
\tag{8.14}
\]

\[
\boxed{
Q_\mu
=
\left\lfloor
\frac{\mathscr X-1}{20\cdot10^e}
\right\rfloor.
}
\tag{8.15}
\]

若 \(Q_\mu<1\)，该状态整体为空。否则定义

\[
\boxed{
\mu_{\max}
=
\max\{u\in\mathbb Z_{\ge0}:10^u\le Q_\mu\}.
}
\tag{8.16}
\]

这与严格门完全等价，并满足相邻阈值

\[
\boxed{
20\cdot10^{e+\mu_{\max}}
<\mathscr X
\le
20\cdot10^{e+\mu_{\max}+1}.
}
\tag{8.17}
\]

### 8.5 完整有限指数段

若离散对数存在，定义

\[
t_{\min}
=
\max\left(
0,
\left\lceil\frac{\mu_{\min}-\mu_0}{P_r}\right\rceil
\right),
\tag{8.18}
\]

\[
t_{\max}
=
\left\lfloor
\frac{\mu_{\max}-\mu_0}{P_r}
\right\rfloor.
\tag{8.19}
\]

若 \(t_{\min}>t_{\max}\)，该状态为空；否则全部指数恰为

\[
\boxed{
\mu=\mu_0+tP_r,
\qquad
t_{\min}\le t\le t_{\max}.
}
\tag{8.20}
\]

每个指数由 (8.9)、(6.5)、(7.1)、(5.10)–(5.12) 唯一恢复
\(z,y,L,q,s,N\)。这是完整有限同余段，不是有限采样 \(\mu\)。

对应的准确整数上端为

\[
\boxed{
z\le
z_{\max}
:=
\left\lfloor
\frac{\mathcal D_\tau+2^\delta10^{\mu_{\max}}}{r}
\right\rfloor.
}
\tag{8.21}
\]

这里必须使用 \(\le\)；若最大指数恰满足整除，等号可以发生。

---

## 9. 奇偶、二进与五进赋值字典

由 (6.7)、(4.8) 与 (2.6)，模 2 有

\[
\begin{aligned}
\Omega_\tau
&\equiv A_\tau-\lambda_\tau\\
&\equiv J+\epsilon_\tau+s_*
 -(\theta+\epsilon_\tau-\tau)\\
&\equiv J+\tau.
\end{aligned}
\]

所以

\[
\boxed{\Omega_\tau\equiv J+\tau\pmod2.}
\tag{9.1}
\]

又因 \(\Lambda\) 为奇数，

\[
\boxed{V\equiv J+\tau\pmod2.}
\tag{9.2}
\]

从而

\[
\boxed{V\equiv\Omega_\tau\pmod2.}
\tag{9.3}
\]

结合根门 \(c+J+\tau\equiv1\pmod2\)：

- 若 \(c\) 为偶数，则 \(V,\Omega_\tau\) 均为奇数；
- 若 \(c\) 为奇数，则 \(V,\Omega_\tau\) 均为偶数。

### 9.1 缺陷的完整二进阶

记

\[
d_2=v_2(\mathcal D_\tau).
\tag{9.4}
\]

若 \(c\) 为偶数，\(cs_*\) 为偶数而
\(5^\kappa V\Omega_\tau\) 为奇数，所以

\[
\boxed{c\equiv0\pmod2\Longrightarrow d_2=0.}
\tag{9.5}
\]

若 \(c\) 为奇数，则 \(V\Omega_\tau\) 被 \(4\) 整除。

- 若 \(s_*\) 为奇数，第一项为奇数，故 \(d_2=0\)；
- 若 \(s_*\) 为偶数，置
  \[
  \alpha_2=v_2(s_*)\ge1,
  \qquad
  \beta_2=v_2(V)+v_2(\Omega_\tau)\ge2.
  \]
  当 \(\alpha_2\ne\beta_2\) 时，
  \[
  \boxed{d_2=\min(\alpha_2,\beta_2).}
  \tag{9.6}
  \]
  当 \(\alpha_2=\beta_2=w\) 时，必须保留同层消去：
  \[
  \boxed{
  d_2
  =w+v_2\left(
  \frac{cs_*}{2^w}
  +
  \frac{5^\kappa V\Omega_\tau}{2^w}
  \right).
  }
  \tag{9.7}
  \]
  括号中两项均为奇数，所以额外阶至少为 \(1\)。

这穷尽全部二进同层情形，不能只取两项赋值的最小值。

由

\[
rz=\mathcal D_\tau+2^{\delta+\mu}5^\mu
\tag{9.8}
\]

且 \(r\) 为奇数，若记 \(n_2=\delta+\mu\)，则

\[
\boxed{
v_2(z)=
\begin{cases}
n_2,&n_2<d_2,\\
d_2,&n_2>d_2,\\
d_2+t_2,&n_2=d_2,
\end{cases}}
\tag{9.9}
\]

其中同层额外阶为

\[
\boxed{
t_2=v_2\left(
\frac{\mathcal D_\tau}{2^{d_2}}+5^\mu
\right)\ge1.
}
\tag{9.10}
\]

前、后两室还分别给出标准低位

\[
\frac{z}{2^{n_2}}
\equiv5^\mu r^{-1}\pmod{2^{d_2-n_2}}
\qquad(n_2<d_2),
\tag{9.11}
\]

\[
\frac{z}{2^{d_2}}
\equiv
\frac{\mathcal D_\tau}{2^{d_2}}r^{-1}
\pmod{2^{n_2-d_2}}
\qquad(n_2>d_2).
\tag{9.12}
\]

### 9.2 缺陷的完整五进阶

由 \(Mc\equiv-2\pmod C\)，

\[
\boxed{5\nmid c.}
\tag{9.13}
\]

置

\[
\alpha_5=v_5(s_*),
\qquad
\beta_5=\kappa+v_5(V)+v_5(\Omega_\tau).
\tag{9.14}
\]

则

\[
\boxed{
v_5(\mathcal D_\tau)=
\begin{cases}
\min(\alpha_5,\beta_5),&\alpha_5\ne\beta_5,\\[1mm]
\alpha_5+v_5\left(
\dfrac{cs_*}{5^{\alpha_5}}
+
\dfrac{5^\kappa V\Omega_\tau}{5^{\beta_5}}
\right),&\alpha_5=\beta_5.
\end{cases}}
\tag{9.15}
\]

当 \(\kappa>0\) 时，

\[
\mathcal D_\tau\equiv cs_*\pmod5.
\tag{9.16}
\]

所以若 \(5\nmid s_*\)，立即有

\[
\boxed{v_5(\mathcal D_\tau)=0.}
\tag{9.17}
\]

若 \(5\mid s_*\)，则仍必须使用 (9.15)：第二项可能追上第一项并发生
同层消去。

当 \(\kappa=0\) 时，两项没有先验层差，必须完整保留

\[
v_5(cs_*+V\Omega_\tau),
\]

这正是 (9.15) 的边界版本。

### 9.3 \(\mu\) 与 \(v_5(\mathcal D_\tau)\) 的三室走廊

记

\[
d_5=v_5(\mathcal D_\tau).
\tag{9.18}
\]

由 (9.8) 且 \(5\nmid r\)，

\[
\boxed{
v_5(z)=
\begin{cases}
\mu,&\mu<d_5,\\
d_5,&\mu>d_5,\\
d_5+t_5,&\mu=d_5,
\end{cases}}
\tag{9.19}
\]

其中同层额外阶为

\[
\boxed{
t_5
=
v_5\left(
\frac{\mathcal D_\tau}{5^{d_5}}
+2^{\delta+d_5}
\right).
}
\tag{9.20}
\]

前、后两室分别给出

\[
\frac{z}{5^\mu}
\equiv
2^{\delta+\mu}r^{-1}
\pmod{5^{d_5-\mu}}
\qquad(\mu<d_5),
\tag{9.21}
\]

\[
\frac{z}{5^{d_5}}
\equiv
\frac{\mathcal D_\tau}{5^{d_5}}r^{-1}
\pmod{5^{\mu-d_5}}
\qquad(\mu>d_5).
\tag{9.22}
\]

式 (9.15)、(9.19)–(9.22) 是完整五进赋值走廊；它不要求枚举任何长度随
\(\Delta\) 增长的提升商。

### 9.4 \(L-V\) 为偶数

由 \(y=Mz-A_\tau\)，模 2 有

\[
y\equiv A_\tau\equiv J+\epsilon_\tau+s_*.
\]

因此

\[
\begin{aligned}
L-V
&\equiv\lambda_\tau+y-J-\tau\\
&\equiv(\theta+\epsilon_\tau-\tau)
 +(J+\epsilon_\tau+s_*)-J-\tau\\
&\equiv\theta+s_*\equiv0\pmod2.
\end{aligned}
\]

这证明了 (7.11) 所用的

\[
\boxed{2\mid L-V.}
\tag{9.23}
\]

---

## 10. 第二 Bezout 坐标与能力审计

定义

\[
\boxed{
X_V=x+MV,
\qquad
D_V=c+CV,
}
\tag{10.1}
\]

\[
\boxed{
X_L=x+ML,
\qquad
D_L=c+CL.
}
\tag{10.2}
\]

由 \(Cx-Mc=2\)，逐项有

\[
\boxed{
CX_V-MD_V=2,
\qquad
CX_L-MD_L=2.
}
\tag{10.3}
\]

又由 \(\rho=Cx-1=1+Mc\)，

\[
\boxed{
r=-1+CX_V=1+MD_V,
}
\tag{10.4}
\]

\[
\boxed{
q=-1+CX_L=1+MD_L.
}
\tag{10.5}
\]

将 (10.4)–(10.5) 代入 \(qr=1+MC\Lambda N\)，约去 \(C\)，得到

\[
\boxed{
CX_LX_V-X_L-X_V=M\Lambda N.
}
\tag{10.6}
\]

因为 \(C=\Lambda5^\kappa\)，(10.6) 模 \(\Lambda\) 给

\[
\boxed{\Lambda\mid X_L+X_V.}
\tag{10.7}
\]

定义

\[
\boxed{
T=\frac{X_L+X_V}{\Lambda}.
}
\tag{10.8}
\]

由

\[
L+V=\theta+\Lambda(J+\epsilon_\tau+y)
\]

与 (4.5)，

\[
\boxed{
T=t_*+M(J+\epsilon_\tau+y).
}
\tag{10.9}
\]

代入 \(y=Mz-A_\tau\)，得到

\[
\boxed{
T=t_*+M(Mz-s_*).
}
\tag{10.10}
\]

将 (10.6) 除以 \(\Lambda\)，

\[
\boxed{
5^\kappa X_LX_V-T=MN.
}
\tag{10.11}
\]

再用 \(N=M2^\delta10^\mu\)，得到

\[
\boxed{
5^\kappa X_LX_V-T
=
M^2 2^\delta10^\mu.
}
\tag{10.12}
\]

### 10.1 gcd 与固定行列式字典

由 \(Cx\equiv2\pmod M\) 且 \(a\ge3\)，

\[
x\equiv2\pmod4.
\]

所以

\[
\boxed{v_2(X_V)=v_2(X_L)=1.}
\tag{10.13}
\]

精确根门与反射保持性给

\[
5\nmid X_VX_L.
\tag{10.14}
\]

又由 (1.16)，

\[
D_V=c+CV\equiv c+J+\tau\equiv1\pmod2.
\]

对 \(D_L\)，由第 9.4 节的奇偶计算有 \(L\equiv J+\tau\pmod2\)，故

\[
D_L=c+CL\equiv c+J+\tau\equiv1\pmod2.
\]

所以 (10.3) 进一步给

\[
\boxed{
\gcd(X_V,D_V)=\gcd(X_L,D_L)=1.
}
\tag{10.15}
\]

而

\[
\boxed{
v_2(\gcd(X_L,X_V))=1,
\qquad
v_5(\gcd(X_L,X_V))=0.
}
\tag{10.16}
\]

奇素数公共因子仍可随状态移动。交叉行列式为

\[
\boxed{
X_LD_V-X_VD_L=2(V-L),
}
\tag{10.17}
\]

不是新的固定小常数。

### 10.2 \(M^2\) 高位限制是否独立

由 (10.13)，\(v_2(5^\kappa X_LX_V)=2\)。又因
\(X_L\equiv X_V\equiv x\pmod M\)，

\[
T\equiv2x\Lambda^{-1}\pmod M,
\]

所以 \(v_2(T)=2\)。式 (10.12) 表现为两个二进阶均为 \(2\) 的量发生
很高阶消去。

但将 (7.1)、(10.1)–(10.2)、(10.10) 直接代入，可得整数恒等式

\[
\boxed{
5^\kappa X_LX_V-T
=
M^2(zr-\mathcal D_\tau).
}
\tag{10.18}
\]

因此 (10.12) 与第一次下降 (6.13) 严格等价。特别地：

1. 模 \(M^2\) 的高位限制只是 (6.13) 的同一低位数字；
2. 高二进消去不是额外矛盾；
3. 固定行列式 \(2\) 已完全体现在坐标变换中；
4. (10.16) 只固定 \((2,5)\)-部分，奇素数 gcd 仍移动；
5. 不能把 (10.12) 的恒等回代误报为新平方门。

---

## 11. 边界 \(\kappa=0\)

边界条件为

\[
2\varphi=3\Delta
\iff
2a=5\Delta.
\]

因 \(\gcd(2,5)=1\)，存在唯一整数 \(u\ge1\) 使

\[
\boxed{
(a,\Delta,\varphi)=(5u,2u,3u).
}
\tag{11.1}
\]

这是无界射线，不是有限小端。此时

\[
\boxed{C=\Lambda,\qquad K=M,\qquad B=M\Lambda.}
\tag{11.2}
\]

核心方程成为

\[
\boxed{
2^\delta10^\mu
=
zr-cs_*-V\Omega_\tau.
}
\tag{11.3}
\]

使用 \(\Omega_\tau=V+\Xi\)，缺陷是显式二次式

\[
\boxed{
\mathcal D_\tau
=
V^2+\Xi V+cs_*.
}
\tag{11.4}
\]

第二 Bezout 式成为

\[
\boxed{
X_LX_V-T=M^2 2^\delta10^\mu.
}
\tag{11.5}
\]

但 (10.18) 在 \(\kappa=0\) 时仍给

\[
X_LX_V-T=M^2(zr-\mathcal D_\tau),
\]

所以 (11.5) 仍只是 (11.3) 的恒等改写。

奇偶方面：若 \(c\) 偶，则 \(V\Omega_\tau\) 奇而缺陷奇；若 \(c\) 奇，
则 \(V,\Omega_\tau\) 均偶，缺陷的奇偶由 \(s_*\) 决定。二者都在无界
射线上实际允许，故没有统一奇偶矛盾。

五进方面必须使用 (9.15) 的

\[
v_5(cs_*+V\Omega_\tau)
\]

同层公式，不能把一项当作高阶扰动。现有恒等式也不强迫二次式 (11.4) 的
判别式为平方，因而没有固定平方因子分解或固定小差。

第 8 节的离散对数和严格大小门仍随 \(u,J,\tau,r\) 移动；本文没有得到
\(u\) 的绝对上界。因此 \(\kappa=0\) 整条射线保持开放。

---

## 12. 完整生成顺序与状态参数化

本区域的全部终端候选必须、且在终端层面只须按以下有限模式生成。

1. 取
   \[
   a\ge3,
   \qquad
   1\le\Delta\le\left\lfloor\frac{2a}{5}\right\rfloor,
   \qquad
   \varphi=a-\Delta.
   \]
2. 取 \(h\in\mathcal H(a)\)，置
   \[
   \delta=\Delta+h,
   \quad
   e=2a+\delta,
   \quad
   \kappa=2a-5\Delta.
   \]
3. 构造
   \[
   M=2^{2a},
   \quad
   \Lambda=5^{3\Delta},
   \quad
   C=\Lambda5^\kappa,
   \quad
   B=M C.
   \]
4. 唯一计算
   \[
   x=\langle2C^{-1}\rangle_M,
   \quad
   c=(Cx-2)/M,
   \quad
   \rho=Cx-1,
   \quad
   \eta=cx,
   \]
   以及 \(\theta,g,s_*,t_*,\Xi\)。这些步骤不含搜索分支。
5. 取 \(J\in\{1,\ldots,9\}\)，再取一个标准代表
   \[
   0\le\tau<\Lambda,
   \quad
   x+M\tau\equiv2,3\pmod5,
   \quad
   c+J+\tau\equiv1\pmod2.
   \]
   可直接使用第 3.3 节的两个模 10 等差类生成，不进行逐位 Hensel 提升。
6. 唯一置
   \[
   \lambda_\tau=\langle\theta-\tau\rangle_\Lambda,
   \quad
   \epsilon_\tau=(\tau+\lambda_\tau-\theta)/\Lambda.
   \]
7. 构造第 5–7 节全部局部量和缺陷，计算
   \(P_r=\operatorname{ord}_r(10)\)，检查 (8.3) 或等价的 (8.6)。
8. 若离散对数存在，按 (8.20) 生成唯一完整有限指数段；每个指数用
   (8.9) 唯一恢复 \(z\)，再恢复 \(y,L,q,s,N\)。
9. 最后进入继承的十三首块、\(a_2\) 窗口、判别式平方、两个恢复符号、
   精确 gcd 尺度、\(a_3\) 窗口、三个逐项既约及原题直接回代。

第 1–8 步在终端层严格双向；第 9 步仍是完整原题候选不可省略的恢复门。
本文没有把终端状态误报为合法六元组。

准确的状态结构是：

\[
\boxed{
\begin{array}{c|c|c|c}
\text{室}&\tau\text{ 区间}&\lambda_\tau&\epsilon_\tau\\ \hline
0&0\le\tau\le\theta&\theta-\tau&0\\
1&\theta<\tau<\Lambda&\theta+\Lambda-\tau&1
\end{array}}
\tag{12.1}
\]

每个 \(\tau\) 的 \((\lambda_\tau,\epsilon_\tau)\) 唯一；固定点已删除；
不存在自由 Hensel 输出数字；每个固定状态只剩至多一条有限指数段。
但是 (3.12)–(3.13) 显示叶节点数仍随 \(\Lambda\) 增长，不能误报为绝对
有限。

---

## 13. 主动端点审计

### 13.1 \(\theta=0\)

公式全部仍成立。此时唯一固定点为 \(\tau_*=0\)，并由 (3.3) 违反根门。
室 0 只有 \(\tau=0\)，故没有合法状态；其余合法状态全部位于室 1。
本文没有先验断言 \(\theta>0\)。

### 13.2 \(\tau=0\)

若 \(x\equiv2\) 或 \(3\pmod5\)，且奇偶门通过，则它是合法有向状态。
此时 \(\lambda_0=\theta\)、\(\epsilon_0=0\)。除 \(\theta=0\) 的已删固定
情形外，必须保留。

### 13.3 \(\tau=\theta\) 与 \(\lambda_\tau=0\)

两者严格等价，并属于 \(\epsilon_\tau=0\) 的闭端点。它与 \(\tau=0\)
组成二循环；是否通过根门和奇偶门由 (1.15)–(1.16) 决定，不能统一删除。

### 13.4 \(\epsilon_\tau=0,1\)

两个室均由 (2.7a)–(2.7b) 双向覆盖。精确合法状态数分别为
(3.12)、(3.13)，没有遗漏进位室。

### 13.5 被删除的唯一固定点

固定点唯一为 (3.2)，且 (3.3) 使其违反精确根门。删除不依赖奇偶门，
也不删除同一二循环中的其他非固定状态，因为固定点自身是一循环。

### 13.6 \(s_*=0\)

由 (4.2) 的正分子严格不可能。准确结论是 \(s_*\ge1\)。

### 13.7 \(s_0=0\)

由 (5.3) 与 \(s_*\ge1\) 严格不可能；全部状态有 \(0<s_0<q_0\)。

### 13.8 \(y=0\)

不能统一删除。它当且仅当 \(M\mid A_\tau\) 且
\(z=z_{\min}^{(0)}=A_\tau/M\)。此时 \(L=\lambda_\tau<V\)，故
\(q<r\)，但其余终端恒等式仍完整成立。

### 13.9 \(A_\tau\) 是 \(M\) 的倍数

该端点已由 13.8 保留。本文没有用有限前缀未观察到它来作理论删除。

### 13.10 \(z=z_{\min}^{(0)}\)

完整保留。其是否产生指数由下端 \(2^\delta10^\mu\ge D_0\)、离散对数
和严格大小门共同决定。

### 13.11 \(\Omega_\tau=1\)

由 \(A_\tau\ge2\)、\(\lambda_\tau\le\Lambda-1\)，
\(\Omega_\tau\ge\Lambda+1\)，故严格不可能。

### 13.12 \(q=r\)

它强迫 \(L=V\)，进而强迫 \(\lambda_\tau=\tau\)，即被删除的固定点。
所以严格不可能。

### 13.13 \(q-r<0\)

不能先验删除。准确符号字典为 (7.6)；负号只可能发生在最小 \(z\) 端，
但现有恒等式没有统一排除该端点。

### 13.14 \(\kappa=0\)

第 11 节完整保留无界射线 \((5u,2u,3u)\)，没有把它当作有限小端。

### 13.15 \(\mu=0\)

完整包含在 (8.8)、(8.12)、(8.16) 和两个赋值三室中。若
\(d_5=0\)，它是五进同层；若 \(d_5>0\)，它属于前室。

### 13.16 五进同层消去

缺陷内部的同层由 (9.15) 保留；指数项与缺陷的同层由
(9.19)–(9.20) 保留。二者不能混为一次取最小值。

### 13.17 二进同层消去

缺陷内部的同层由 (9.7) 保留；指数项与缺陷的同层由
(9.9)–(9.10) 保留。两个奇单位之和会至少再提升一阶。

### 13.18 大小门严格端点

严格不等式通过 \((\mathscr X-1)/(20\cdot10^e)\) 下取整处理。
\(\mu_{\max}\) 满足相邻阈值 (8.17)；以 \(\mu_{\max}\) 写出的 \(z\)
上端必须使用 \(\le\)。

### 13.19 仿射反射的能力边界

反射退化只删除了逐位 Hensel 树。它没有自动删除任一非固定合法状态，也
没有固定移动模数 \(r\) 的十进制阶。

### 13.20 计算攻击的证明等级

为攻击公式错误，本文制作阶段以精确整数算术逐项核对了 227,251 个小参数
局部状态，又对 20,000 个跨更大参数的随机标准状态复核 (2.5)、(3.4)、
(5.6)–(5.9)、(6.10)–(6.13)、(8.4)、(10.3)–(10.18) 及全部端点奇偶。
另对 6,224,943 个小参数指数状态作过有限诊断，未发现终端命中。

这些计算只用于反例攻击和排版审计，不作为无界结论、分支无解或
GALS(-)-3 的证明。正式分类完全由上述符号双向推导成立。

---

## 14. 为什么不能升级为关闭或绝对有限化

本轮没有得到 GALS(-)-1，原因是：

1. 离散对数目标虽塌缩为 (8.6)，但模数 \(r\) 与阶
   \(\operatorname{ord}_r(10)\) 仍移动；Jacobi 符号自动相容。
2. 二进、五进走廊完整限制 \(z\) 的赋值，却没有与
   \([z_{\min}^{(0)},z_{\max}]\) 形成统一空交。
3. 第二 Bezout 式严格等价于第一次下降；模 \(M^2\) 的高位消去不是独立
   新门。
4. \(q-r\) 的五进阶固定，但更高二进阶和符号仍由移动量 \(L-V\) 控制。
5. \(\kappa=0\) 无界射线没有产生统一奇偶矛盾、平方分解或固定小差。

本轮没有得到 GALS(-)-2，因为 \(a,\Delta\) 未被压到绝对有限范围。

本轮没有得到 GALS(-)-4，因为两个进位室、\(\kappa>0\) 与
\(\kappa=0\) 均未统一关闭。

但本轮严格达到 GALS(-)-3：

- involution 完全退化成两个显式仿射反射室；
- 全部 Hensel 输出数字消失；
- 每个固定 \((a,\Delta,h,J,\tau)\) 至多只剩一条完整有限指数同余段；
- 每个指数唯一恢复全部剩余终端整数；
- 状态计数、端点、二进与五进同层消去均已显式封闭。

由于残余仍随 \(a,\Delta,\tau,r\) 无界，本文不生成伪造的绝对有限证书，
也不以任何有限 \(a\) 或 \(\Delta\) 前缀外推。

---

## 15. 最终分类与停止点

本轮严格建立

\[
\boxed{
\begin{gathered}
C=\Lambda5^\kappa,
\qquad
B=K\Lambda,\\
\theta=\langle\eta\rangle_\Lambda,
\qquad
\lambda_\tau=\langle\theta-\tau\rangle_\Lambda,\\
\tau+\lambda_\tau=\theta+\epsilon_\tau\Lambda,\\
\tau_*=\langle-xM^{-1}\rangle_\Lambda,
\qquad
x+M\tau_*\equiv0\pmod\Lambda,\\
s_*=g+5^\kappa x\theta,
\qquad
5^\kappa x^2=t_*+Mg,
\qquad
\Xi=\Lambda s_*-\theta,\\
r=\rho+BV,
\qquad
s_0=s_*+\rho\epsilon_\tau+K\tau\lambda_\tau,\\
q_0=\rho+B\lambda_\tau,
\qquad
N_0=\rho(J+\epsilon_\tau)+s_*+KV\lambda_\tau,\\
q_0r=1+B\Lambda N_0,
\qquad
N_0=Jq_0+s_0,
\qquad
0<s_0<q_0,\\
A_\tau=J+\epsilon_\tau+s_*,
\qquad
y=Mz-A_\tau,
\qquad
z\ge\left\lceil\frac{A_\tau}{M}\right\rceil,\\
\Omega_\tau=A_\tau\Lambda-\lambda_\tau=V+\Xi,\\
N_0-A_\tau r=-M c s_*-M5^\kappa V\Omega_\tau,\\
\mathcal D_\tau=cs_*+5^\kappa V\Omega_\tau>0,\\
2^\delta10^\mu=zr-\mathcal D_\tau,\\
L=M\Lambda z-\Omega_\tau,\\
q+r=2\rho+B(M\Lambda z-\Omega_\tau+V),\\
q-r=B(M\Lambda z-\Omega_\tau-V)\ne0,\\
v_2(q+r)=1,
\quad
v_5(q+r)=0,
\quad
v_5(q-r)=2\varphi,
\quad
v_2(q-r)\ge2a+1,\\
10^\mu\equiv-2^{-\delta}\mathcal D_\tau\pmod r,\\
2^{2a+h}10^{\mu+2a+\Delta}\equiv-1\pmod r,\\
\mu=\mu_0+t\operatorname{ord}_r(10),
\qquad
t_{\min}\le t\le t_{\max},\\
z=\dfrac{\mathcal D_\tau+2^\delta10^\mu}{r},\\
CX_V-MD_V=CX_L-MD_L=2,\\
5^\kappa X_LX_V-T
=M^2(zr-\mathcal D_\tau)
=M^2 2^\delta10^\mu.
\end{gathered}}
\tag{15.1}
\]

全部允许 \(\tau\) 由两个模 10 等差类和两个反射室显式给出；每个状态的
二进、五进赋值由第 9 节穷尽；全部指数由第 8 节的一条完整有限同余段
穷尽。因此本区域已经完全脱离 GAL-2 的 Hensel 树。

但外层 \((a,\Delta)\)、反射状态 \(\tau\)、移动模数 \(r\) 与阶
\(\operatorname{ord}_r(10)\) 仍无界；双 Bezout 坐标和 \(\kappa=0\)
边界均未产生统一矛盾。因此最终分类为

\[
\boxed{\mathrm{GALS(-)\text{-}3}.}
\]

本文到此停止，不研究浅正根、真正深区、高 \(\varphi\) 的
\(\mathcal F_{P-}\)、B、C、\(\gamma>1\)、C2/C5、Q 或严格层。
