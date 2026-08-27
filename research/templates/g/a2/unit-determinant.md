# 三项十进制拼接平方和问题：临界 (G) 模板 A2 单位行列式战役

日期：2026-08-01（Asia/Tokyo）

研究范围：

\[
\boxed{
G_{\mathrm{prim}},\qquad \gamma=1,\qquad \mathrm{A2}.
}
\]

本文暂时接受 T1–T18、K5、CG、E4、GT4、VA1、GD1、GP3、CD6、
PR6、SD6 和 GA1-1，不作全项目统一独立审计。本文不研究 B、C、
\(\gamma>1\)、非本原 C2/C5、Q 或严格层。

最终分类为

\[
\boxed{\mathrm{GA2\text{-}6}.}
\]

这里必须同时记录两个强于“裸局部筛”的分支定理：

\[
\boxed{a=2\Longrightarrow\text{无候选},}
\tag{0.1}
\]

以及对全部 (a\ge2) 的精确五进尺度锁定

\[
\boxed{v_5(k^2-1)=2\varphi.}
\tag{0.2}
\]

但高层 (a\ge3) 仍含随 (a) 移动的 (\varphi) 和 (r) 提升深度；
本文没有把它们压成有限个递推提升族，也没有给出覆盖全部 (a) 的有限
周期证书。因此不能分类为 GA2-1、GA2-2 或 GA2-3。

---

## 1. GA1-1 后的 (G) 状态

GA1-1 已严格证明

\[
G_{\mathrm{prim}},\quad\gamma=1,\quad\mathrm{A1}
\Longrightarrow\text{无候选}.
\]

在同一 A 室中只剩 A2：

\[
b_1=v=2,\qquad c=0,\qquad u=5^e,
\tag{1.1}
\]

\[
T=10^m,\qquad Y=10^n,\qquad m\ge2,
\tag{1.2}
\]

\[
a\ge2,\qquad \lambda=v_2(kq-1)=2a-1,\qquad n=3a.
\tag{1.3}
\]

本原单位行列式给出

\[
g=d=2^a5^\varphi,
\tag{1.4}
\]

而 GP3、PR6 给出

\[
N=2^m5^{m-e},\qquad b_2=q5^e,\qquad b_3=2d5^e,
\tag{1.5}
\]

\[
q\ge3,\qquad \gcd(q,10)=1,\qquad e\le m.
\tag{1.6}
\]

十三首块在 A 室中只剩

\[
a_1\in\{5,7,9,11,13\},
\tag{1.7}
\]

并始终保留

\[
10^{m-2}\le a_2<10^{m-1},\qquad
Y\le a_3<10Y,
\tag{1.8}
\]

以及三个逐项既约条件。

---

## 2. A2 单位行列式系统与完整双向终端化

PR6 中

\[
Z=\frac{Y}{2d},\qquad E_0=2Z,\qquad M_0=k-Z,
\tag{2.1}
\]

\[
qM_0-E_0N=1.
\tag{2.2}
\]

定义

\[
r=k-Z.
\tag{2.3}
\]

则 (2.2) 严格等价于

\[
\boxed{qr=2ZN+1.}
\tag{2.4}
\]

又因

\[
M_0=JE_0+\rho_0,qquad0<\rho_0<E_0,
\]

有

\[
\boxed{
2JZ<r<2(J+1)Z,qquad J\in\{1,\ldots,9\},
}
\tag{2.5}
\]

\[
\rho_0=r-2JZ.
\tag{2.6}
\]

恢复公式是

\[
q=\frac{2ZN+1}{r},\qquad k=r+Z,
\tag{2.7}
\]

\[
s=N-Jq
=\frac{N(r-2JZ)-J}{r}
=\frac{N\rho_0-J}{r}.
\tag{2.8}
\]

因此真正的初端门为

\[
\boxed{s>0\iff N\rho_0>J.}
\tag{2.9}
\]

另一方面，由 (r<2(J+1)Z)，

\[
q-s=(J+1)q-N
=\frac{N(2(J+1)Z-r)+(J+1)}r>0.
\tag{2.10}
\]

所以一旦 (s>0)，便自动有

\[
0<s<q.
\tag{2.11}
\]

此时 (q\) 是正奇数；后文还将得到 (5\nmid qr)，故 (q\ne2)。
结合 (0<s<q)，自动有 (q\ge3)。此外

\[
N=Jq+s
\]

给

\[
q<N<10q,
\]

于是

\[
\frac T{10}<b_2<T.
\tag{2.12}
\]

这证明了终端状态与

\[
(q,r,s,\rho_0,J,k)
\]

之间的完整双向性；非平凡初端条件只有 (2.9)，而不是另行对有限个
(m) 试验。

---

## 3. 尾窗条带

由 (n=3a) 与 (1.4)，

