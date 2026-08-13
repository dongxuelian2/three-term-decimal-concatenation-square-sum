# 三项十进制拼接平方和问题：临界 G 模板 A2 低 \(\varphi\) 浅深度正根报告

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

中的浅深度正根区域

\[
\boxed{
\mathcal L_{\mathrm{sh},+}:
\quad
\sigma=+1,
\qquad
2\varphi\ge3(a-\varphi).
}
\tag{0.1}
\]

接受 PR6、SD6、GA2-6、GE2-1 与 GAL-2 的完整终端系统；不研究浅负根、
真正深区、高 \(\varphi\) 的 \(\mathcal F_{P-}\)、B、C、\(\gamma>1\)、
非本原 C2/C5、Q 或严格层。

本轮得到以下严格结论。

1. 模 \(\Lambda\) 的 Möbius involution 完全退化为补数映射
   \(\tau\mapsto\Lambda-\tau\)，因而本区域不再含 Hensel 树；
2. 全部局部量均成为 \((J,\tau)\) 的显式多项式；
3. 第一次二进下降把仿射参数唯一写成
   \(y=Mz-(J+1)\)，并证明 \(z\ge1\)、\(y>0\)；
4. 每个固定 \((a,\Delta,h,J,\tau)\) 的全部指数至多是一条
   \(\operatorname{ord}_r(10)\)-级数，严格大小门再把它截成完整有限段；
5. \(z\) 对每个指数唯一显式恢复，并具有完整二进数字和三个五进赋值走廊；
6. 共轭和差给出 \(q>r\) 及精确 \((2,5)\)-赋值，但平方路线最终只是恒等式，
   没有关闭 \(\kappa>0\) 或 \(\kappa=0\)。

因此准确分类为

\[
\boxed{
\mathrm{GALS{+}\text{-}3}:
\quad
\text{involution 完全退化，得到二进下降、显式多项式正规形与每状态唯一有限指数段，}
\text{但仍有无界残余。}
}
\tag{0.2}
\]

没有找到合法原题六元组，也没有发现 GAL-2、GE2-1、GA2-6、PR6 或 SD6
的继承错误。

---

## 1. 参数与浅深度恒等式

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
}
\tag{1.4}
\]

\[
\boxed{K=M5^\kappa.}
\tag{1.5}
\]

因为

\[
\kappa+3\Delta=2\varphi,
\]

严格得到

\[
K\Lambda
=M5^{\kappa+3\Delta}
=M5^{2\varphi}
=MC
=B.
\]

因此

\[
\boxed{B=K\Lambda.}
\tag{1.6}
\]

这一步是后文全部约分的关键；没有把 \(K\) 与 GAL-2 中的
\(k^2-1\) 混用。

尾窗为

\[
h\in\mathcal H(a),
\qquad
e=2a+\Delta+h.
\tag{1.7}
\]

为缩短公式，记

\[
\boxed{\delta=\Delta+h,\qquad e=2a+\delta.}
\tag{1.8}
\]

正根中

\[
\rho=1,\qquad\eta=0.
\tag{1.9}
\]

全部真实局部状态还必须满足

\[
\boxed{
0\le\tau<\Lambda,
\qquad
\tau\equiv2\text{ 或 }3\pmod5,
}
\tag{1.10}
\]

\[
\boxed{J+\tau\equiv1\pmod2,\qquad J\in\{1,\ldots,9\}.}
\tag{1.11}
\]

由 (1.10)，\(\tau\ne0\)，故真实状态中

\[
\boxed{0<\tau<\Lambda.}
\tag{1.12}
\]

定义

\[
\boxed{V=J\Lambda+\tau.}
\tag{1.13}
\]

则

\[
J\Lambda<V<(J+1)\Lambda,
\qquad
\Lambda<V<10\Lambda,
\tag{1.14}
\]

而 (1.11) 与 \(\Lambda\) 为奇数给出

\[
\boxed{V\text{ 为奇数}.}
\tag{1.15}
\]

---

## 2. Möbius involution 的完全退化

GAL-2 的正根 involution 为

\[
\lambda_\tau
=
\left\langle
-\tau(1+B\tau)^{-1}
\right\rangle_\Lambda.
\tag{2.1}
\]

由 (1.6)，\(\Lambda\mid B\)，所以

\[
1+B\tau\equiv1\pmod\Lambda.
\]

其逆元唯一满足

\[
\boxed{(1+B\tau)^{-1}\equiv1\pmod\Lambda.}
\tag{2.2}
\]

因此

\[
\lambda_\tau\equiv-\tau\pmod\Lambda.
\tag{2.3}
\]

由 \(0<\tau<\Lambda\)，标准代表不是 \(0\)，而是

\[
\boxed{\lambda_\tau=\Lambda-\tau.}
\tag{2.4}
\]

特别地，

\[
\boxed{0<\lambda_\tau<\Lambda.}
\tag{2.5}
\]

反向方向同样成立：任取满足 (1.10) 的 \(\tau\)，(2.4) 直接满足

