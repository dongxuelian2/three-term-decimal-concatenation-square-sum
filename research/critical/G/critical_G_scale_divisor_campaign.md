# 三项十进制拼接平方和问题：临界 \(G\) 模板本原尺度—约数分配报告

## 1. PR6 后的本原系统

本文只研究临界层

\[
(\delta_2,\delta_3)=(-1,1),\qquad N_L=1
\]

中 \(G\) 模板的本原正余数层

\[
\boxed{h=1}.
\]

按本轮约定，暂时接受 T1–T18、K5、CG、E4、GT4、VA1、GD1、
GP3、CD6 和 PR6，不作整个项目的统一独立审计。特别地，

\[
J\in\{1,\ldots,9\},\qquad q\ge3,
\]

\[
T=\tau N,\qquad b_2=\tau q,\qquad
\tau=\frac{b_1u}{v},
\]

\[
N=Jq+s,\qquad 1\le s<q,\qquad
\gcd(N,q)=\gcd(s,q)=1,
\]

\[
d=\gcd(g,E),\qquad g=d\gamma,\qquad E=dE_0,
\]

\[
q\rho_0-E_0s=\gamma,\qquad
qM_0-E_0N=\gamma,
\]

\[
E_0=b_1Z,\qquad
\gamma(qk-1)=Z(q+b_1N),
\tag{1.1}
\]

\[
Z=\frac{Y}{vd},\qquad
\gamma\mid q+b_1N,\qquad
\gamma<21q.
\tag{1.2}
\]

这里

\[
T=10^m,\qquad Y=10^n,\qquad m\ge2,\quad n\ge1,
\]

\[
u=2^c5^e,\qquad
g=2^a5^\varphi g_\ast,\qquad a\ge1,\quad \gcd(g_\ast,10)=1,
\]

\[
b_2=\frac{b_1qu}{v},\qquad
b_3=b_1d\gamma u,
\tag{1.3}
\]

\[
\frac T{10}\le b_2<T,\qquad
\frac Y{10}\le b_3<Y.
\tag{1.4}
\]

K5 的互素和支撑门、十三种首块、E4 的全部高阶参数及三个逐项既约
条件均原样保留。特别地，

\[
(a_1,b_1)\in
\{(1,1),\ldots,(8,1)\}
\cup
\{(5,2),(7,2),(9,2),(11,2),(13,2)\},
\tag{1.5}
\]

\[
10^{m-2}\le a_2<10^{m-1},\qquad
Y\le a_3<10Y.
\tag{1.6}
\]

定义

\[
\boxed{
A=vZH_1,\qquad
H_1=a_1T+10a_2,
}
\tag{1.7}
\]

\[
\boxed{
\mathcal R=(ua_1)^2+(va_2)^2,\qquad
K=k^2-1.
}
\tag{1.8}
\]

PR6 的约化判别式是

\[
\boxed{
w_0^2=A^2-K\gamma^2\mathcal R,
}
\tag{1.9}
\]

其中 \(w_0\in\mathbb Z_{\ge0}\)，且 \(k>1\)、\(K>0\)。本轮只使用
三个阶段，每阶段三个核心新引理：

- 阶段 I：SD-I.1–SD-I.3，共轭因子与互补尺度；
- 阶段 II：SD-II.1–SD-II.3，\(2,5\) 及非十进制奇素数分配；
- 阶段 III：SD-III.1–SD-III.3，第三块窗口、完整恢复与停止点。

本轮最终分类为

\[
\boxed{\mathrm{SD6}},
\]

但附带严格关闭了此前开放的整个五进尺度溢出

\[
\boxed{v_5(g)>n}.
\]

该附带关闭不等于关闭 \(\gamma>1\)：\(\gamma\) 仍可含二进溢出或
非十进制奇核心。

---

## 2. 共轭因子恒等式

### 2.1 阶段 I 核心引理 SD-I.1：乘积、和差与符号

定义

\[
\boxed{
L_+=A+kw_0,\qquad L_-=A-kw_0,
}
\tag{2.1}
\]

\[
\boxed{
Q=k^2\gamma^2\mathcal R-A^2.
}
\tag{2.2}
\]

由 (1.9)，

\[
\begin{aligned}
L_+L_-
&=A^2-k^2w_0^2\\
&=A^2-k^2(A^2-K\gamma^2\mathcal R)\\
&=K(k^2\gamma^2\mathcal R-A^2).
\end{aligned}
\]

因此

\[
\boxed{L_+L_-=KQ.}
\tag{2.3}
\]

同时直接有