\[
\boxed{Z=2^{2a-1}5^{3a-\varphi}.}
\tag{3.1}
\]

定义

\[
h=\varphi+e-3a.
\tag{3.2}
\]

第三分母窗口

\[
\frac Y{10}\le2d5^e<Y
\]

严格等价于

\[
1<2^{2a-1}5^{-h}\le10,
\tag{3.3}
\]

即

\[
\boxed{
\frac{2^{2a-2}}5\le5^h<2^{2a-1}.
}
\tag{3.4}
\]

若 (h\le-1)，则 (5^h\le1/5)，而 (a\ge2) 时
(2^{2a-2}/5\ge4/5)，矛盾。因此

\[
\boxed{h\ge0.}
\tag{3.5}
\]

令

\[
c_5=\log_5 2,
\qquad
h_+(a)=\left\lfloor(2a-1)c_5\right\rfloor,
\qquad
h_-(a)=h_+(a)-1.
\tag{3.6}
\]

(c_5) 无理，所以不存在端点歧义。全部允许整数恰为

\[
\boxed{
\mathcal H(a)=
\left\{
h\in\{h_-(a),h_+(a)\}:
5^{h+1}\ge2^{2a-2}
\right\}.
}
\tag{3.7}
\]

证明是：允许区间的实长度为

\[
1+\log_5 2<2,
\]

故至多包含两个整数；最大的整数严格小于
((2a-1)\log_5 2)，正是 (h_+(a))，可能的另一个只能是
(h_-(a))，最后用左端不等式过滤。

特别地，“每个 (a) 至多两个 (h)”不意味着 (a) 有界。

由 (3.2)，

\[
e=3a+h-\varphi,
\tag{3.8}
\]

并且

\[
m-h=(m-e)+(3a-\varphi)\ge0.
\tag{3.9}
\]

还可把尾窗写成一个有用的尺度比较：

\[
\boxed{5^e<Z\le10\cdot5^e.}
\tag{3.10}
\]

---

## 4. 终端因子与完整指数级数

由 (2.4)、(3.1) 和 (N=2^m5^{m-e})，

\[
\boxed{
qr=1+2^{2a+m}5^{m-h}.
}
\tag{4.1}
\]

令

\[
\ell=m-h,\qquad C_{a,h}=2^{2a+h}.
\tag{4.2}
\]

则

\[
\boxed{qr=1+C_{a,h}10^\ell.}
\tag{4.3}
\]

后文将证明 \(\varphi\ge1\) 且 \(5\mid Z\)。由 \(d\mid k^2-1\)
又有 \(k\equiv\pm1\pmod5\)，故

\[
r=k-Z\equiv\pm1\pmod5.
\]

所以

\[
\gcd(r,10)=1.
\tag{4.4}
\]

固定

\[
(a,h,\varphi,J,r)
\]

后，令

\[
M_r=\operatorname{ord}_r(10),
\tag{4.5}
\]

并考察离散对数

\[
10^\ell\equiv-C_{a,h}^{-1}\pmod r.
\tag{4.6}
\]

若 (4.6) 无解，该 (r) 整体删除；若有解，则解在
(\mathbb Z/M_r\mathbb Z) 中唯一。记其标准代表为
(\ell_0\in[0,M_r))。全部指数恰为

\[
\ell=\ell_0+tM_r,qquad t\in\mathbb Z.
\tag{4.7}
\]

再令 (\ell_*\) 是该同余类中满足

\[
\ell\ge\max(0,2-h,e-h),
\tag{4.8}
\]

\[
2^{\ell+h}5^{\ell+h-e}\rho_0>J
\tag{4.9}
\]

的最小整数。由于左边沿 (\ell\mapsto\ell+M_r) 严格增加，
(\ell_*\) 存在且唯一。于是该终端状态的全部真实指数恰为

\[
\boxed{
m=m_*+tM_r,qquad m_*=h+\ell_*,\qquad t\ge0.
}
\tag{4.10}
\]

这里 (4.9) 正是 (s>0)；(2.10) 自动给 (s<q)。这是一条覆盖
全部无界指数的精确级数，不是有限 (m) 搜索。

---

## 5. 尺度大小门

SD6 精确恢复首先给

\[
\boxed{d\mid K:=k^2-1.}
\tag{5.1}
\]

由终端窗口，

\[
k=r+Z<(2J+3)Z\le21Z.
\tag{5.2}
\]

若 \(\varphi=3a\)，则

\[
d=2^a5^{3a},\qquad Z=2^{2a-1}.
\]

因此

\[
2^a5^{3a}=d\le K<k^2<441Z^2
=441\cdot2^{4a-2},
\]

即

\[
5^{3a}<441\cdot2^{3a-2}.
\tag{5.3}
\]

当 (a=2) 时左、右之比已经为

\[
\frac{5^6}{441\cdot2^4}>1,
\]