\[
\lambda_\tau(1+B\tau)\equiv-\tau\pmod\Lambda,
\]

所以它恰是 GAL-2 的标准 Möbius 像，不是额外放宽的补数参数。

补数映射满足

\[
\tau\longleftrightarrow\Lambda-\tau.
\tag{2.6}
\]

并交换模 5 的两个合法数字 \(2,3\)。在允许状态上没有固定点。这里应精确区分：

- 在整个环 \(\mathbb Z/\Lambda\mathbb Z\) 上，\(\tau=0\) 仍是补数映射的固定点；
- 该点已经被正根精确五进门删除；
- 对 \(0<\tau<\Lambda\)，若标准代表满足
  \(\tau=\Lambda-\tau\)，则 \(2\tau=\Lambda\)，与 \(\Lambda\) 为奇数矛盾。

所以准确结论是

\[
\boxed{
\text{全部允许浅正根状态组成非平凡二循环；本区域不再需要任何逐位 Hensel 递推。}
}
\tag{2.7}
\]

此外，二循环两端奇偶相反，因为

\[
\Lambda-\tau\equiv1-\tau\pmod2.
\]

故对固定 \(J\)，终端模 8 门 (1.11) 在每个二循环中恰保留一个有向端点。
根门共有 \(2\cdot5^{3\Delta-1}\) 个 \(\tau\)，配成
\(5^{3\Delta-1}\) 个二循环；终端奇偶门对每个 \(J\) 恰留下

\[
\boxed{5^{3\Delta-1}}
\]

个有向状态。这个计数只描述状态族，不要求枚举这些 \(\tau\)。

---

## 3. 全部局部状态的闭式

沿用

\[
V=J\Lambda+\tau,
\qquad
\lambda=\Lambda-\tau.
\tag{3.1}
\]

正根终端量为

\[
\boxed{r=1+BV,}
\tag{3.2}
\]

\[
\boxed{q_0=1+B\lambda=1+B(\Lambda-\tau),}
\tag{3.3}
\]

\[
\begin{aligned}
s_0
&=\frac{\tau+\lambda+B\tau\lambda}{\Lambda}\\
&=1+\frac B\Lambda\tau(\Lambda-\tau).
\end{aligned}
\]

使用 \(B/\Lambda=K\)，得到

\[
\boxed{s_0=1+K\tau(\Lambda-\tau).}
\tag{3.4}
\]

再由 \(N_0=Jq_0+s_0\)，

\[
\begin{aligned}
N_0
&=J+1+JB(\Lambda-\tau)+K\tau(\Lambda-\tau)\\
&=J+1+K(J\Lambda+\tau)(\Lambda-\tau),
\end{aligned}
\]

所以

\[
\boxed{N_0=J+1+KV(\Lambda-\tau).}
\tag{3.5}
\]

### 3.1 对终端乘积的独立复核

由 (3.2)–(3.3)，

\[
\begin{aligned}
q_0r
&=(1+B\lambda)(1+BV)\\
&=1+B(V+\lambda)+B^2V\lambda.
\end{aligned}
\]

而

\[
V+\lambda
=J\Lambda+\tau+\Lambda-\tau
=(J+1)\Lambda,
\]

\[
B^2V\lambda
=B\Lambda\,KV\lambda.
\]

故

\[
q_0r
=1+B\Lambda\{J+1+KV\lambda\}
=1+B\Lambda N_0.
\]

即

\[
\boxed{q_0r=1+B\Lambda N_0.}
\tag{3.6}
\]

这独立验证了 (3.3)–(3.5)。

### 3.2 余数端点

由 (3.4)，

\[
\boxed{s_0>0.}
\tag{3.7}
\]

并且

\[
\begin{aligned}
q_0-s_0
&=B(\Lambda-\tau)-K\tau(\Lambda-\tau)\\
&=K(\Lambda-\tau)^2>0.
\end{aligned}
\]

所以

\[
\boxed{0<s_0<q_0.}
\tag{3.8}
\]

式 (3.5) 还直接给出

\[
\boxed{N_0=Jq_0+s_0.}
\tag{3.9}
\]

### 3.3 仿射恢复

GAL-2 的仿射恢复在本区域成为

\[
\boxed{q=q_0+B\Lambda y,}
\tag{3.10}
\]

\[
\boxed{s=s_0+(1+B\tau)y,}
\tag{3.11}
\]

\[
\boxed{N=N_0+ry,}
\tag{3.12}
\]

其中 \(y\in\mathbb Z_{\ge0}\)。由 (3.6)，这些式子与

\[
qr=1+B\Lambda N,
\qquad
N=Jq+s
\tag{3.13}
\]

双向等价。

---

## 4. 第一次二进下降

真实指数写为

\[
\boxed{N=2^e10^\mu,\qquad \mu=m-e\ge0.}
\tag{4.1}
\]

因为

\[
e=2a+\Delta+h=2a+\delta>2a,
\]

故

\[
\boxed{M=2^{2a}\mid N.}
\tag{4.2}
\]