\[
\boxed{
L_++L_-=2A,\qquad
L_+-L_-=2kw_0.
}
\tag{2.4}
\]

还有一个对符号审计很重要的等式：

\[
\boxed{
Q=\gamma^2\mathcal R-w_0^2.
}
\tag{2.5}
\]

这是因为 \(A^2=w_0^2+K\gamma^2\mathcal R\) 且 \(k^2-K=1\)。
由 \(\mathcal R>0\)、\(K>0\)，

\[
0\le w_0<A.
\tag{2.6}
\]

所以

\[
L_+>0
\]

恒成立，而由 (2.3)

\[
\boxed{
\operatorname{sgn}(L_-)=\operatorname{sgn}(Q).
}
\tag{2.7}
\]

特别地：

- \(Q<0\) 时只能保留 \(L_+\)；
- \(Q=0\) 时 \(L_-=0\)，仍只能保留 \(L_+\)；
- \(Q>0\) 时两个共轭因子都为正，但两个恢复符号仍须分别检查整性、
  窗口与既约性。

因此不能预设 \(Q>0\)，也不能把两个共轭因子都默认为正。

### 2.2 一个负 \(Q\) 与一个零 \(Q\) 的算术反例

这些数据不冒充原题候选，只用于攻击错误符号加强。

取

\[
A=5,\quad k=3,\quad K=8,\quad
\gamma=1,\quad\mathcal R=2,\quad w_0=3.
\]

则

\[
w_0^2=A^2-K\gamma^2\mathcal R=9,
\]

\[
Q=9\cdot2-25=-7,\qquad
(L_+,L_-)=(14,-4).
\]

而

\[
d=\frac8{\gcd(8,14)}=4,\qquad
a_3=\frac{14}{\gcd(8,14)}=7.
\]

所以这一共轭—恢复算术状态同时满足

\[
d^2=16\nmid K=8.
\]

它还显示 \(d\) 与 \(K/d\) 可以共享素数 \(2\)。

再取

\[
A=15,\quad k=3,\quad K=8,\quad
\gamma=1,\quad\mathcal R=25,\quad w_0=5.
\]

则

\[
Q=0,\qquad (L_+,L_-)=(30,0),
\]

\[
d=4,\qquad a_3=15.
\]

所以 \(Q=0\) 也不能在纯共轭层被删除。

---

## 3. 互补尺度分配

### 3.1 阶段 I 核心引理 SD-I.2：两个尺度的精确互补

固定一个满足

\[
L_\varepsilon>0,\qquad \varepsilon\in\{+1,-1\}
\]

并约定 \(L_\varepsilon=A+\varepsilon kw_0\)。假设该符号恢复合法
第三块。PR-III.2 给出

\[
a_3=\frac{L_\varepsilon}{\gcd(K,L_\varepsilon)},
\qquad
d=\frac K{\gcd(K,L_\varepsilon)}.
\tag{3.1}
\]

因此

\[
\gcd(K,L_\varepsilon)=\frac Kd,
\]

并且

\[
\boxed{
L_\varepsilon=\frac Kd\,a_3.
}
\tag{3.2}
\]

由 (2.3)，

\[
\frac Kd\,a_3L_{-\varepsilon}=KQ,
\]

故

\[
\boxed{
L_{-\varepsilon}=\frac{dQ}{a_3}.
}
\tag{3.3}
\]

第三块既约性和 (1.3) 给出

\[
\boxed{
\gcd(a_3,d\gamma ub_1)=1.
}
\tag{3.4}
\]

特别地 \(\gcd(a_3,d)=1\)。由 (3.3) 中

\[
a_3L_{-\varepsilon}=dQ
\]

立即推出

\[
\boxed{a_3\mid Q.}
\tag{3.5}
\]

定义新的第三块共轭商

\[
\boxed{Q=a_3\mathscr R_3.}
\tag{3.6}
\]

这里 \(\mathscr R_3\) 不表示 GT4 中曾使用的尾余项 \(b_3/v\)。
于是

\[
\boxed{
L_{-\varepsilon}=d\mathscr R_3.
}
\tag{3.7}
\]

所以完整互补分配是

\[
\boxed{
\frac Kd\mid L_\varepsilon,\qquad
d\mid L_{-\varepsilon}.
}
\tag{3.8}
\]

把 (3.2)、(3.7) 代入 (2.4)，还得到本轮真正新增的线性恒等式

\[
\boxed{
\frac Kd\,a_3+d\mathscr R_3=2A,
}
\tag{3.9}
\]