以后每增加一次 (a)，该比值再乘 (125/8>1)。故 (5.3)
对全部 (a\ge2) 失败。于是

\[
\boxed{\varphi\le3a-1.}
\tag{5.4}
\]

由 (h\ge0) 与 (3.8)，

\[
e\ge1.
\tag{5.5}
\]

K5 的支撑门 (\operatorname{rad}(u)\mid qg) 及 (5\nmid q)
随即给出

\[
\boxed{\varphi\ge1.}
\tag{5.6}
\]

所以

\[
\boxed{
1\le\varphi\le3a-1,qquad e\ge1,qquad5\mid Z,
}
\tag{5.7}
\]

并始终保留

\[
\boxed{2^a5^\varphi\mid k^2-1.}
\tag{5.8}
\]

---

## 6. 二进、五进尺度恢复

### 6.1 统一局部记号

归一化判别式为

\[
\boxed{
w_0^2=A^2-KR,
}
\tag{6.1}
\]

其中

\[
A=2ZH_1,qquad H_1=a_1T+10a_2,
\tag{6.2}
\]

\[
R=(5^ea_1)^2+(2a_2)^2,qquad K=k^2-1.
\tag{6.3}
\]

两个恢复因子为

\[
L_\varepsilon=A+\varepsilon kw_0,qquad\varepsilon\in\{\pm1\},
\tag{6.4}
\]

并且一个完整候选必须对某个符号满足

\[
\boxed{
d=\frac K{\gcd(K,L_\varepsilon)}.
}
\tag{6.5}
\]

因 (a_3=L_\varepsilon/\gcd(K,L_\varepsilon)) 与 (2d5^e)
互素，对 (p=2,5) 都有精确值

\[
\boxed{
v_p(L_\varepsilon)=v_p(K)-v_p(d).
}
\tag{6.6}
\]

互补因子还满足

\[
\boxed{v_p(L_{-\varepsilon})\ge v_p(d).}
\tag{6.7}
\]

逐项既约给 (5\nmid a_2)。由于 (m\ge2)，

\[
v_5(H_1)=1.
\tag{6.8}
\]

另一方面 (b_2=q5^e) 为奇数，所以 (a_2) 的奇偶性不固定。令

\[
u_2=v_2(H_1)\ge1.
\tag{6.9}
\]

则

\[
v_2(A)=2a+u_2,qquad
v_5(A)=3a-\varphi+1.
\tag{6.10}
\]

并且

\[
v_2(R)=v_5(R)=0.
\tag{6.11}
\]

式 (6.11) 在二进处来自“奇平方加 (4) 的倍数”，在五进处来自
(e\ge1) 与 (5\nmid a_2)。

### 6.2 五进尺度完全锁定

记

\[
\beta=v_5(K),\qquad \zeta=3a-\varphi,qquad
C_a=(2a-1)\log_5 2+\log_5 22.
\tag{6.12}
\]

由 (5^\varphi\mid K)，(k\) 是模 (5^\varphi) 的平方根
\(\pm1\)。故

\[
5^\varphi\le k+1<21Z+1<22Z.
\tag{6.13}
\]

取 (\log_5) 得

\[
2\varphi<3a+C_a,
\qquad
\zeta>\frac{3a-C_a}{2}.
\tag{6.14}
\]

对 (a\ge2)，有

\[
3a+4>3C_a.
\tag{6.15}
\]

证明只需检查 (a=2)：(6.15) 等价于

\[
5^{10}>2^9\cdot22^3,
\]

即 (9{,}765{,}625>5{,}451{,}776)；以后左、右对数斜率之差为
(3-6\log_5 2>0)，因为 (5>4)。

由 (6.14)–(6.15)，

\[
C_a<\zeta+2.
\tag{6.16}
\]

又因 (5^\beta\le k+1<22Z)，

\[
\boxed{
\beta<\zeta+C_a<2\zeta+2
=2v_5(A).
}
\tag{6.17}
\]

所以 (6.1) 在五进处的唯一最低项是 (KR)。判别式为平方迫使

\[
\beta\in2\mathbb Z,qquad v_5(w_0)=\frac\beta2<v_5(A).
\tag{6.18}
\]

因此两个符号都满足

\[
v_5(L_\pm)=\frac\beta2.
\tag{6.19}
\]

把 (6.19) 代入精确恢复 (6.6)：

\[
\frac\beta2=\beta-\varphi.
\]

故严格得到

\[
\boxed{
\beta=v_5(k^2-1)=2\varphi.
}
\tag{6.20}
\]

这证明了题设 (D3?) 的五进一半，而且没有异常高层室。

再由 (5^{2\varphi}\le k+1<22Z)，得到更强的移动上界

\[
\boxed{
3\varphi<3a+C_a,
\qquad
\varphi<a+\frac{C_a}{3}.
}
\tag{6.21}
\]