由 \(r=1+BV\)、\(M\mid B\)，

\[
r\equiv1\pmod M.
\tag{4.3}
\]

由 (3.5) 及 \(M\mid K\)，

\[
N_0\equiv J+1\pmod M.
\tag{4.4}
\]

将 \(N=N_0+ry\) 模 \(M\)，得到

\[
\boxed{y\equiv-(J+1)\pmod M.}
\tag{4.5}
\]

因为 \(a\ge3\)，

\[
M\ge64>J+1,
\]

且 \(y\ge0\)，故唯一写成

\[
\boxed{y=Mz-(J+1),\qquad z\in\mathbb Z_{\ge1}.}
\tag{4.6}
\]

这里 \(z=1\) 完整保留；同时得到比 GAL-2 的一般端点更强的结论

\[
\boxed{y\ge M-10>0.}
\tag{4.7}
\]

因此浅正根中 \(y=0\) 实际不可能。

### 4.1 关键下降恒等式

由 (3.2)、(3.5) 与 \(B=K\Lambda\)，

\[
\begin{aligned}
N_0-(J+1)r
&=KV(\Lambda-\tau)-(J+1)BV\\
&=KV\{\Lambda-\tau-(J+1)\Lambda\}\\
&=-KV(J\Lambda+\tau).
\end{aligned}
\]

所以

\[
\boxed{N_0-(J+1)r=-KV^2.}
\tag{4.8}
\]

将 (4.6) 代入 \(N=N_0+ry\)：

\[
\begin{aligned}
N
&=Mzr+N_0-(J+1)r\\
&=M\{zr-5^\kappa V^2\}.
\end{aligned}
\]

故

\[
\boxed{\frac NM=zr-5^\kappa V^2.}
\tag{4.9}
\]

另一方面，(4.1) 与 \(e=2a+\delta\) 给

\[
\boxed{
\frac NM
=2^\delta10^\mu
=2^{\Delta+h+\mu}5^\mu.
}
\tag{4.10}
\]

于是全部指数状态被压成

\[
\boxed{
2^\delta10^\mu
=zr-5^\kappa V^2,
\qquad
z\ge1,\quad\mu\ge0,
}
\tag{4.11}
\]

其中

\[
\boxed{r=1+B V=1+M5^{2\varphi}V.}
\tag{4.12}
\]

式 (4.11) 就是不含 Hensel 树的核心指数正规形。

### 4.2 反向充分性

固定一个满足第 1、2 节局部门的

\[
(a,\Delta,h,J,\tau).
\]

任取 \(z\ge1,\mu\ge0\) 满足 (4.11)，定义

\[
y=Mz-(J+1).
\]

则 \(y\ge0\)，且 (4.8) 反向给出

\[
N_0+ry=M\,2^\delta10^\mu=2^e10^\mu.
\]

再由 (3.10)–(3.12) 唯一恢复 \(q,s,N\)，并自动满足 (3.13)。
此外，

\[
q-s
=(q_0-s_0)+\{B\Lambda-(1+B\tau)\}y
\]

而

\[
q_0-s_0=K(\Lambda-\tau)^2>0,
\]

\[
B\Lambda-(1+B\tau)
=B(\Lambda-\tau)-1>0.
\]

故

\[
0<s<q.
\]

又由 \(qr-B\Lambda N=1\)，

\[
\gcd(N,q)=\gcd(N,r)=1.
\]

所以 (4.11) 与原仿射终端候选严格双向，不只是必要同余。

---

## 5. 消去 \(y\) 后的显式多项式正规形

GAL-2 中

\[
L=\lambda+\Lambda y.
\]

代入 \(\lambda=\Lambda-\tau\) 与 \(y=Mz-(J+1)\)：

\[
\begin{aligned}
L
&=\Lambda-\tau+\Lambda\{Mz-(J+1)\}\\
&=M\Lambda z-(J\Lambda+\tau).
\end{aligned}
\]

因此

\[
\boxed{L=M\Lambda z-V.}
\tag{5.1}
\]

由 \(V<10\Lambda\)、\(M\ge64\)、\(z\ge1\)，

\[
L>0,
\qquad
L-V=M\Lambda z-2V>0.
\tag{5.2}
\]

全部终端量可直接写成

\[
\boxed{
\begin{aligned}
r&=1+BV,\\
q&=1+B(M\Lambda z-V),\\
s&=Mz-J+K\tau(M\Lambda z-V),\\
N&=M\{zr-5^\kappa V^2\}.
\end{aligned}
}
\tag{5.3}
\]

其中 \(s\) 的公式来自

\[
\Lambda s=\tau+L+BL\tau
\]

及 \(B=K\Lambda\)。式 (5.3) 是完全显式的多项式—指数正规形；
自由变量只剩 \(\tau,\mu,z\)，而 \(z\) 将在第 7 节由 \(\mu\) 唯一恢复。

---

## 6. 共轭和差、互素性与符号

由 (5.1)，