\[
\boxed{
\varepsilon\left(
\frac Kd\,a_3-d\mathscr R_3
\right)=2kw_0.
}
\tag{3.10}
\]

因 \(dA=YH_1\)，(3.9) 等价于

\[
\boxed{
Ka_3+d^2\mathscr R_3=2YH_1.
}
\tag{3.11}
\]

这比单独的尺度唯一性更强：\(d\) 与 \(K/d\) 被送入两个共轭因子，
而第三块同时整除 \(Q\)。

### 3.2 阶段 I 核心引理 SD-I.3：共享素数只能穿过 \(2A\)

对任意素数 \(p\)，记

\[
\delta_p=v_p(d),\qquad
\kappa_p=v_p(K).
\]

约定 \(v_p(0)=+\infty\)。由 (3.8)，

\[
v_p(L_\varepsilon)\ge\kappa_p-\delta_p,
\qquad
v_p(L_{-\varepsilon})\ge\delta_p.
\tag{3.12}
\]

而两个因子之和为 \(2A\)，故

\[
v_p(2A)
=v_p(L_\varepsilon+L_{-\varepsilon})
\ge
\min\bigl(v_p(L_\varepsilon),v_p(L_{-\varepsilon})\bigr).
\]

所以

\[
\boxed{
\min(\delta_p,\kappa_p-\delta_p)\le v_p(2A).
}
\tag{3.13}
\]

由于

\[
\boxed{
A=\frac{YH_1}{d},
}
\tag{3.14}
\]

对 \(p=2,5\) 有精确式

\[
\boxed{
v_p(2A)=v_p(2)+n+v_p(H_1)-\delta_p.
}
\tag{3.15}
\]

若记右端为 \(B_p\)，则 (3.13) 的几何意义是

\[
\boxed{
\delta_p\le B_p
\quad\text{或}\quad
\kappa_p-\delta_p\le B_p.
}
\tag{3.16}
\]

因此 \(d\) 的 \(p\)-指数只能落在 \(0\) 端或 \(\kappa_p\) 端的两个
移动“领圈”中；当 \(\kappa_p>2B_p\) 时，中间开区间

\[
B_p<\delta_p<\kappa_p-B_p
\]

被删除。

但这不能关闭 \(d\) 接近 \(K\) 的状态。事实上，当
\(\delta_p>\kappa_p/2\) 且 \(p\mid d\) 时，由 (3.2)、(3.4)

\[
v_p(L_\varepsilon)=\kappa_p-\delta_p
<
v_p(L_{-\varepsilon}),
\]

于是反而有精确等式

\[
\boxed{
\kappa_p-\delta_p=v_p(2A).
}
\tag{3.17}
\]

所以“\(d\) 接近 \(K\)”不是矛盾，而是把互补指数精确钉在 \(2A\)
的赋值上。式 (3.13) 只排除两个尺度同时含有超过 \(v_p(2A)\) 的
高次公共 \(p\)-幂。

---

## 4. 二进部分

### 4.1 阶段 II 核心引理 SD-II.1：\(K\) 的二进分配与 E4 字典

因为 \(k\) 为奇数，

\[
\gcd(k-1,k+1)=2
\]

并且

\[
\boxed{
\{v_2(k-1),v_2(k+1)\}=\{1,\nu\},
\qquad \nu\ge2.
}
\tag{4.1}
\]

故

\[
\boxed{v_2(K)=1+\nu.}
\tag{4.2}
\]

记

\[
\delta_2=v_2(d),\qquad \kappa_2=v_2(K).
\]

本原 A、B、C 室中 \(\delta_2\) 的精确表为

\[
\boxed{
\begin{array}{c|c}
\text{E4 室}&\delta_2\\ \hline
\mathrm A&a\\
\mathrm B\text{ 的全部本原行}&a\\
\mathrm{C1}&\min(a,n)\\
\mathrm{C2},\mathrm{C3}&a
\end{array}}
\tag{4.3}
\]

这里同时使用了 E4 的 \(n\)-关系和 PR6 的 \(d\mid Y/v\)。
特别地，

\[
\delta_2\ge1,
\]

所以 \(a_3\) 必为奇数。由 (3.2) 因而得到精确值

\[
\boxed{
v_2(L_\varepsilon)=\kappa_2-\delta_2.
}
\tag{4.4}
\]

设 \(\sigma_2\in\{\pm1\}\) 是使

\[
v_2(k-\sigma_2)=\nu
\]

的唯一符号。若 \(\delta_2\ge2\)，由
\(\delta_2\le1+\nu\) 只能推出