最后，将 (6.1) 除以 (5^{2\varphi}) 并模 (5)，有

\[
\left(\frac{w_0}{5^\varphi}\right)^2
\equiv
-4\frac K{5^{2\varphi}}a_2^2\pmod5.
\]

因为 (-1) 和 (4) 都是模 (5) 平方，必须有

\[
\boxed{
\frac K{5^{2\varphi}}\equiv1\text{ 或 }4\pmod5.
}
\tag{6.22}
\]

### 6.3 二进尺度的完整分室

记

\[
\alpha=v_2(K),\qquad A_2=2a+u_2=v_2(A).
\tag{6.23}
\]

由 (d\mid K)，

\[
\alpha\ge a.
\tag{6.24}
\]

必须分三种比较。

#### 情形 I：\(\alpha<2A_2\)

(KR) 是 (6.1) 的唯一最低项。因此

\[
\alpha\in2\mathbb Z,qquad v_2(w_0)=\frac\alpha2<A_2.
\]

两个 (L_\pm) 都有赋值 (\alpha/2)。由 (6.6)，

\[
\frac\alpha2=\alpha-a,
\]

所以

\[
\boxed{\alpha=2a.}
\tag{6.25}
\]

#### 情形 II：\(\alpha>2A_2\)

(A^2) 是唯一最低项，故

\[
v_2(w_0)=A_2.
\]

把 (A,w_0) 同除以 (2^{A_2})，所得两项都是奇数。因此

\[
v_2(L_+),v_2(L_-)
=A_2+\{1,c\},\qquad c\ge2.
\tag{6.26}
\]

若恢复符号落在低赋值因子上，则 (6.6) 给

\[
\alpha-a=A_2+1,
\]

即 (a=\alpha-A_2-1>A_2-1)，与 (A_2=2a+u_2) 矛盾。
所以恢复符号必须是高消去因子，互补符号恰有赋值 (A_2+1)。

#### 情形 III：\(\alpha=2A_2\)

若 (v_2(w_0)>A_2)，则两个 (L_\pm) 都只有赋值 (A_2)，而
(6.6) 要求 (2A_2-a>A_2)，矛盾。因此仍须

\[
v_2(w_0)=A_2,
\]

并与情形 II 一样只能选择高消去符号。

综上，二进尺度的完整替代关系是

\[
\boxed{
\begin{array}{ll}
\mathrm P_2:&\alpha=2a;\\[1mm]
\mathrm E_2:&\alpha\ge2A_2=4a+2u_2\ge4a+2,
\end{array}}
\tag{6.27}
\]

其中异常室 (\mathrm E_2) 对唯一恢复符号满足

\[
\boxed{
v_2\!\left(
\frac A{2^{A_2}}+\varepsilon k\frac{w_0}{2^{A_2}}
\right)=\alpha-a-A_2,
}
\tag{6.28}
\]

而相反符号的归一化赋值恰为 (1)。

所以题设拟议的

\[
\alpha=2a
\]

不能无条件预设；准确结论是 (6.27)。这已经完整处理最低赋值唯一、
同层消去、平方偶赋值、两个恢复符号、(a_2) 奇偶和移动的
(v_2(H_1))。

在主室中，将 (6.1) 除以 (2^{2a}) 并模 (8)，得到

\[
\boxed{
\frac K{2^{2a}}\equiv
\begin{cases}
7\pmod8,&2\mid a_2,\\
3\pmod8,&2\nmid a_2.
\end{cases}}
\tag{6.29}
\]

---

## 7. 修正后的 Jacobi 锁定

题设草案中有一步不能直接使用：

\[
k^2\equiv1\pmod8
\not\Longrightarrow
k\equiv\pm1\pmod8.
\tag{7.1}
\]

事实上所有奇数平方都模 (8) 等于 (1)，例如 (k\equiv3,5\pmod8)
也满足左式。因此仅从 (2^a\mid K) 且 (a=3) 不能得到题设的
(k\equiv\pm1\pmod8)。这不是 PR6、SD6 或 GA1-1 的继承错误；
它只是本轮拟议 Jacobi 论证中的新漏洞。

正确修复必须先使用第 6.3 节。由 (6.27)，任何完整候选都有

\[
\alpha\ge2a\ge4.
\]

故 (16\mid k^2-1)，从模 (16) 的四个平方根得到

\[
k\equiv\pm1\pmod8.
\tag{7.2}
\]

又因 (8\mid Z)，

\[
r=k-Z\equiv k\equiv\pm1\pmod8.
\tag{7.3}
\]

由 (5^\varphi\mid K)、(5\mid Z)，

\[
r\equiv k\equiv\pm1\pmod5,
\]

所以对正奇数复合分母也有

\[
\left(\frac5r\right)
=\left(\frac r5\right)=1.
\tag{7.4}
\]