\[
\boxed{q=1+B(M\Lambda z-V),}
\tag{6.1}
\]

而 \(r=1+BV\)。所以

\[
\boxed{q+r=2+BM\Lambda z,}
\tag{6.2}
\]

\[
\boxed{q-r=B(M\Lambda z-2V).}
\tag{6.3}
\]

由 (5.2)，

\[
\boxed{q-r>0,\qquad q>r.}
\tag{6.4}
\]

因此 \(q=r\) 不可能。

置

\[
W=M\Lambda z-2V.
\tag{6.5}
\]

因为 \(V\) 为奇数、\(M\Lambda z\) 被 \(4\) 整除，

\[
\boxed{v_2(W)=1.}
\tag{6.6}
\]

又因 \(5\mid\Lambda\)、\(5\nmid V\)，

\[
\boxed{v_5(W)=0.}
\tag{6.7}
\]

故和差具有精确赋值

\[
\boxed{
v_2(q-r)=2a+1,
\qquad
v_5(q-r)=2\varphi,
}
\tag{6.8}
\]

\[
\boxed{
v_2(q+r)=1,
\qquad
v_5(q+r)=0.
}
\tag{6.9}
\]

同时

\[
\gcd(q,B\Lambda)=\gcd(r,B\Lambda)=1.
\tag{6.10}
\]

但 \(q,r\) 之间没有由现有恒等式强迫出的统一互素性。准确公式是

\[
\boxed{
\gcd(q,r)
=\gcd\bigl(r,M\Lambda z-2V\bigr),
}
\tag{6.11}
\]

因为 \(q-r=BW\) 且 \(\gcd(r,B)=1\)。右端仍随 \(z,V,r\) 移动；
它只说明 \(\gcd(q,r)\) 与 \(10\) 互素，不给固定因子分解。

---

## 7. 每个状态至多一条完整指数级数

将 (4.11) 改写为

\[
rz=5^\kappa V^2+2^\delta10^\mu.
\tag{7.1}
\]

因为

\[
\gcd(r,10V)=1,
\]

式 (7.1) 模 \(r\) 严格等价于

\[
\boxed{
10^\mu
\equiv
-2^{-\delta}5^\kappa V^2
\pmod r.
}
\tag{7.2}
\]

定义

\[
\boxed{P_r=\operatorname{ord}_r(10),}
\tag{7.3}
\]

以及单位

\[
c_r=\left\langle-2^{-\delta}5^\kappa V^2\right\rangle_r.
\tag{7.4}
\]

若

\[
c_r\notin\langle10\rangle
\subset(\mathbb Z/r\mathbb Z)^\times,
\]

则该整个 \((a,\Delta,h,J,\tau)\) 状态为空。

若 \(c_r\in\langle10\rangle\)，则存在唯一

\[
\mu_0\in\{0,\ldots,P_r-1\}
\]

满足

\[
10^{\mu_0}\equiv c_r\pmod r,
\]

并且全部非负整数解恰为

\[
\boxed{\mu=\mu_0+tP_r,\qquad t\in\mathbb Z_{\ge0}.}
\tag{7.5}
\]

这已经证明：

\[
\boxed{
\text{每个固定浅正根局部状态至多有一条指数递推，不存在多分支指数树。}
}
\tag{7.6}
\]

一旦 \(\mu\) 确定，\(z\) 唯一为

\[
\boxed{
z=\frac{5^\kappa V^2+2^\delta10^\mu}{r}.
}
\tag{7.7}
\]

因此不需要再枚举 \(z\)。

### 7.1 精确下端

由 \(V<10\Lambda<M\Lambda\)，

\[
\begin{aligned}
D_0
&:=r-5^\kappa V^2\\
&=1+5^\kappa V(M\Lambda-V)>0.
\end{aligned}
\tag{7.8}
\]

特别地

\[
0<\frac{5^\kappa V^2}{r}<1.
\tag{7.9}
\]

若 (7.1) 有整数 \(z\ge1\)，则必须有

\[
2^\delta10^\mu\ge D_0.
\]

定义完全整数化的下端

\[
\boxed{
\mu_{\min}
=\min\{u\in\mathbb Z_{\ge0}:2^\delta10^u\ge D_0\}.
}
\tag{7.10}
\]

若需要只用整数商表示，可先置

\[
R_0=\left\lceil\frac{D_0}{2^\delta}\right\rceil,
\]

再取最小的 \(u\ge0\) 使 \(10^u\ge R_0\)。

### 7.2 严格大小门与 \(\mu_{\max}\)

继承大小门为

\[
20\cdot10^m<194029Z^2Y,
\qquad
Z=\frac{B\Lambda}{2},
\qquad
Y=10^{3a},
\qquad
m=e+\mu.
\tag{7.11}
\]

定义整数

\[
\mathscr X=194029Z^2Y,
\tag{7.12}
\]

\[
\boxed{
Q_\mu
=
\left\lfloor
\frac{\mathscr X-1}{20\cdot10^e}
\right\rfloor.
}
\tag{7.13}
\]