\[
\nu\ge\delta_2-1,
\qquad
k\equiv\sigma_2\pmod{2^{\delta_2-1}},
\tag{4.5}
\]

而不是 \(k\equiv\sigma_2\pmod{2^{\delta_2}}\)。

E4 的参数

\[
\lambda=v_2(kq-1)
\]

满足：若 \(\lambda<\nu\)，则

\[
\boxed{
\lambda=v_2(\sigma_2q-1);
}
\tag{4.6}
\]

若 \(\lambda\ge\nu\)，则必须有

\[
\boxed{
q\equiv\sigma_2\pmod{2^\nu}.
}
\tag{4.7}
\]

这只是 \(q\) 与高二进邻因子的符号匹配，不产生统一矛盾。不能把
\(\lambda\) 写成 \(v_2(k-1)\)。例如

\[
k=5,\quad q=3
\]

时

\[
v_2(kq-1)=1,\qquad v_2(k-1)=2.
\]

更一般地，取固定 \(q=3\) 和

\[
k=1+2^r,\qquad r\ge2,
\]

则

\[
v_2(3k-1)=1,\qquad v_2(k^2-1)=r+1.
\]

所以即使 \(\lambda=1\) 固定，\(\kappa_2\) 仍可任意大。反方向，
固定奇数 \(k\) 后，也可由中国剩余定理选择移动的奇数 \(q\)，使
\(v_2(kq-1)\) 任意大。这里的例子只证明两个赋值没有代数同一性，
不冒充完整候选。

结合 (3.15)，二进互补条件为

\[
\boxed{
\min(\delta_2,\kappa_2-\delta_2)
\le
1+n+v_2(H_1)-\delta_2.
}
\tag{4.8}
\]

其右端随 \(n\) 和数字块 \(H_1\) 移动。它能删除高而平衡的
\(2\)-进分配，却不能关闭 A、B、C 中任一完整室。

---

## 5. 五进部分

### 5.1 阶段 II 核心引理 SD-II.2：五进尺度溢出整体无解

先记录两个由真实尾窗得到的严格关系。由

\[
b_3=b_1d\gamma u,\qquad
Y=vdZ,\qquad
\tau=\frac{b_1u}{v},
\]

有

\[
\frac{b_3}{Y}=\frac{\gamma\tau}{Z}.
\]

所以

\[
\boxed{
\gamma\tau<Z\le10\gamma\tau.
}
\tag{5.1}
\]

再由 (1.1)，

\[
qk-1=Z\frac{q+b_1N}{\gamma}.
\]

使用 \(Z\le10\gamma\tau\)、\(N<10q\)、\(b_1\le2\)、\(q\ge3\)，
得到

\[
\begin{aligned}
qk-1
&\le10\tau(q+b_1N)
<210\tau q,
\end{aligned}
\]

故

\[
\boxed{k\le210\tau.}
\tag{5.2}
\]

现在反设

\[
\varphi=v_5(g)>n.
\tag{5.3}
\]

则

\[
v_5(d)=n,\qquad 5^n\mid d\mid K.
\tag{5.4}
\]

奇素数幂模 \(5^n\) 的 \(1\) 的平方根只有 \(\pm1\)，故

\[
k\equiv\pm1\pmod{5^n}.
\]

由于 \(k>1\) 且 \(k\) 为奇数，

\[
\boxed{k\ge2\cdot5^n-1.}
\tag{5.5}
\]

另一方面，\(\varphi>n\) 使

\[
5\mid\gamma.
\]

又因 \(d\mid Y/v\)、\(v_2(d)\ge1\)，约去 \(d\) 的完整
\(5^n\) 后，

\[
Z=\frac{Y}{vd}\le2^{n-1}.
\tag{5.6}
\]

由 (5.1)，

\[
\boxed{
\tau<\frac Z\gamma\le\frac{2^{n-1}}5.
}
\tag{5.7}
\]

联合 (5.2)、(5.5)、(5.7)：

\[
2\cdot5^n-1
\le k
\le210\tau
<21\cdot2^n.
\tag{5.8}
\]

当 \(n=3\) 时左端为 \(249\)，右端为 \(168\)；此后两端的主比率
每增加一次 \(n\) 还会再乘 \(5/2\)。所以 (5.8) 强迫

\[
n\le2.
\tag{5.9}
\]

但 \(a\ge1\)、\(\varphi\ge n+1\)、\(u\ge1\)、\(b_1\ge1\) 又给

\[
b_3=b_1gu
\ge2\cdot5^{n+1}.
\]