把 (4.1) 模 (r) 并取 Jacobi 符号：

\[
\left(\frac{-1}{r}\right)
=\left(\frac2r\right)^{2a+m}
 \left(\frac5r\right)^{m-h}.
\tag{7.5}
\]

这里 (m-h\ge0)，且 (7.3) 给

\[
\left(\frac2r\right)=1.
\]

于是

\[
\left(\frac{-1}{r}\right)=1.
\]

结合 (r\equiv\pm1\pmod8)，严格得到

\[
\boxed{r\equiv1\pmod8,\qquad k\equiv1\pmod8.}
\tag{7.6}
\]

该论证允许 (r) 为任意正奇复合数，不假设素数或平方自由；它只锁定
符号类，不产生立即矛盾。

---

## 8. 二进、五进提升类

第 6、7 节给出两个二进原型。

在主室 (\mathrm P_2) 中，(\alpha=2a) 且 (k\equiv1\pmod8)，
故

\[
v_2(k-1)=2a-1.
\]

写

\[
k=1+2^{2a-1}u_2',\qquad u_2'\text{ 奇}.
\]

而 (Z=2^{2a-1}z)，(z) 为奇数，所以

\[
\boxed{r\equiv1\pmod{2^{2a}}.}
\tag{8.1}
\]

在异常室 (\mathrm E_2) 中，

\[
v_2(k-1)=\alpha-1\ge4a+1,
\]

故

\[
\boxed{
r\equiv1+2^{2a-1}\pmod{2^{2a}}.
}
\tag{8.2}
\]

五进方面，(6.20) 给唯一符号 (\sigma_5\in\{\pm1\}) 使

\[
k=\sigma_5+5^{2\varphi}u_5,qquad5\nmid u_5.
\tag{8.3}
\]

若 (\varphi\le a)，则 (\zeta=3a-\varphi\ge2\varphi)，所以

\[
\boxed{r\equiv\sigma_5\pmod{5^{2\varphi}}.}
\tag{8.4}
\]

若 (\varphi>a)，则 (\zeta<2\varphi)，从而

\[
\boxed{v_5(r-\sigma_5)=\zeta=3a-\varphi.}
\tag{8.5}
\]

因此对固定 ((a,h,\varphi,J))，(r) 落入有限个二进—五进 CRT
原型。但当 (\varphi<a) 时，(8.4) 到完整窗口模数之间仍有深度

\[
\zeta-2\varphi=3(a-\varphi)
\tag{8.6}
\]

的五进自由提升。该深度随 (a-\varphi) 无界，正是本文不能把高层
误报成有限提升族的第一个障碍。

---

## 9. 归一化曲线与统一指数截断

完整球面和拼接方程为

\[
t^2=(d5^ea_1)^2+(2da_2)^2+a_3^2,
\tag{9.1}
\]

\[
Y(a_1T+10a_2)+a_3=kt.
\tag{9.2}
\]

令

\[
X=10^m,\qquad y=a_2,
\]

\[
P=Ya_1X+a_3,qquad
S=(d5^ea_1)^2+a_3^2.
\tag{9.3}
\]

把 (9.1)–(9.2) 视为关于 (y) 的二次方程，其判别式逐项化简为

\[
\operatorname{Disc}_y
=(4dk)^2
\left[P^2-(k^2-100Z^2)S\right],
\tag{9.4}
\]

这里使用 (Y=2dZ)。若整数 (y) 存在，则括号必须是整数平方：

\[
\boxed{
z^2=P^2-(k^2-100Z^2)S,qquad z\in\mathbb Z_{\ge0}.
}
\tag{9.5}
\]

因为 (k) 为奇数而 (10Z) 为偶数，

\[
k^2-100Z^2\ne0.
\tag{9.6}
\]

若 (k^2>100Z^2)，则

\[
(P-z)(P+z)=(k^2-100Z^2)S,
\]

所以右边至少为 (P)。若 (k^2<100Z^2)，则

\[
(z-P)(z+P)=(100Z^2-k^2)S,
\]

右边甚至至少为 (2P+1)。统一得到

\[
\boxed{
|k^2-100Z^2|S>P.
}
\tag{9.7}
\]

由 (k<21Z)，

\[
|k^2-100Z^2|<341Z^2.
\tag{9.8}
\]

又因 (b_3=2d5^e<Y)、(a_1\le13)、(a_3<10Y)，

\[
S<\left(\frac{13Y}{2}\right)^2+(10Y)^2
=\frac{569}{4}Y^2.
\tag{9.9}
\]

同时

\[
P>5YX.
\tag{9.10}
\]

将 (9.8)–(9.10) 代入 (9.7)，得到全部完整候选的统一必要上界

\[
\boxed{
10^m<\frac{194029}{20}Z^2Y.
}
\tag{9.11}
\]

利用 (Z\le10\cdot5^e)、(Y=10^{3a})，还可写成