若 \(Q_\mu<1\)，该状态整体为空。否则定义

\[
\boxed{
\mu_{\max}
=\max\{u\in\mathbb Z_{\ge0}:10^u\le Q_\mu\}.
}
\tag{7.14}
\]

这完全等价于严格大小门，并满足相邻端点核对

\[
\boxed{
20\cdot10^{e+\mu_{\max}}
<\mathscr X
\le
20\cdot10^{e+\mu_{\max}+1}.
}
\tag{7.15}
\]

### 7.3 完整有限指数段

若离散对数存在，定义

\[
t_{\min}
=
\max\left(
0,
\left\lceil\frac{\mu_{\min}-\mu_0}{P_r}\right\rceil
\right),
\tag{7.16}
\]

\[
t_{\max}
=
\left\lfloor
\frac{\mu_{\max}-\mu_0}{P_r}
\right\rfloor.
\tag{7.17}
\]

若 \(t_{\min}>t_{\max}\)，该状态为空；否则全部指数恰为

\[
\boxed{
\mu=\mu_0+tP_r,
\qquad
t_{\min}\le t\le t_{\max},
}
\tag{7.18}
\]

并由 (7.7)、(4.6)、(5.3) 唯一恢复 \(z,y,q,s,N\)。

这是一条完整有限同余段，不是有限 \(\mu\) 前缀外推。

### 7.4 \(z\) 的严格区间与端点修正

由 (7.1)，

\[
\boxed{
\frac{5^\kappa V^2}{r}<z.
}
\tag{7.19}
\]

结合 (7.9)，这只给 \(z\ge1\)，且 \(z=1\) 必须保留。

对 \(\mu\le\mu_{\max}\)，准确的整数上界是

\[
\boxed{
z
\le
z_{\max}
:=
\left\lfloor
\frac{5^\kappa V^2+2^\delta10^{\mu_{\max}}}{r}
\right\rfloor.
}
\tag{7.20}
\]

这里不能把 \(\le\) 改成严格 \(<\)：当 \(\mu=\mu_{\max}\) 且整除成立时，
等号可以发生。若要求严格实数上界，应直接使用原大小门：

\[
\boxed{
z
<
\frac{
5^\kappa V^2+
2^\delta\mathscr X/(20\cdot10^e)
}{r}.
}
\tag{7.21}
\]

所以题设中以 \(\mu_{\max}\) 写出的上端必须审计为非严格端点；这不是
GAL-2 的继承错误。

---

## 8. \(z\) 的完整二进数字

由 (4.11)，

\[
zr\equiv5^\kappa V^2
\pmod{2^{\delta+\mu}}.
\]

因 \(r\) 为奇数，实际上有比题设截断式更强的完整数字

\[
\boxed{
z
\equiv
5^\kappa V^2r^{-1}
\pmod{2^{\delta+\mu}}.
}
\tag{8.1}
\]

现在定义

\[
\boxed{g=\min(\delta+\mu,2a).}
\tag{8.2}
\]

由 \(r\equiv1\pmod{2^{2a}}\)，(8.1) 降为

\[
\boxed{
z\equiv5^\kappa V^2\pmod{2^g}.
}
\tag{8.3}
\]

因为 \(V\) 为奇数，右端是奇数，所以其标准代表严格位于

\[
\boxed{\{1,3,\ldots,2^g-1\};}
\tag{8.4}
\]

不存在标准代表 \(0\) 或上端 \(2^g\) 的歧义。

必须区分：

1. 若 \(\delta+\mu<2a\)，则 (8.3) 给出长度
   \(2^{\delta+\mu}\) 的完整当前低位；
2. 若 \(\delta+\mu\ge2a\)，则
   \[
   \boxed{z\equiv5^\kappa V^2\pmod M}
   \]
   唯一锁定完整低 \(M\)-进数字。

超过 \(M\) 后也不需要二进 Hensel 树。若令 \(n_2=\delta+\mu\)，则

\[
r^{-1}
\equiv
\sum_{j=0}^{\lfloor(n_2-1)/(2a)\rfloor}
(-BV)^j
\pmod{2^{n_2}},
\tag{8.5}
\]

所以 (8.1) 是一个显式有限几何多项式。将其标准代表与
\(1\le z\le z_{\max}\) 相交，只留下有限个二进走廊；但
\(z_{\max}/2^{\delta+\mu}\) 没有统一小于 1，故不能由此推出
每个外层状态至多一个 \(\mu\) 或推出 \(\Delta\) 绝对有界。

---

## 9. \(z\) 的五进赋值走廊

式 (7.1) 为

\[
zr=5^\kappa V^2+5^\mu2^{\delta+\mu},
\tag{9.1}
\]

其中

\[
r\equiv1\pmod{5^{2\varphi}},
\qquad
5\nmid V.
\tag{9.2}
\]

### 9.1 第一室：\(\mu<\kappa\)

从 (9.1) 提出 \(5^\mu\)：