与 \(b_3<Y=2^n5^n\) 比较得到

\[
10<2^n,
\]

即 \(n\ge4\)，与 (5.9) 矛盾。因此

\[
\boxed{v_5(g)=\varphi\le n.}
\tag{5.10}
\]

于是

\[
\boxed{
v_5(d)=\varphi,\qquad v_5(\gamma)=0.
}
\tag{5.11}
\]

这完整关闭了题设要求检查的

\[
\boxed{v_5(g)>n}
\]

尺度溢出，而不依赖有限搜索。

若 \(\varphi>0\)，全部 \(5\)-进赋值确实落在 \(k-1\) 或 \(k+1\)
之一。存在唯一符号 \(\sigma_5\in\{\pm1\}\) 使

\[
\boxed{k\equiv\sigma_5\pmod{5^\varphi}.}
\tag{5.12}
\]

但 \(\sigma_5\) 不由 A、B、C 统一固定。循环方程只把它与移动的
\(q\) 和 \(q+b_1N\) 的五进类耦合；两种符号都没有被现有 E4
关系统一排除。

五进互补条件现在化为

\[
\boxed{
\min(\varphi,v_5(K)-\varphi)
\le n+v_5(H_1)-\varphi.
}
\tag{5.13}
\]

它仍只给移动领圈，不给 \(\varphi\) 或 \(v_5(d)\) 的绝对上界。

---

## 6. 奇素数部分

### 6.1 阶段 II 核心引理 SD-II.3：非十进制部分整体进入恢复因子

令

\[
\boxed{
K^{(10)}
=\frac{K}{2^{v_2(K)}5^{v_5(K)}}.
}
\tag{6.1}
\]

由于 \(d=\gcd(g,E)\) 是 \((2,5)\)-平滑数，

\[
\gcd(d,K^{(10)})=1.
\]

由 (3.2)，对每个 \(p\ne2,5\) 且 \(p^{\kappa_p}\parallel K\)，

\[
\boxed{
p^{\kappa_p}\mid L_\varepsilon.
}
\tag{6.2}
\]

统一写为

\[
\boxed{
K^{(10)}\mid A+\varepsilon kw_0.
}
\tag{6.3}
\]

这正是全部非十进制奇素数进入同一共轭因子的全局同步条件。它不能被
拆成逐个素数任选符号：同一个 \(\varepsilon\) 必须同时适用于
\(K^{(10)}\) 的全部素因子。

模任意 \(p^{\kappa_p}\parallel K^{(10)}\)，(6.3) 给出

\[
A\equiv-\varepsilon kw_0\pmod{p^{\kappa_p}}.
\tag{6.4}
\]

平方后与

\[
A^2-k^2w_0^2=KQ
\]

完全相容。因此单个素数上没有固定二次非剩余障碍；真正的新条件是所有
奇素数必须选择同一个共轭符号。另一方面，

\[
K^{(10)}
\le L_\varepsilon
<
(k+1)A
\tag{6.5}
\]

在 \(L_+\) 恢复时成立，而 \(L_-\) 恢复时有

\[
K^{(10)}\le L_-\le A.
\tag{6.6}
\]

但 \(A=YH_1/d\) 仍随 \(m,n,d\) 无界移动，(6.5)–(6.6) 不产生
统一大小矛盾。

不能假定 \(K\) 的奇素因子彼此不同。例如

\[
k=19,\qquad K=360=2^3\cdot3^2\cdot5
\]

已含平方奇因子。全文的 (6.2) 按完整素数幂表述，没有使用平方自由性。

因此 P1 得到严格证明，但它没有关闭 \(\gamma=1\)、\(\gamma>1\)
或 A、B、C 中任一完整室。

---

## 7. 第三块窗口

### 7.1 阶段 III 核心引理 SD-III.1：共轭商的严格区间

由 (2.6)，

\[
0\le w_0<A.
\]

先取 \(L_+\) 恢复。此时

\[
L_+=\frac Kd\,a_3,\qquad
L_-=d\mathscr R_3.
\]

由

\[
L_+<(k+1)A,\qquad
-(k-1)A<L_-\le A,
\]

得到

\[
\boxed{
(k-1)a_3<YH_1,
}
\tag{7.1}
\]

\[
\boxed{
-\frac{(k-1)YH_1}{d^2}
<
\mathscr R_3
\le
\frac{YH_1}{d^2}.
}
\tag{7.2}
\]

所以 \(L_+\) 恢复允许 \(Q=a_3\mathscr R_3\) 为负、零或正。