\[
\boxed{
m<3a+2e\log_{10}5+
\log_{10}(970145).
}
\tag{9.12}
\]

这一步有两个重要后果。

1. 对每个固定终端种子，(4.10) 的无界指数级数只剩有限个初项；
2. 但右端仍随 (a,e) 线性增长，所以 (9.12) 不给 (a) 绝对上界。

因此固定模数上的周期没有被误写成全体参数有限；相反，完整判别式把每条
固定级数截成有限段，但全体模数 (r) 仍随 (a) 移动。

---

## 10. (a=2) 完整有限层

### 10.1 严格参数范围

当 (a=2) 时，(3.4) 给

\[
\boxed{h\in\{0,1\}.}
\tag{10.1}
\]

裸大小门给

\[
1\le\varphi\le5,qquad e=6+h-\varphi.
\tag{10.2}
\]

生成器先按 (10.1)–(10.2) 枚举全部严格窗口，再依次检查：

1. (\gcd(r,10)=1)；
2. (d\mid k^2-1)；
3. 真实 (M_r=\operatorname{ord}_r(10)) 与 (4.6) 的完整离散对数；
4. (m\ge\max(2,e)) 与 (s>0) 的唯一单调初端；
5. (\beta=2\varphi)；
6. 二进主室或异常室；
7. 修正后的 Jacobi 类；
8. (6.22) 与主室模 (8) 平方门。

精确计数为

\[
\begin{array}{c|r}
\text{阶段}&\text{状态数}\\ \hline
\text{严格窗口整数}&1{,}124{,}550\\
\gcd(r,10)=1&449{,}856\\
d\mid k^2-1&187{,}500\\
\text{完整乘法轨道有解}&38{,}220\\
\text{二、五进尺度室}&1{,}155\\
\text{Jacobi 与最低模后}&295
\end{array}
\tag{10.3}
\]

最后 295 行中：

\[
278\text{ 行属于主室},\qquad17\text{ 行属于异常室},
\tag{10.4}
\]

\[
\boxed{50\le m_*\le245{,}955.}
\tag{10.5}
\]

独立验证器不使用生成器的残数时间戳表，而以单独的哈希表 BSGS
重建乘法轨道，再逐行比较规范集合。验证输出为

```text
independently verified a=2 certificate: rows=295 primary=278 exceptional=17 min_m=50 max_m=245955
```

### 10.2 统一间隙关闭

对 (a=2)，有

\[
Y=10^6,qquad Z\le25{,}000.
\]

由 (9.11)，任何完整候选必须满足

\[
10^m<\frac{194029}{20}(25{,}000)^2\cdot10^6
=6{,}063{,}406{,}250{,}000{,}000{,}000
<10^{19}.
\]

所以

\[
\boxed{m\le18.}
\tag{10.6}
\]

这与证书的统一初端 (m\ge50) 矛盾。因此

\[
\boxed{
a=2\Longrightarrow\text{无 A2 单位行列式候选}.
}
\tag{10.7}
\]

该结论覆盖 295 条级数的全部 (t\ge0)，不是只检查有限个 (m)。
由于矛盾已经发生在完整球面—拼接必要判别式，两个恢复符号、全部五个
首块、全部真实 (a_2,a_3) 窗口及其后的 (a_3\mid Q)、
(K^{(10)}\mid L_\varepsilon)、逐项既约和原题回代都被统一覆盖；
不存在“只检查判别式平方”的充分性误报。

规范文件及 SHA-256：

```text
critical_G_A2_a2_certificate.csv
e7948a4698fd3208f1a4112e58c672a00b665440edf51eacad5dc75083e2b776

critical_G_A2_a2_generator.cpp
2897b6a6eb06131a31bb1144e82eac03fea4585b25c9f041ca198cee48d87ab0

critical_G_A2_a2_verifier.cpp
cb49205c30d47d950f9682a93ccdecef81e7be76afbcf88792d870f05b469060
```

---

## 11. 高层终端系统与准确停止点

由第 10 节，从此可假设

\[
a\ge3.
\tag{11.1}
\]

全部剩余候选必须按以下顺序生成。

1. 取 (a\ge3)；
2. 取 (h\in\mathcal H(a))，每个 (a) 至多两个；
3. 取
   
   \[
   1\le\varphi<a+\frac{C_a}{3};
   \tag{11.2}
   \]
4. 置
   
   \[
   e=3a+h-\varphi,quad
   Z=2^{2a-1}5^{3a-\varphi},quad
   d=2^a5^\varphi;
   \tag{11.3}
   \]
5. 取 (J\in\{1,\ldots,9\})，并取严格窗口中的 (r)，满足
   (8.1) 或 (8.2)、(8.4) 或 (8.5)；