\[
zr
=5^\mu
\left(
2^{\delta+\mu}+5^{\kappa-\mu}V^2
\right).
\]

括号模 5 是非零的 \(2^{\delta+\mu}\)，故

\[
\boxed{v_5(z)=\mu.}
\tag{9.3}
\]

写

\[
z=5^\mu z_0,
\qquad5\nmid z_0.
\]

则

\[
z_0r
=2^{\delta+\mu}+5^{\kappa-\mu}V^2.
\tag{9.4}
\]

因为

\[
1\le\kappa-\mu<2\varphi,
\]

由 (9.2) 精确得到

\[
\boxed{
z_0\equiv2^{\delta+\mu}
\pmod{5^{\kappa-\mu}}.
}
\tag{9.5}
\]

### 9.2 第二室：\(\mu>\kappa\)

从 (9.1) 提出 \(5^\kappa\)：

\[
zr
=5^\kappa
\left(
V^2+5^{\mu-\kappa}2^{\delta+\mu}
\right).
\]

括号模 5 为 \(V^2\ne0\)，故

\[
\boxed{v_5(z)=\kappa.}
\tag{9.6}
\]

写

\[
z=5^\kappa z_0,
\qquad5\nmid z_0.
\]

则

\[
z_0r
=V^2+5^{\mu-\kappa}2^{\delta+\mu},
\tag{9.7}
\]

从而有完整低位

\[
\boxed{
z_0
\equiv
V^2r^{-1}
\pmod{5^{\mu-\kappa}}.
}
\tag{9.8}
\]

特别地，若

\[
n_5=\min(\mu-\kappa,2\varphi),
\]

则

\[
\boxed{z_0\equiv V^2\pmod{5^{n_5}}.}
\tag{9.9}
\]

超过精度 \(2\varphi\) 后同样不需要 Hensel 树。因为
\(v_5(r-1)=2\varphi\)，

\[
r^{-1}
\equiv
\sum_{j=0}^{\lfloor(\mu-\kappa-1)/(2\varphi)\rfloor}
(-BV)^j
\pmod{5^{\mu-\kappa}}.
\tag{9.10}
\]

所以 (9.8) 仍是显式有限几何多项式数字。

### 9.3 同层：\(\mu=\kappa\)

此时必须保留同层消去：

\[
\boxed{
zr
=5^\kappa
\left(
V^2+2^{\delta+\kappa}
\right).
}
\tag{9.11}
\]

定义

\[
\boxed{
t_5
=v_5\left(V^2+2^{\delta+\kappa}\right).
}
\tag{9.12}
\]

则

\[
\boxed{v_5(z)=\kappa+t_5.}
\tag{9.13}
\]

额外提升的首层条件可以完全判定。由 \(V\equiv2\) 或 \(3\pmod5\)，

\[
V^2\equiv4\pmod5.
\]

所以

\[
t_5\ge1
\iff
2^{\delta+\kappa}\equiv1\pmod5
\iff
\delta+\kappa\equiv0\pmod4.
\]

而

\[
\delta+\kappa
=\Delta+h+2a-5\Delta
=2a-4\Delta+h,
\]

故

\[
\boxed{
t_5\ge1
\iff
2a+h\equiv0\pmod4.
}
\tag{9.14}
\]

若该同余不成立，则 \(t_5=0\)。若成立，额外提升仍不是分支树；对固定
\(V\)，\(t_5\) 就是单个显式整数，并满足

\[
0\le t_5
\le
\left\lfloor
\log_5\left(V^2+2^{\delta+\kappa}\right)
\right\rfloor.
\tag{9.15}
\]

更精确地，

\[
t_5\ge n
\iff
V^2\equiv-2^{\delta+\kappa}\pmod{5^n}.
\tag{9.16}
\]

写

\[
z=5^{\kappa+t_5}z_0,
\qquad5\nmid z_0,
\]

则候选必须且只须满足

\[
\boxed{
z_0r
=
\frac{V^2+2^{\delta+\kappa}}{5^{t_5}}.
}
\tag{9.17}
\]

特别地，由 \(5\nmid r\)，同层候选要求

\[
\boxed{r\mid V^2+2^{\delta+\kappa}.}
\tag{9.18}
\]

三室 (9.3)、(9.6)、(9.13) 穷尽全部 \(\mu\)，没有把同层消去错误并入
前两室。

---

## 10. 边界 \(\kappa=0\)

边界条件为

\[
2\varphi=3\Delta
\iff
2a=5\Delta.
\tag{10.1}
\]

因为 \(\gcd(2,5)=1\)，存在唯一整数 \(u\ge1\) 使

\[
\boxed{
a=5u,
\qquad
\Delta=2u,
\qquad
\varphi=3u.
}
\tag{10.2}
\]

所以该边界是一条无界整数射线，不是有限小端。

此时

\[
\boxed{K=M,\qquad C=\Lambda,\qquad B=M\Lambda.}
\tag{10.3}
\]

核心方程化为

\[
\boxed{
\frac NM
=2^\delta10^\mu
=zr-V^2.
}
\tag{10.4}
\]