再取 \(L_-\) 恢复。它只有在 \(Q>0\) 时存在，并满足

\[
0<L_-\le A,\qquad
A\le L_+<(k+1)A.
\]

于是

\[
\boxed{
Ka_3\le YH_1,
}
\tag{7.3}
\]

\[
\boxed{
\frac{YH_1}{d^2}
\le
\mathscr R_3
<
\frac{(k+1)YH_1}{d^2}.
}
\tag{7.4}
\]

特别地 \(L_-\) 恢复自动有

\[
\mathscr R_3>0,\qquad Q>0.
\]

联合严格第三块窗口，

\[
\boxed{
\begin{array}{ll}
L_+\text{ 恢复}:&
Y\le a_3<10Y,\quad
a_3<\dfrac{YH_1}{k-1};\\[3mm]
L_-\text{ 恢复}:&
Y\le a_3<10Y,\quad
a_3\le\dfrac{YH_1}{K}.
\end{array}}
\tag{7.5}
\]

所以任何候选都必须满足

\[
\boxed{k-1<H_1,}
\tag{7.6}
\]

而负号恢复还必须满足

\[
\boxed{K\le H_1.}
\tag{7.7}
\]

由中分子窗口，

\[
\frac T{10}\le10a_2<T,
\]

故

\[
\left(a_1+\frac1{10}\right)T
\le H_1<(a_1+1)T\le14T.
\tag{7.8}
\]

因此得到统一的相对上界

\[
\boxed{k\le H_1<14T,}
\tag{7.9}
\]

并在负号恢复中得到

\[
\boxed{k^2-1\le H_1<14T.}
\tag{7.10}
\]

这些上界随 \(T=10^m\) 移动，不是 SD4 所要求的绝对上界。

式 (7.2)、(7.4) 对每个固定约化状态只留下有限多个整数
\(\mathscr R_3\)，但区间长度含

\[
\frac{YH_1}{d^2},\qquad k,
\]

它们尚未统一有界。因此这不是 SD5 的有限尺度状态。

### 7.2 阶段 III 核心引理 SD-III.2：共轭分配后的完整回代

由 (3.11)，

\[
Ka_3^2-2YH_1a_3+d^2Q=0.
\tag{7.11}
\]

代入

\[
Q=k^2\gamma^2\mathcal R-A^2,
\qquad dA=YH_1,
\]

得到

\[
(YH_1+a_3)^2
=k^2\bigl(d^2\gamma^2\mathcal R+a_3^2\bigr).
\tag{7.12}
\]

定义

\[
t=\frac{YH_1+a_3}{k}>0.
\tag{7.13}
\]

式 (7.12) 说明 \(t^2\) 是整数。正有理数的平方若为整数，则该有理数
本身为整数，所以

\[
t\in\mathbb Z_{>0}.
\]

于是精确恢复

\[
\boxed{
(gua_1)^2+(gva_2)^2+a_3^2=t^2,
}
\tag{7.14}
\]

\[
\boxed{
Y(a_1T+10a_2)+a_3=kt.
}
\tag{7.15}
\]

因此，共轭因子、正确尺度公式与 \(a_3\) 恢复确实足以恢复两条主方程；
但原题候选还必须同时核对：

\[
10^{m-2}\le a_2<10^{m-1},\qquad
Y\le a_3<10Y,
\]

\[
\gcd(a_1,b_1)=
\gcd(a_2,b_2)=
\gcd(a_3,b_3)=1,
\]

以及 K5、终端商、E4 高阶门和真实分母窗口。单独的
\(a_3\mid Q\)、(3.13) 或 (6.3) 都不是原题解。

### 7.3 阶段 III 核心引理 SD-III.3：为什么没有有限化

本轮得到的完整新必要链为

\[
\boxed{
\begin{gathered}
L_+L_-=KQ,\qquad
L_\varepsilon=\frac Kd a_3,\qquad
L_{-\varepsilon}=d\mathscr R_3,\\
Q=a_3\mathscr R_3,\qquad
Ka_3+d^2\mathscr R_3=2YH_1,\\
\min(v_p(d),v_p(K)-v_p(d))\le v_p(2A),\\
K^{(10)}\mid L_\varepsilon,\qquad
v_5(g)\le n.
\end{gathered}}
\tag{7.16}
\]

但下列量仍可在继承系统中移动：

\[
q,\ N,\ \gamma,\ Z,\ k,\ m,\ n,\ a,\ e,\ \varphi,\ g_\ast,
\]

以及按室出现的