6. 置 (k=r+Z)，检查
   
   \[
   v_5(k^2-1)=2\varphi,
   \quad
   \frac{k^2-1}{5^{2\varphi}}\equiv1,4\pmod5,
   \tag{11.4}
   \]
   
   以及二进主室或异常室；
7. 只取满足
   
   \[
   \max(2,e)\le m<
   \log_{10}\!\left(\frac{194029}{20}Z^2Y\right)
   \tag{11.5}
   \]
   
   且
   
   \[
   r\mid1+2^{2a+m}5^{m-h}
   \tag{11.6}
   \]
   
   的整数 (m)；
8. 用 (2.7)–(2.9) 恢复 (q,s,\rho_0)，核对初端门；
9. 最后进入 (6.1)、两个 (L_\varepsilon)、精确 gcd 尺度和完整回代。

由于 (11.5)，固定 ((a,h,\varphi,J,r)) 后不再有无界 (m)；可以
直接枚举有限区间，而不必把 (4.10) 的完整周期当作无限曲线。但是：

\[
\boxed{a\text{ 仍未绝对有界}.}
\tag{11.7}
\]

当 (\varphi<a) 时，(8.6) 的五进提升深度仍随 (a-\varphi)
无界；现有链条没有把这些 (r) 压成有限个固定递推。故：

- (r) 只落入有限种局部 CRT 原型，不落入已证明的有限全局提升族；
- 固定 (r) 后 (m) 原本是一条指数级数，但 (9.11) 只保留有限初段；
- 没有统一 Jacobi、LTE 或大小矛盾关闭全部 (a\ge3)；
- 没有资格建立有限种子级二维周期证书。

这就是本轮的准确停止点。

---

## 12. 完整恢复、主动反例攻击与审计

### 12.1 仍开放高层的完整恢复门

对第 11 节产生的状态，仍须取

\[
a_1\in\{5,7,9,11,13\},qquad
10^{m-2}\le a_2<10^{m-1},
\]

检查 (6.1) 为平方，并对两个符号定义

\[
L_\varepsilon=2ZH_1+\varepsilon kw_0.
\]

完整候选必须满足

\[
\gcd(K,L_\varepsilon)=\frac Kd,
\tag{12.1}
\]

\[
a_3=\frac{dL_\varepsilon}{K}in[Y,10Y),
\tag{12.2}
\]

\[
a_3\mid Q,qquad K^{(10)}\mid L_\varepsilon,
\tag{12.3}
\]

以及三个逐项既约、全部数字块窗口、完整球面方程和原拼接等式直接回代。
本文没有把 (6.1) 平方或任一局部赋值室写成充分条件。

### 12.2 对题设 Jacobi 草案的攻击

式 (7.1) 是具体漏洞。正确证明依赖第 6.3 节先推出
(v_2(K)\ge4)，而不能直接从 (a\ge3)、(2^a\mid K) 推出。
修复后 Jacobi 结论 (7.6) 成立，但只锁定正号类，不关闭高层。

### 12.3 对 (\alpha=2a) 的攻击

最低赋值唯一时确有 (\alpha=2a)，但当

\[
\alpha\ge4a+2v_2(H_1)
\]

时，两个恢复符号中一个可发生高阶消去。忽略该室会非法删除潜在候选。
第 6.3 节已经给出全部允许赋值关系；本文没有用有限样本声称异常室为空。

### 12.4 对五进异常室的攻击

五进与二进不同。式 (6.17) 先用终端大小门严格证明

\[
\beta<2v_5(A),
\]

所以五进不存在同层或反向最低赋值室；(6.20) 是完整结论，不是预设。

### 12.5 对固定周期误报的攻击

固定 (r) 的确只有一个 (m\bmod M_r) 类，但 (r) 随 (a)
移动。第 11 节没有把所有 (M_r) 合并成一个伪造的公共周期；
相反，(9.11) 只逐种子截断指数。

### 12.6 对 (a=2) 有限试验误报的攻击

机器只承担严格有限终端集合的重建。关闭 295 条无界级数的是统一符号
不等式 (m\le18<m_*\)，不是对若干 (m) 的试验。

### 12.7 是否发现继承错误

没有发现 PR6、SD6 或 GA1-1 的错误。本文发现并修复的是题设本轮草案中
尚未被冻结的模 (8) 推理 (7.1)，因此不分类为 GA2-5。

---

## 13. 最终分类与 (G) 模板最新状态

### 13.1 已严格完成

本文严格证明：

1. A2 尾窗每个 (a) 至多两个规范 (h)，但 (a) 未因此有限；
2. 终端状态与 ((q,r,s,\rho_0,J,k)) 完全双向；
3. 固定终端模数的全部指数是一条真实 (M_r) 级数；
4. (\varphi=3a) 不可能，且 (1\le\varphi\le3a-1)、(e\ge1)；
5. 五进尺度完全锁定为
   
   \[
   v_5(k^2-1)=2\varphi;
   \]