又因 \(M\Lambda=B\)，

\[
\boxed{q+r=2+B^2z,}
\tag{10.5}
\]

\[
\boxed{q-r=B(Bz-2V)>0.}
\tag{10.6}
\]

二进数字变为

\[
z\equiv V^2\pmod{2^{\min(\delta+\mu,2a)}}.
\tag{10.7}
\]

五进分室只剩：

- \(\mu>0\) 时，\(v_5(z)=0\)，且
  \[
  z\equiv V^2r^{-1}\pmod{5^\mu};
  \]
- \(\mu=0\) 时，这是同层，
  \[
  v_5(z)=v_5(V^2+2^\delta),
  \]
  额外提升当且仅当 \(\delta\equiv0\pmod4\)。

这些关系均与 \(z\ge1\)、\(q>r\) 和大小门相容。现有链条没有在
\(\kappa=0\) 上产生额外因式分解、奇偶矛盾或绝对边界；因此该无界射线
保持开放。

---

## 11. 平方路线的完整复核

由 (6.2)–(6.3)，形式上有

\[
(q-r)^2=(q+r)^2-4qr.
\tag{11.1}
\]

代入

\[
q+r=2+BM\Lambda z,
\qquad
qr=1+B\Lambda N,
\]

以及

\[
N=M(zr-5^\kappa V^2),
\qquad
B=M5^\kappa\Lambda,
\]

逐项展开：

\[
\begin{aligned}
(q+r)^2-4qr
&=(2+BM\Lambda z)^2-4(1+B\Lambda N)\\
&=B^2(M\Lambda z-2V)^2.
\end{aligned}
\]

所以

\[
\boxed{
(q+r)^2-4qr
=B^2(M\Lambda z-2V)^2
=(q-r)^2.
}
\tag{11.2}
\]

这只是由 (4.11) 回代得到的恒等式，不是新的平方判别门。

两个归一化因子

\[
M\Lambda z,
\qquad
M\Lambda z-2V
\]

的 gcd 仍含移动的 \(\gcd(z,V)\) 信息；(6.6)–(6.9) 只固定了
\((2,5)\)-赋值，没有给固定小差因子、统一奇素数或严格大小间隙。
因此无法仿照 \(\mathcal F_+\) 得到三层终端因子矛盾。

---

## 12. 完整生成顺序

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
   K=M5^\kappa,
   \quad
   B=K\Lambda.
   \]
4. 取 \(J\in\{1,\ldots,9\}\) 及一个符号状态
   \[
   0<\tau<\Lambda,
   \quad
   \tau\equiv2,3\pmod5,
   \quad
   J+\tau\equiv1\pmod2.
   \]
   不进行逐位 Hensel 生成；直接置
   \[
   \lambda=\Lambda-\tau,
   \quad
   V=J\Lambda+\tau.
   \]
5. 构造 (3.2)–(3.5)，或直接使用显式正规形 (5.3)。
6. 计算 \(P_r=\operatorname{ord}_r(10)\)，检查 (7.2)。若无离散对数，
   删除整个状态；若有，按 (7.18) 生成唯一完整有限指数段。
7. 对每个指数用 (7.7) 唯一恢复 \(z\)，再恢复 \(y,q,s,N,L\)。
8. 最后进入继承的十三首块、\(a_2\) 窗口、判别式平方、两个恢复符号、
   精确 gcd 尺度、\(a_3\) 窗口、三个逐项既约及原题直接回代。

第 1–7 步在终端层严格双向；第 8 步仍是完整原题候选不可省略的恢复门。
本文没有把终端状态误报为合法六元组。

---

## 13. 主动审计

### 13.1 \(\tau=0\)

它是整个补数 involution 的固定点，但违反
\(\tau\equiv2,3\pmod5\)，所以在允许状态进入本文之前已被删除。

### 13.2 \(\lambda_\tau=0\)

由 \(\lambda_\tau=\Lambda-\tau\) 与 \(0<\tau<\Lambda\)，不可能发生。

### 13.3 \(\lambda_\tau=\tau\)

在正标准代表区间中会给 \(2\tau=\Lambda\)，与 \(\Lambda\) 为奇数矛盾。
模环中的另一固定点表述只产生 \(\tau=0\)，已由 13.1 删除。

### 13.4 \(\kappa=0\)

第 10 节完整保留无界射线
\((a,\Delta,\varphi)=(5u,2u,3u)\)，没有把它当作有限边界。

### 13.5 \(z=1\)

没有先验删除。它严格等价于

\[
2^\delta10^\mu
=r-5^\kappa V^2
=1+5^\kappa V(M\Lambda-V),
\]

并由唯一指数段决定是否发生。

### 13.6 \(\mu=0\)

完整包含在 (7.2) 与大小端点中。若 \(\kappa>0\)，它属于
\(\mu<\kappa\) 室；若 \(\kappa=0\)，它恰是同层室。

### 13.7 \(\mu=\kappa\)