\[
\eta,\theta_A,\theta_B,\kappa,\xi_C,\zeta_{C,J},e_2,h_B,\varepsilon_B.
\]

具体地：

1. \(v_5(g)>n\) 已关闭，但 \(0\le\varphi\le n\) 仍随 \(n\) 无界；
2. \(\gamma\) 已被证明与 \(5\) 互素，却仍可含
   \(g_\ast>1\)，并可在 C1 的 \(a>n\) 状态含二进溢出；
3. 二进条件只把 \(v_2(d)\) 放入两个随
   \(n+v_2(H_1)\) 移动的领圈；
4. \(K^{(10)}\) 的全部素数必须同步进入一个共轭因子，但
   \(K\)、\(A\) 和该共轭因子本身都无界；
5. \(\mathscr R_3\) 对每个固定状态有限，但其允许区间长度没有统一上界；
6. \(k<14T\) 与负号下的 \(k^2<14T+1\) 都是相对界，不是绝对界。

所以本轮没有把本原层压成有限多个尺度分配状态。

---

## 8. 完整回代与主动反例攻击

### 8.1 \(Q\) 是否可能为负

可以。第 2.2 节的

\[
(A,k,K,\gamma,\mathcal R,w_0)=(5,3,8,1,2,3)
\]

给出 \(Q=-7\)。此时 \(L_+>0>L_-\)，只有正号恢复可保留。

### 8.2 是否只保留 \(L_\varepsilon>0\)

是。\(L_+\) 恒正；\(L_-\) 当且仅当 \(Q>0\) 时为正。
\(Q=0\) 时 \(L_-=0\)，不是合法恢复符号。

### 8.3 是否正确使用 \(\gcd(a_3,d)=1\)

是。从

\[
a_3L_{-\varepsilon}=dQ
\]

和 \(\gcd(a_3,d)=1\) 推出 \(a_3\mid Q\)。没有从
\(a_3\mid dQ\) 直接跳步。

### 8.4 是否把 \(d\mid K\) 加强成 \(d^2\mid K\)

没有。第 2.2 节的负 \(Q\) 数据有

\[
d=4,\qquad K=8,\qquad d^2\nmid K.
\]

### 8.5 是否混淆 \(\lambda\) 与 \(v_2(k-1)\)

没有。第 4 节只通过高邻因子的符号 \(\sigma_2\) 建立 (4.6)–(4.7)，
并给出 \(k=5,q=3\) 的显式反例。

### 8.6 是否假定 \(K\) 的奇素因子全部不同

没有。全部结论按 \(p^{v_p(K)}\) 表述；\(k=19\) 的
\(3^2\mid K\) 明确展示了重复奇因子。

### 8.7 是否遗漏 \(d\) 与 \(K/d\) 共享 \(2,5\) 因子

没有。共享时正是 (3.13) 发挥作用。负 \(Q\) 数据中

\[
d=4,\qquad K/d=2
\]

已经共享因子 \(2\)，并且

\[
\min(2,1)=v_2(2A)=1,
\]

说明 (3.13) 可以取等。

### 8.8 第三块端点是否严格

是。始终使用

\[
Y\le a_3<10Y.
\]

正号的附加上界严格，负号的 \(Ka_3\le YH_1\) 在 \(w_0=0\)
时允许等号。

### 8.9 是否在移动参数未控制时有限搜索

没有。本轮只用整数恒等式、赋值、严格窗口和两个显式小型算术反例。
没有以任何有界盒支持全局结论。

### 8.10 是否把 \(a_3\mid Q\) 误写成原题解

没有。第 7.2 节明确回代两条主方程，并在其后继续保留全部数字块窗口、
逐项既约、K5、终端商和 E4 门。

### 8.11 是否真正关闭了 \(v_5(g)>n\)

是。证明同时使用：

1. 共轭恢复给出的 \(d\mid K\)；
2. 奇数 \(k\) 在模 \(5^n\) 下的 \(\pm1\) 分类；
3. 终端因子给出的 \(k\le210\tau\)；
4. 尾窗给出的 \(\gamma\tau<Z\)；
5. \(v_2(d)\ge1\) 给出的 \(Z\le2^{n-1}\)；
6. 原尾分母严格上窗。

没有把该关闭扩大成 \(\gamma>1\) 整体无解。

---

## 9. 最终分类 SD1–SD6

本轮在题设六级分类中达到

\[
\boxed{
\mathrm{SD6}:
\quad
\text{得到新的共轭因子、互补尺度和第三块整除条件，}
\text{但未达到 SD1--SD5。}
}
\tag{9.1}
\]