6. 二进尺度完整二分为
   
   \[
   \alpha=2a
   \quad\text{或}\quad
   \alpha\ge4a+2v_2(H_1);
   \]
7. 修正后的 Jacobi 锁定为 (r\equiv k\equiv1\pmod8)；
8. 完整判别式给出统一指数截断 (9.11)；
9. (a=2) 的完整有限层无候选。

### 13.2 为什么不是 GA2-1

没有关闭全部 (a\ge3) 高层。

### 13.3 为什么不是 GA2-2

(a) 未有绝对上界；全体 (r) 模数没有化为有限种子表。

### 13.4 为什么不是 GA2-3

虽然二进、五进只有有限个局部 CRT 原型，但当 (\varphi<a) 时仍有
深度 (3(a-\varphi)) 的移动五进提升。本文没有给出把这些提升统一递推
为有限族的双向定理，也没有覆盖所有 (a) 的完整周期证书。

### 13.5 为什么不是 GA2-4 或 GA2-5

没有找到合法原题六元组；也没有发现 PR6、SD6 或 GA1-1 的继承错误。

### 13.6 最终分类

按题设给定的互斥标签，只能取

\[
\boxed{
\mathrm{GA2\text{-}6}:
\quad
a=2\text{ 已关闭，尺度和指数获得强必要压缩，}
\text{但高层尚未全局有限化}.
}
\tag{13.1}
\]

### 13.7 (G) 模板最新状态

截至本文：

\[
\boxed{
G_{\mathrm{prim}},\ \gamma=1,\ \mathrm{A1}
\text{ 已由 GA1-1 关闭};
}
\]

\[
\boxed{
G_{\mathrm{prim}},\ \gamma=1,\ \mathrm{A2},\ a=2
\text{ 已由本文关闭};
}

\[
\boxed{
G_{\mathrm{prim}},\ \gamma=1,\ \mathrm{A2},\ a\ge3
\text{ 保持开放，但必须满足第 11、12 节系统}.
}

未研究并保持原状态：B、C 的 (\gamma=1) 分支、全部
(\gamma>1)、非本原 C2/C5、Q 和严格层。

本文到此停止。

---

## 14. 后继状态说明：GE2-1 删除异常二进室

日期：2026-08-06（Asia/Tokyo）

本节记录后继报告
`critical_G_A2_exceptional_binary_resolution.md` 的严格加强；原第 6.3 节的
分室推导仍然正确，但第 11、13 节把 \(\mathrm E_2\) 保留为开放必要室的
状态已被本节取代。

沿用

\[
\mathcal A=2ZH_1,qquad
R=(5^ea_1)^2+(2a_2)^2,qquad
K=k^2-1,
\]

\[
w_0^2=\mathcal A^2-KR,qquad
L_\varepsilon=\mathcal A+\varepsilon kw_0.
\]

若符号 \(\varepsilon\) 完成尺度恢复，则

\[
d=\frac K{\gcd(K,L_\varepsilon)}=2^a5^\varphi
\]

精确强迫

\[
v_2(L_\varepsilon)=\alpha-a,
\qquad \alpha=v_2(K).
\tag{14.1}
\]

异常室 \(\alpha\ge2A_2\)、\(A_2=v_2(\mathcal A)=2a+u_2\)
使 \(2^{A_2}\) 同时整除 \(L_+\) 和 \(L_-\)。另一方面，完整乘积

\[
L_+L_-=K(k^2R-\mathcal A^2)
\]

中的第二因子为奇数，故

\[
v_2(L_+)+v_2(L_-)=\alpha.
\]

与 (14.1) 联合得到

\[
v_2(L_{-\varepsilon})=a.
\]

但异常室又要求

\[
v_2(L_{-\varepsilon})\ge A_2=2a+u_2>a,
\]

矛盾。因此后继结论为

\[
\boxed{
\mathrm E_2\Longrightarrow\text{无完整候选}.
}
\tag{14.2}
\]

结合第 6.3 节已经证明的完备二分，A2 的完整二进尺度关系升级为

\[
\boxed{v_2(k^2-1)=2a.}
\tag{14.3}
\]

这不依赖 \(\varphi\ge a\)、五进提升、终端因子、指数级数或有限枚举；
\(\alpha=2A_2\)、\(\alpha>2A_2\) 与 \(w_0=0\) 均已在 GE2-1 中
逐项审计。故 GA2-6 的原推导不是错误，而是保留了一个尚未结合乘积恒等式
删除的过宽必要室。

最新 A2 状态应读为：\(a=2\) 仍由第 10 节关闭；全部完整 A2 候选若存在，
只能位于主二进室 \(\mathrm P_2\)。本节不关闭主二进室，也不对 B、C、
\(\gamma>1\)、非本原 C2/C5、Q 或严格层作结论。