第 9.3 节单独保留额外提升 \(t_5\)，没有套用前后两室的赋值公式。

### 13.8 \(y=0\)

由 \(y=Mz-(J+1)\)、\(z\ge1\)、\(M>J+1\)，严格不可能。

### 13.9 \(q=r\)

由 \(q-r=B(M\Lambda z-2V)>0\)，严格不可能。

### 13.10 \(q-r\) 的符号

因 \(M\Lambda z\ge64\Lambda>20\Lambda>2V\)，始终为正。

### 13.11 \(s_0>0\)

\(s_0=1+K\tau(\Lambda-\tau)>0\)，且
\(q_0-s_0=K(\Lambda-\tau)^2>0\)。

### 13.12 二进标准代表端点

右端 \(5^\kappa V^2\) 为奇数，所以模 \(2^g\) 的标准代表既不是 0，
也不取上端 \(2^g\)。

### 13.13 五进同层消去

额外赋值恰为 \(t_5=v_5(V^2+2^{\delta+\kappa})\)；首层提升条件是
\(2a+h\equiv0\pmod4\)。

### 13.14 大小门严格端点

严格不等式由 \((\mathscr X-1)/(20\cdot10^e)\) 下取整处理。
以 \(\mu_{\max}\) 写出的 \(z\) 上端必须使用 \(\le\)，严格上端应使用
(7.21)。

### 13.15 involution 退化的能力边界

补数公式只删除了 Hensel 树；它没有删除任一合法 \(\tau\)，也没有直接关闭
浅正根区域。每个 \(J\) 仍有 \(5^{3\Delta-1}\) 个符号状态，且
\(r\)、\(P_r\) 随外层参数移动。

---

## 14. 为什么不能升级为关闭或绝对有限化

本轮没有得到 GALS+-1，原因是：

1. 二进数字 (8.1) 与三个五进走廊彼此 CRT 相容；
2. \(z\) 的大小区间没有统一短于完整二进或五进模数；
3. 平方路线 (11.2) 是已有终端方程的恒等回代；
4. \(\gcd(q,r)\) 仍由移动量 \(M\Lambda z-2V\) 控制；
5. \(\kappa=0\) 无界射线没有产生额外矛盾。

本轮没有得到 GALS+-2，原因是 \(a,\Delta\) 未被压到绝对有限范围。

本轮没有得到 GALS+-4，因为 \(\kappa>0\) 与 \(\kappa=0\) 均未统一关闭。

但本轮严格超过“仅退化 involution”的层级：每个固定
\((a,\Delta,h,J,\tau)\) 已经至多只剩一条显式指数递推，并由大小门截成
完整有限段；每个指数又只对应一个显式 \(z\)。因此准确达到 GALS+-3。

由于残余仍随 \(a,\Delta,\tau,r\) 无界，本文不生成伪造的有限证书，
也不以任何有限 \(a\) 或 \(\Delta\) 前缀外推。

---

## 15. 最终分类与停止点

本轮严格建立

\[
\boxed{
\begin{gathered}
B=K\Lambda,
\qquad
\lambda_\tau=\Lambda-\tau,\\
r=1+BV,
\qquad
q_0=1+B(\Lambda-\tau),\\
s_0=1+K\tau(\Lambda-\tau),\\
N_0=J+1+KV(\Lambda-\tau),\\
q_0r=1+B\Lambda N_0,
\qquad
N_0=Jq_0+s_0,
\qquad
0<s_0<q_0,\\
y=Mz-(J+1),
\qquad
z\ge1,\\
N_0-(J+1)r=-KV^2,\\
2^\delta10^\mu=zr-5^\kappa V^2,\\
L=M\Lambda z-V,\\
q+r=2+BM\Lambda z,\\
q-r=B(M\Lambda z-2V)>0,\\
10^\mu\equiv-2^{-\delta}5^\kappa V^2\pmod r,\\
\mu=\mu_0+t\operatorname{ord}_r(10),
\qquad
t_{\min}\le t\le t_{\max},\\
z=\dfrac{5^\kappa V^2+2^\delta10^\mu}{r}.
\end{gathered}
}
\tag{15.1}
\]

全部二进数字由 (8.1) 显式给出；全部五进赋值由
\(\mu<\kappa\)、\(\mu>\kappa\)、\(\mu=\kappa\) 三室穷尽。
因此本区域已经完全脱离 GAL-2 的 Hensel 树，并压成每状态至多一条有限指数段。

但外层 \((a,\Delta)\)、补数状态 \(\tau\)、移动模数 \(r\) 与阶
\(\operatorname{ord}_r(10)\) 仍无界；平方和差与 \(\kappa=0\) 边界均未产生
统一矛盾。因此最终分类为

\[
\boxed{
\mathrm{GALS{+}\text{-}3}.
}
\]

本文到此停止，不研究浅负根、真正深区、高 \(\varphi\) 的
\(\mathcal F_{P-}\)、B、C、\(\gamma>1\)、C2/C5、Q 或严格层。