同时记录一个超出“裸 SD6”描述的附带分支关闭：

\[
\boxed{
v_5(g)>n\quad\text{整体无解}.
}
\tag{9.2}
\]

为什么不是 SD1：

- A、B、C 均仍有开放本原状态；
- 没有证明完整本原层无解，也没有找到合法解。

为什么不是 SD2：

- \(\gamma=1\) 未关闭；
- \(\gamma>1\) 未关闭；
- (9.2) 只删除 \(\gamma\) 的五进溢出来源，不能删除奇核心或 C1
  的二进溢出。

为什么不是 SD3：

- 没有关闭 A、B、C 中任何一个完整 E4 室；
- 五进溢出只是一条横切各室的子分支。

为什么不是 SD4：

- \(v_5(g)\le n\) 是相对界；
- \(k<14T\) 和负号下 \(k^2<14T+1\) 也是相对界；
- \(d,v_2(d),v_5(d),a_3,k\) 均无绝对统一上界。

为什么不是 SD5：

- 每个固定约化状态的两个恢复符号和 \(\mathscr R_3\) 区间有限；
- 但约化状态及区间长度仍随
  \((q,N,\gamma,Z,k,m,n)\) 无界移动。

为什么达到 SD6：

1. 证明了完整乘积 \(L_+L_-=KQ\)；
2. 证明了精确互补分配
   \[
   L_\varepsilon=(K/d)a_3,\qquad
   L_{-\varepsilon}=d\mathscr R_3;
   \]
3. 证明了 \(a_3\mid Q\)；
4. 得到统一共享素数门 (3.13)；
5. 证明全部 \(K^{(10)}\) 必须进入同一恢复因子；
6. 得到符号化的第三块和共轭商严格窗口；
7. 完成两条主方程的回代审计；
8. 额外关闭全部五进尺度溢出。

没有找到合法原题解。

---

## 10. \(G\) 模板是否继续

本轮后的本原正余数候选除 PR6 全部条件外，还必须满足

\[
\boxed{
\begin{gathered}
v_5(g)\le n,\qquad \gcd(\gamma,5)=1,\\
L_+L_-=KQ,\qquad
Q=a_3\mathscr R_3,\\
L_\varepsilon=\frac Kd a_3,\qquad
L_{-\varepsilon}=d\mathscr R_3,\\
Ka_3+d^2\mathscr R_3=2YH_1,\\
\min(v_p(d),v_p(K)-v_p(d))\le v_p(2A),\\
K^{(10)}\mid A+\varepsilon kw_0,\\
k\le H_1<14T,
\end{gathered}}
\tag{10.1}
\]

并按恢复符号满足：

\[
\boxed{
\begin{array}{c|c|c}
\text{符号}&Q\text{ 的符号}&\mathscr R_3\text{ 区间}\\ \hline
L_+&\text{任意}&
-\dfrac{(k-1)YH_1}{d^2}
<\mathscr R_3\le\dfrac{YH_1}{d^2}\\[3mm]
L_-&Q>0&
\dfrac{YH_1}{d^2}
\le\mathscr R_3<
\dfrac{(k+1)YH_1}{d^2}
\end{array}}
\tag{10.2}
\]

其中负号还要求

\[
k^2-1\le H_1.
\tag{10.3}
\]

这条路线值得保留，但现阶段不值得仅继续增加逐素数模条件。下一次若继续
\(G\)，真正需要的新输入必须至少完成下列一项：

1. 控制同一符号下 \(K^{(10)}\mid A+\varepsilon kw_0\) 的全局同步；
2. 对移动量 \(YH_1/d^2\) 给出绝对或有限状态界；
3. 把 C1 的二进溢出或 \(g_\ast>1\) 的奇核心整体关闭；
4. 把 (3.11) 与 E4 某一完整室的高阶关系组合成矛盾。

单独重复尺度唯一性、逐个枚举 \(K\) 的素因子、固定移动参数做有限搜索，
或只使用 \(a_3\mid Q\)，都不能越过本报告的停止点。

\[
\boxed{
\begin{gathered}
\text{五进尺度溢出已经关闭；}\\
\text{共轭因子给出精确互补尺度和第三块商；}\\
\text{但 }\gamma=1,\gamma>1\text{、A、B、C 仍均有开放状态；}\\
\text{故本轮分类为 SD6，G 模板保留但暂不沿同一机制重复推进。}
\end{gathered}}
\]

全文到此停止；不研究非本原 C2、C5、O 或 Q，不返回 \(J=10\)、
零余数或 \(5\mid q\)。
