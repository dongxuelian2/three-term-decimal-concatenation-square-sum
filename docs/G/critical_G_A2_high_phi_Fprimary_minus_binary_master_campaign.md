# 三项十进制拼接平方和问题：临界 G 模板 A2 高 \(\varphi\) 主二进室负符号族统一二进 Bezout 塔报告

日期：2026-08-07（Asia/Tokyo）

本文严格限定于

\[
\boxed{
\mathcal F_{P-},\qquad
a\ge3,\qquad 0\le t<\frac a2,\qquad
h\in\mathcal H(a),\qquad J\in\{1,\ldots,9\}.
}
\]

低 \(\varphi\) 的 GALMB-3 在本文中完全冻结。GE2-1 也完全冻结；全文始终
保留

\[
\boxed{v_2(k^2-1)=2a.}
\]

本文接受 GFPmR-3、GFPmZ-6、GFPmP0-3、GFPmP1-3 中已经证明的双向
正规形，但独立重建其中全部移动二进高位数据。本文不研究 B、C、
\(\gamma>1\)、非本原 C2/C5、Q、严格层或任何低 \(\varphi\) 分支。

---

## 0. 裁决

本轮没有证明

\[
\mathcal F_{P-}\Longrightarrow\text{无候选}.
\]

也没有关闭 \(\mathscr P_0\)、\(\mathscr P_1\) 或六条零商族中的一个完整
大类。但是，本轮严格完成了以下统一化。

1. 建立标准二进逆元—Bezout 塔
   \[
   Y_s(n)=\langle5^{-n}\rangle_{2^s}^{+},\qquad
   D_s(n)=\frac{5^nY_s(n)-1}{2^s},
   \]
   并证明逐 bit、整块及反向提升公式。
2. 证明全部继承基坐标都来自同一个塔点：若
   \(s_0=2a-1\)，则
   \[
   x=2Y_{s_0}(c_0),\qquad c=D_{s_0}(c_0).
   \]
3. 证明深度零零商读取的是
   \(\mathfrak e_{s_0,s_0}(c_0)\)；平方 Bezout 对、P1 的
   \(\delta_1\) 和两个深度一零商读取的是同一块的平方。
4. 证明 P0 的逆元不是第三种数据。若
   \(v=c_0-F\)，则
   \[
   I_{a,t,F}
   =\left\langle5^vY_{2s_0}(2c_0)\right\rangle_{2^{2s_0}}^{+}.
   \]
5. 对深度 \(2,3\)，用 \(r=1+MD\) 的有限几何级数把
   \(r^{-1}\) 完全消去；所需 \(n_d,\theta_d\) 都成为上述标准塔点与
   \(J\) 的有限整数代数函数，不再重新求模 \(M^{d+1}\) 的逆元。
6. P0 被严格改写为长度 \(2a\) 的零字，P1 被严格改写为由五进低块指定
   一个长度 \(2a\) 的二进字，六条零商族被严格改写为同一塔的一个块字、
   一个平方块字以及两个有限几何读出字。

有限精确诊断覆盖 \(3\le a\le500\)，没有发现任何接受态；但该前缀不承担
无界证明。没有得到固定有限状态集合、完整周期覆盖或绝对有限的 \(a\) 上界。
因此准确分类为

\[
\boxed{
\mathrm{GFPmB\text{-}4}:
\quad
\mathscr Z,\mathscr P_0,\mathscr P_1
\text{ 已统一为一个二进逆元—Bezout 塔的不同窗口，}
\text{但比例长度禁字尚未证明。}
}
\]

本文还发现 GFPmP1-3 的式 (1.10) 有一个局部排印错误：其中写成了

\[
r=\rho+BCJ.
\]

正确式为

\[
\boxed{r=\rho+BJ=\rho+MCJ.}
\]

同一报告从第 3 节起实际使用的是正确式 \(r=\rho+MCJ\)，全部平方 Bezout、
\(E_1\)、\(\delta_1\) 与恢复公式也使用正确式，故该排印错误不影响任何
后续定理。它不构成需要推翻继承链的 GFPmB-6。

---

## 1. 继承参数与固定行列式

置

\[
\boxed{
M=2^{2a},\qquad c_0=2a-t,\qquad
C=5^{c_0},\qquad B=MC.
}
\tag{1.1}
\]

保留

\[
x=\langle2C^{-1}\rangle_M,\qquad Cx=2+Mc,
\tag{1.2}
\]

\[
U=JM+x,\qquad D=CJ+c,
\tag{1.3}
\]

从而

\[
\boxed{CU-MD=2,}
\tag{1.4}
\]

\[
\boxed{r=-1+CU=1+MD=\rho+BJ,}
\tag{1.5}
\]

其中

\[
\rho=Cx-1=1+Mc,\qquad \eta=cx,
\tag{1.6}
\]

\[
E_0=\eta+\rho J=cU+J=xD-J.
\tag{1.7}
\]

全部局部门、尾窗、严格提升界及正商边界仍按继承报告逐项检查；本文的塔公式
没有放大参数域。

---

## 2. 标准二进逆元—Bezout 塔

### 2.1 定义、正性与对偶代表

对 \(n\ge1,s\ge1\)，定义

\[
\boxed{
Y_s(n)=\left\langle5^{-n}\right\rangle_{2^s}^{+},
\qquad 1\le Y_s(n)<2^s,
}
\tag{2.1}
\]

\[
\boxed{
D_s(n)=\frac{5^nY_s(n)-1}{2^s}.
}
\tag{2.2}
\]

于是

\[
\boxed{5^nY_s(n)-2^sD_s(n)=1.}
\tag{2.3}
\]

因为 \(n\ge1\)，有 \(5^nY_s(n)>1\)，故 \(D_s(n)>0\)。又由
\(Y_s(n)<2^s\)，

\[
0<D_s(n)<5^n.
\tag{2.4}
\]

将 (2.3) 模 \(5^n\) 化简，并使用 (2.4) 的标准区间，得到对偶公式

\[
\boxed{
D_s(n)=\left\langle-2^{-s}\right\rangle_{5^n}^{+}.
}
\tag{2.5}
\]

因此 \(D_s(n)\) 恰是模 \(5^n\) 的 inverse-doubling 轨道，而不是一个
附加的任意商。

### 2.2 逐 bit 提升定理

定义

\[
\boxed{\varepsilon_s(n)=D_s(n)\bmod2\in\{0,1\}.}
\tag{2.6}
\]

则

\[
\boxed{Y_{s+1}(n)=Y_s(n)+\varepsilon_s(n)2^s,}
\tag{2.7}
\]

\[
\boxed{
D_{s+1}(n)=\frac{D_s(n)+\varepsilon_s(n)5^n}{2}.
}
\tag{2.8}
\]

**证明。** 候选提升只有 \(Y_s\) 与 \(Y_s+2^s\) 两个。由 (2.3)，

\[
5^n\bigl(Y_s+\varepsilon2^s\bigr)-1
=2^s(D_s+\varepsilon5^n).
\]

因 \(5^n\) 为奇数，右侧再被 \(2^{s+1}\) 整除，当且仅当
\(\varepsilon\equiv D_s\pmod2\)。这唯一给出 (2.6)–(2.7)，除以
\(2^{s+1}\) 得 (2.8)。新代表严格位于 \([1,2^{s+1})\)，故它就是标准
代表。

反向地，给定满足 (2.3) 的标准对 \((Y_s,D_s)\)，(2.6) 是唯一能使
\(D_s+\varepsilon5^n\) 为偶数的 bit；所以 (2.7)–(2.8) 唯一产生下一层
标准对。证毕。

特别地，

\[
\boxed{\text{逆元的下一二进数字}=\text{当前 Bezout 商的奇偶位}.}
\tag{2.9}
\]

### 2.3 整块提升

对 \(w\ge1\)，定义

\[
\boxed{
\mathfrak e_{s,w}(n)
=\frac{Y_{s+w}(n)-Y_s(n)}{2^s}
\in\{0,\ldots,2^w-1\}.
}
\tag{2.10}
\]

于是

\[
\boxed{Y_{s+w}(n)=Y_s(n)+2^s\mathfrak e_{s,w}(n).}
\tag{2.11}
\]

连续使用 (2.7) 立即证明 \(\mathfrak e_{s,w}\) 从低到高的二进数字恰为

\[
\varepsilon_s,\varepsilon_{s+1},\ldots,\varepsilon_{s+w-1}.
\tag{2.12}
\]

将精度 \(s\) 与 \(s+w\) 的两个 Bezout 恒等式相减，得到不逐 bit 的块公式

\[
\boxed{
D_s(n)+5^n\mathfrak e_{s,w}(n)=2^wD_{s+w}(n).
}
\tag{2.13}
\]

所以

\[
\boxed{
\mathfrak e_{s,w}(n)
\equiv-5^{-n}D_s(n)\pmod{2^w}.
}
\tag{2.14}
\]

这里的 \(5^{-n}\pmod{2^w}\) 准确指 \(Y_w(n)\)。因左边已经规定在
\([0,2^w)\)，还可写成完全显式的标准代表

\[
\boxed{
\mathfrak e_{s,w}(n)
=\left\langle-Y_w(n)D_s(n)\right\rangle_{2^w}.
}
\tag{2.15}
\]

### 2.4 长零字的五个严格等价形式

由 (2.10)–(2.13)，有

\[
\boxed{
\begin{aligned}
\mathfrak e_{s,w}(n)=0
&\Longleftrightarrow Y_{s+w}(n)=Y_s(n)\\
&\Longleftrightarrow 2^w\mid D_s(n)\\
&\Longleftrightarrow
v_2\bigl(5^nY_s(n)-1\bigr)\ge s+w.
\end{aligned}}
\tag{2.16}
\]

还有一个精确的对偶小区间形式。由 (2.5)，

\[
D_{s+w}(n)=\left\langle-2^{-(s+w)}\right\rangle_{5^n}^{+}.
\]

若零字成立，(2.13) 给 \(D_{s+w}=D_s/2^w<5^n/2^w\)。反之，若
\(D_{s+w}<5^n/2^w\)，则

\[
Y_{s+w}=\frac{1+2^{s+w}D_{s+w}}{5^n}<2^s+1.
\]

该整数为奇数，故不能等于偶数 \(2^s\)，于是 \(Y_{s+w}<2^s\)，标准
约化即给 \(Y_{s+w}=Y_s\)。因此

\[
\boxed{
\mathfrak e_{s,w}(n)=0
\Longleftrightarrow
\left\langle-2^{-(s+w)}\right\rangle_{5^n}^{+}
<\frac{5^n}{2^w}.
}
\tag{2.17}
\]

式 (2.17) 是反向 doubling orbit 的准确区间命中定理。

---

## 3. 全部高位数据的三个共同锚点

置

\[
\boxed{s_0=2a-1,\qquad 2s_0=4a-2.}
\tag{3.1}
\]

定义基础塔点

\[
y=Y_{s_0}(c_0),\qquad c_*=D_{s_0}(c_0).
\tag{3.2}
\]

由

\[
Cy-2^{s_0}c_*=1
\]

乘以 \(2\)，并用 \(2^{s_0+1}=M\)，得到

\[
C(2y)-Mc_*=2.
\]

与 (1.2) 的标准区间唯一性比较，严格得到

\[
\boxed{x=2y,\qquad c=c_*.}
\tag{3.3}
\]

所以继承的最初 Bezout 对本身就是标准塔的一层。

再定义共同高块

\[
\boxed{g=\mathfrak e_{s_0,s_0}(c_0),}
\tag{3.4}
\]

\[
\boxed{
z=Y_{2s_0}(c_0)=y+2^{s_0}g.
}
\tag{3.5}
\]

最后定义平方锚点

\[
\boxed{
\iota=Y_{2s_0}(2c_0)
=\left\langle z^2\right\rangle_{2^{2s_0}}^{+},
}
\tag{3.6}
\]

\[
\boxed{m_1=D_{2s_0}(2c_0).}
\tag{3.7}
\]

式 (3.6) 来自 \(5^{-2c_0}=(5^{-c_0})^2\)；右边是奇数，故不可能为
零代表。于是

\[
5^{2c_0}\iota-2^{2s_0}m_1=1.
\tag{3.8}
\]

注意

\[
2^{2s_0}=\frac{M^2}{4}.
\]

因此 GFPmZ-6、GFPmP0-3、GFPmP1-3 中看似不同的低精度逆元、平方
逆元和高位数字，实际上都从

\[
\boxed{(y,c),\qquad g,\qquad(\iota,m_1)}
\tag{3.9}
\]

这三个共同锚点读出。

---

## 4. P0：同一平方锚点的长零字

### 4.1 精确指数三角形

P0 中

\[
a+1\le F\le2a-t-1.
\]

定义边界距离

\[
u=F-a,\qquad v=c_0-F=2a-t-F.
\tag{4.1}
\]

则

\[
\boxed{u,v\ge1,\qquad u+v=a-t.}
\tag{4.2}
\]

P0 指数为

\[
\boxed{
n_0=c_0+F=3a-t+u=2c_0-v.
}
\tag{4.3}
\]

所以对固定 \((a,t)\)，精确整数区间为

\[
\boxed{3a+1-t\le n_0\le4a-2t-1.}
\tag{4.4}
\]

### 4.2 P0 与平方锚点的直接连接

由 \(n_0=2c_0-v\)，

\[
5^{-n_0}=5^v5^{-2c_0}.
\]

因此

\[
\boxed{
I_{a,t,F}=Y_{2s_0}(n_0)
=\left\langle5^v\iota\right\rangle_{2^{2s_0}}^{+}.
}
\tag{4.5}
\]

这证明 P0 的高精度逆元不是第三条独立逆元轨道；它是 P1/深度一共同平方
锚点 \(\iota\) 的有限 \(5\)-倍乘轨道，且

\[
1\le v\le a-t-1.
\tag{4.6}
\]

### 4.3 长零字定理

P0 的小区间上端为

\[
2^{2a-2}=2^{s_0-1}.
\]

置

\[
s_P=s_0-1=2a-2,
\qquad
w_P=s_0+1=2a.
\tag{4.7}
\]

则 \(s_P+w_P=2s_0=4a-2\)。因
\(Y_{s_P}(n_0)<2^{s_P}\)，标准代表唯一性给出

\[
\boxed{
1\le I_{a,t,F}\le2^{2a-2}-1
\Longleftrightarrow
Y_{2s_0}(n_0)=Y_{s_P}(n_0).
}
\tag{4.8}
\]

联合第 2.4 节，P0 接受门严格等价于

\[
\boxed{\mathfrak e_{2a-2,\,2a}(n_0)=0,}
\tag{4.9}
\]

\[
\boxed{2^{2a}\mid D_{2a-2}(n_0),}
\tag{4.10}
\]

\[
\boxed{
v_2\!\left(5^{n_0}Y_{2a-2}(n_0)-1\right)\ge4a-2,
}
\tag{4.11}
\]

以及对偶区间

\[
\boxed{
\left\langle-2^{-(4a-2)}\right\rangle_{5^{n_0}}^{+}
<\frac{5^{n_0}}{2^{2a}}.
}
\tag{4.12}
\]

这就是 P0 的统一“长度 \(2a\) 连续零提升字”标准形式。

### 4.4 P0 端点审计

1. \(D_{2a-2}(n_0)=0\) 不可能，因为 \(n_0>0\) 且
   \(5^{n_0}Y>1\)。
2. \(I=2^{2a-2}-1\) 不可能。任何 \(5^{-n_0}\) 的模 \(4\) 代表均为
   \(1\)，而 \(2^{2a-2}-1\equiv3\pmod4\)。
3. \(Y_{2a-2}(n_0)=1\) 也不可能。LTE 给
   \[
   v_2(5^{n_0}-1)=2+v_2(n_0).
   \]
   若代表为 \(1\)，则需 \(2^{2a-4}\mid n_0\)。当 \(a\ge5\) 时
   \(n_0\le4a-1<2^{2a-4}\)；当 \(a=3,4\) 时由 (4.4) 直接核对
   也无该整除。
4. \(F=a+1\) 对应 \(u=1,v=a-t-1\)，被 (4.2)–(4.12) 完整保留。
5. \(F=2a-t-1\) 对应 \(v=1\)，同样完整保留。

端点排除没有证明中间全部逆元都越过上端；P0 因而仍未关闭。

---

## 5. P1：同一平方锚点的指定字对齐

由 (3.6)–(3.8)，GFPmP1-3 的平方 Bezout 数据严格为

\[
\boxed{
\iota_1=\iota=Y_{2s_0}(2c_0),\qquad
n_1=4\iota,\qquad
m_1=D_{2s_0}(2c_0).
}
\tag{5.1}
\]

并且全部基坐标为

\[
\boxed{
x=2y,\quad c=D_{s_0}(c_0),\quad
U=JM+2y,\quad D=CJ+D_{s_0}(c_0).
}
\tag{5.2}
\]

所以 P1 的二进高位字有不含任何新逆元的闭式

\[
\boxed{
\delta_1
=\left\langle
\iota\bigl(D^2-m_1\bigr)
\right\rangle_M.
}
\tag{5.3}
\]

五进低块仍为

\[
\boxed{
e_5=
\left\langle-(4\iota+U^2)M^{-2}\right\rangle_{5^F}.
}
\tag{5.4}
\]

因此 P1 的 CRT 门严格改写为

\[
\boxed{
e_5\ne0,\qquad
e_5\equiv
\iota(D^2-m_1)\pmod M.
}
\tag{5.5}
\]

它的准确解释是：五进低块 \(e_5\) 指定一个长度 \(2a\) 的二进字，而
共同平方锚点 \((\iota,m_1)\) 与 \(J\) 产生的字 \(\delta_1\) 必须与之
相等。

### 5.1 不使用逆元黑箱的模 \(M^3\) 路径

因为 \(r=1+MD\)，

\[
(1+MD)^{-1}\equiv1-MD+M^2D^2\pmod{M^3}.
\tag{5.6}
\]

故 GFPmP1-3 中

\[
n_2=\left\langle U^2r^{-1}\right\rangle_{M^3}^{+}
\]

可直接写成

\[
\boxed{
n_2=
\left\langle
U^2(1-MD+M^2D^2)
\right\rangle_{M^3}^{+}.
}
\tag{5.7}
\]

其模 \(M^2\) 标准余数为 \(n_1=4\iota\)，所以

\[
\boxed{
\delta_1=\frac{n_2-4\iota}{M^2}\in\{0,\ldots,M-1\}.
}
\tag{5.8}
\]

式 (5.3) 与 (5.7)–(5.8) 是两条完全显式、彼此独立复核的路径；两条都只用
共同标准塔点及有限多项式，不再“重新求一个模 \(M^3\) 的逆元”。

### 5.2 边界

\(e_5=0\) 时正商窗口没有合法 \(\ell\)，必须立即拒绝；
\(\delta_1=0\) 本身不构成拒绝，只有与 (5.5) 联合时才决定状态。本文没有
把两个零边界混同。

---

## 6. 六条零商族：同一塔的四种有限读出

六室继续使用继承表

\[
\boxed{
\begin{array}{c|c|c|c}
(j,\epsilon)&d&A&F\\ \hline
(0,0)&0&2a-t+h+v_0&v_0\\
(1,0)&1&2a-t+h+v_0&v_0+t\\
(2,0)&2&2a-t+h+v_0&v_0+2t\\
(0,1)&1&h+v_0-t&v_0+t-2a\\
(1,1)&2&h+v_0-t&v_0+2t-2a\\
(2,1)&3&h+v_0-t&v_0+3t-2a
\end{array}}
\tag{6.1}
\]

其中

\[
\epsilon=0\iff v_0+(j+1)t<2a,
\qquad
\epsilon=1\iff v_0+(j+1)t\ge2a,
\tag{6.2}
\]

\[
0\le F<c_0,qquad A>0,qquad d=j+\epsilon\le3.
\tag{6.3}
\]

零商接受当且仅当继承余项

\[
E_d=2^A5^F.
\tag{6.4}
\]

### 6.1 深度零：共同块字本身

由 (3.5)，

\[
Y_{2s_0}(c_0)=Y_{s_0}(c_0)+2^{s_0}g.
\]

GFPmZ-6 的深度零提升式

\[
\frac y4=\frac x2+\frac J2\frac M2
\]

在当前记号中准确变成

\[
\boxed{
\mathscr Z_{0,0}Longrightarrow
J\in\{2,6\},\qquad
g=\mathfrak e_{s_0,s_0}(c_0)=\frac J2\in\{1,3\}.
}
\tag{6.5}
\]

这里模 \(M/2=2^{s_0}\) 到模 \(M^2/4=2^{2s_0}\) 的两位尺度差已经
被准确保留；没有把除以 \(2\) 写成模 \(M\) 的逆元。

### 6.2 深度一：共同块字的平方

由 (5.1) 定义

\[
p_1=\frac{Cn_1-2x}{M},\qquad
s_1=\frac{\rho n_1-x^2}{M^2}.
\tag{6.6}
\]

则

\[
\boxed{
C^2n_1-M^2m_1=4,
\qquad
p_1^2+4s_1=n_1m_1,
}
\tag{6.7}
\]

\[
\boxed{E_1=s_1+p_1J-J^2.}
\tag{6.8}
\]

因 \(n_1=4\iota\)，而 \(\iota\) 由 \(g\) 经 (3.5)–(3.6) 得到，
深度一两个室所需的 \(E_1\) 已完全成为同一塔的有限代数函数。准确接受方程为

\[
\boxed{
\begin{aligned}
\mathscr Z_{1,0}:\quad
&s_1+p_1J-J^2
=2^{2a-t+h+v_0}5^{v_0+t};\\
\mathscr Z_{0,1}:\quad
&s_1+p_1J-J^2
=2^{h+2a-2t+f}5^f,
\quad f=v_0+t-2a,\ 0\le f<t.
\end{aligned}}
\tag{6.9}
\]

### 6.3 深度二、三：有限几何读出

对 \(d\in\{2,3\}\)，定义

\[
\boxed{
G_d=\sum_{q=0}^{d}(-MD)^q.
}
\tag{6.10}
\]

因为

\[
(1+MD)G_d\equiv1\pmod{M^{d+1}},
\]

而 \(r=1+MD\)，GFPmZ-6 的

\[
n_d=\left\langle U^{d+1}r^{-1}\right\rangle_{M^{d+1}}^{+}
\]

可完全消去逆元黑箱，写成

\[
\boxed{
n_d=\left\langle U^{d+1}G_d\right\rangle_{M^{d+1}}^{+}.
}
\tag{6.11}
\]

定义当前 Bezout 商

\[
\boxed{
q_d=\frac{rn_d-U^{d+1}}{M^{d+1}}\in\mathbb Z.
}
\tag{6.12}
\]

下一 bit 为

\[
\boxed{\theta_d=q_d\bmod2.}
\tag{6.13}
\]

确实，\(n_d+\theta_dM^{d+1}\) 是
\(U^{d+1}r^{-1}\) 从模 \(M^{d+1}\) 提升到模 \(2M^{d+1}\) 的唯一
标准提升。在零商候选中 \(E_d=2^A5^F\) 且 \(A>0\)，所以 \(E_d\) 为
偶数；旧报告中的二值商

\[
K_d=n_d+\theta_dM^{d+1}
\]

恰满足这一下一 bit 条件。于是

\[
\boxed{
E_d=
\frac{r(n_d+\theta_dM^{d+1})-U^{d+1}}{M^{d+1}},
\qquad d=2,3.
}
\tag{6.14}
\]

式 (6.11)–(6.14) 中的 \(U,D,r\) 全由 (3.3)、(5.2) 和固定
\(J\in\{1,\ldots,9\}\) 生成。因此深度二、三也没有新的移动逆元。

三个室的接受条件就是把 (6.14) 分别与表 (6.1) 的
\((2,0),(1,1),(2,1)\) 行的 \(2^A5^F\) 相等。\(\theta_d=0,1\)
均被完整保留。

---

## 7. 八个残余族的共同窗口表

全部高位对象现在可汇总为下表。

| 残余族 | 塔指数 | 二进窗口或读出 | 接受字 |
|---|---:|---|---|
| \(\mathscr Z_{0,0}\) | \(c_0=2a-t\) | \(\mathfrak e_{s_0,s_0}(c_0)\) | \(J/2\in\{1,3\}\) |
| \(\mathscr Z_{1,0},\mathscr Z_{0,1}\) | \(2c_0=4a-2t\) | \(\iota=Y_{2s_0}(2c_0)\) 与 \(m_1\) | 固定二次型为指定 \((2,5)\)-单位 |
| \(\mathscr Z_{2,0},\mathscr Z_{1,1},\mathscr Z_{2,1}\) | 基指数仍为 \(c_0\) | \(r^{-1}\) 由长度 \(d+1\le4\) 的几何式读出 | \(\theta_d=q_d\bmod2\) 后等于指定 \((2,5)\)-单位 |
| \(\mathscr P_0\) | \(n_0=2c_0-v\) | \(\mathfrak e_{s_0-1,s_0+1}(n_0)\) | \(0^{2a}\) |
| \(\mathscr P_1\) | \(2c_0\) | \(\delta_1=\langle\iota(D^2-m_1)\rangle_M\) | \(e_5\bmod M\) 指定的字 |

其中

\[
c_0=2a-t,qquad
2c_0=4a-2t,qquad
n_0=2c_0-v,\qquad 1\le v\le a-t-1.
\tag{7.1}
\]

所以整个高位问题只涉及题设要求的线性指数

\[
\boxed{n=\alpha a+\beta t+\gamma F,}
\]

而且 P0 的三参数域已经缩成 (4.2) 的窄整数三角形。三种“神秘高位数字”
已经被消除：它们是同一固定 bit 动力系统的不同窗口、平方和有限几何读出。

---

## 8. P0 长零字攻击

### 8.1 inverse-doubling orbit

由 (2.5)，

\[
\boxed{2^sD_s(n)\equiv-1\pmod{5^n}.}
\tag{8.1}
\]

而 (2.8) 模 \(5^n\) 给

\[
D_{s+1}(n)\equiv2^{-1}D_s(n)\pmod{5^n}.
\tag{8.2}
\]

P0 因而严格等价于该轨道在时刻 \(4a-2\) 命中 (4.12) 的小区间。
若写

\[
D_{2a-2}(n_0)=2^{2a}q,
\]

则

\[
\boxed{
2^{4a-2}q+1=5^{n_0}Y_{2a-2}(n_0),
\qquad
0<q<\frac{5^{n_0}}{2^{2a}}.
}
\tag{8.3}
\]

这些界彼此相容；单纯比较两边大小不会产生矛盾。

### 8.2 stationary lift

P0 也严格等价于同一个小整数 \(Y_{2a-2}(n_0)\) 同时成为模
\(2^{4a-2}\) 的逆元，即 (4.11)。LTE 只能直接处理
\(Y=1\) 或另一个固定幂；这里 \(Y\) 随参数变化，并不属于固定的
\(2,5\)-单位集合。故 LTE 删除了第 4.4 节的端点，却没有删除全部中间代表。

### 8.3 \(5=1+4\) 的严格二项截断

在 \(\mathbb Z_2\) 中

\[
(1+4)^{-n}
=\sum_{j\ge0}(-1)^j\binom{n+j-1}{j}4^j.
\tag{8.4}
\]

从第 \(N\) 项起，每项都被 \(2^{2N}\) 整除，所以尾项严格属于
\(2^{2N}\mathbb Z_2\)；这里没有使用实数收敛。取
\(N=2a-1\)，得到模 \(2^{4a-2}\) 的完全有限式

\[
\boxed{
Y_{4a-2}(n)
=\left\langle
\sum_{j=0}^{2a-2}
(-1)^j\binom{n+j-1}{j}4^j
\right\rangle_{2^{4a-2}}^{+}.
}
\tag{8.5}
\]

式 (8.5) 给出严格余项赋值，但高半块由 \(2a-1\) 个整数项的全部进位共同
决定；现有二项赋值没有证明该高半块非零。把前若干项的规律外推会丢失后续
进位，不能作为证明。

### 8.4 二进对数路线

因 \(5^{-n}\equiv1\pmod4\)，stationary lift 可以在
\(1+4\mathbb Z_2\) 中写成

\[
n\log5+\log Y_{2a-2}(n)\equiv0\pmod{2^{4a-2}}.
\tag{8.6}
\]

对数级数第 \(j\) 项的二进赋值至少为 \(2j-v_2(j)\)，故可在任何指定
模数前作完全整数化截断。问题是第二个对数的整数
\(Y_{2a-2}(n)\) 本身随 \((a,t,F)\) 变化；(8.6) 不是两个固定代数数
对数的线性形式。当前材料没有从该可变项得到小于 \(4a-2\) 的统一赋值上界。

因此对数形式在本轮只重写了同一 stationary lift，没有关闭 P0。

---

## 9. 为什么当前递推还不是固定有限自动机

逐 bit 规则 (2.6)–(2.8) 的转移公式本身与 \(a\) 无关，但完整状态
\(D_s(n)\) 的位数增长。若只保存固定的

\[
D_s(n)\bmod2^k,qquad n\bmod T,
\]

则不能精确更新下一状态：两个商若相差 \(2^k\)，它们在模 \(2^k\) 下相同，
但经 (2.8) 除以 \(2\) 后相差 \(2^{k-1}\)，下一模 \(2^k\) 状态已经不同。
把精度改成 \(k+1\) 只把同一问题推迟一步；长度与 \(a\) 成比例的字需要成比例
的未读高位，除非再发现一个新的闭合不变量。

固定奇素数模 \(p\) 时，(2.8) 的确可由

\[
D_s\bmod p,\qquad n\bmod\operatorname{ord}_p(5)
\]

有限更新。但是 P0 接受门是 \(2^{2a}\mid D_{2a-2}\)，有限个奇模剩余
不能决定该二进整除；若没有额外大小界，有限奇素数 CRT 也不能把它升级成
双向排除。

因此本文建立的是一个固定**转移定律**和统一**窗口字典**，不是状态数与
\(a\) 无关的有限自动机。把完整 \(D_s\)、\(\iota\) 或 \(n_d\) 塞入状态会
违反固定状态要求。

---

## 10. 精确整数诊断（不承担无界证明）

独立整数程序按继承尾窗、\(t\) 初段、九个 \(J\) 局部门、正商区间和六室
指数表，完整检查 \(3\le a\le500\)。主要计数为

```text
P0 raw local states                  =   319995
P0 nonempty positive corridors      =   274866
P0 length-2a zero-word accepts      =        0
max v2(D_{2a-2}(n0))                =       16
required v2 for that maximum state  =      384

P1 nonempty positive corridors      =   274864
P1 e5 = 0 states                    =        0
P1 full binary high-digit accepts   =        0

six-Z room states                   =  1336288
six-Z reverse-replay accepts        =        0
Z00 prescribed-word hits            =        0
```

P0 的最大观测商赋值 \(16\) 出现在

\[
(a,t,F,n_0)=(192,0,308,692),
\]

而接受需要 \(2a=384\)。观测到的最小
\(I/2^{2a-2}\) 为

\[
\frac{373}{16}=23.3125
\]

（状态 \((a,t,h,J,F,n_0)=(3,0,1,4,5,11)\)）。这些间隙只属于有限
前缀。

P1 的低 bit 对齐计数为

```text
mod 2^3  matches = 34965
mod 2^5  matches =  8560
mod 2^8  matches =  1004
mod 2^12 matches =    58
mod 2^16 matches =     3
mod 2^17 matches =     0
```

所以模 \(8,16,32\) 明确不足以区分全部状态；模 \(2^{17}\) 只在该有限前缀
奏效，不能外推。最大共同低位长度为 \(16\)，出现在

\[
(a,t,h,J,F)=(332,0,285,9,593).
\]

深度 \(2,3\) 的 \(\theta_d=0,1\) 在该前缀中都实际出现：

```text
d=2: theta=0 -> 465, theta=1 -> 433
d=3: theta=0 -> 459, theta=1 -> 439
```

故不能通过预设某个固定 \(\theta_d\) 删除零商室。

这些数据只用于攻击公式、端点和固定小模猜想；本文没有据此制作周期证书。

---

## 11. 主动审计

| 项目 | 审计结果 |
|---|---|
| \(D_s=0\) | 对 \(n>0\) 不可能，见第 4.4 节 |
| \(Y_s=1\) | P0 参数域内由 LTE 与小端核对排除 |
| 连续零提升 bit | 与 \(2^w\mid D_s\) 严格双向，不是经验解释 |
| 块字全零 | 由 (2.16)–(2.17) 完整保留，尚未全局排除 |
| P0 上端 \(I=M/4-1\) | 模 \(4\) 排除 |
| \(F=a+1\) | 对应 \(u=1\)，完整保留 |
| \(F=2a-t-1\) | 对应 \(v=1\)，完整保留 |
| \(t=0\) | 全部公式合法；诊断最大商赋值也来自 \(t=0\) |
| \(a=3\) | 单独核对 P0 的 \(Y=1\) 端与正商小端 |
| P1 \(e_5=0\) | 立即拒绝，不以 \(5^F\) 替代零代表 |
| P1 \(\delta_1=0\) | 不单独拒绝，只通过 (5.5) 判断 |
| 零商 \(\theta_d=0,1\) | 两值都保留，且有限诊断中两值均出现 |
| \(J=1,9\) | 统一多项式读出没有删除端点 |
| \(\mathscr Z_{0,0}\), \(J=2,6\) | 精确成为共同块字 \(g=1,3\) |
| 模 \(M^2/4\) 与模 \(M^2\) | 以 \(s_0,2s_0\) 和 \(n_1=4\iota\) 分开处理 |
| 非法除以 \(2\) | \(x/2\) 只在模 \(M/2\) 解释，未当作模 \(M\) 逆元 |
| 固定深度与固定高位位置 | \(d\le3\) 只限制几何式长度，不把 bit 位置固定 |
| 有限前缀外推 | 明确禁止；第 10 节不承担无界结论 |
| “统一逆元塔”是否等于关闭 | 否；第 0、9、12 节均明确区分 |
| 旧公式错误 | 只发现 GFPmP1-3 (1.10) 的 \(BCJ\) 排印误差；后文使用正确式，无定理受影响 |

没有找到合法原题六元组，也没有发现 GFPmZ-6、GFPmP0-3、
GFPmP1-3 或上游系统中的实质性推导错误。

---

## 12. 最终分类与停止点

本轮严格证明的统一主链为

\[
\boxed{
\begin{gathered}
Y_{s+1}=Y_s+(D_s\bmod2)2^s,\qquad
D_{s+1}=\frac{D_s+(D_s\bmod2)5^n}{2},\\
D_s+5^n\mathfrak e_{s,w}=2^wD_{s+w},\\
x=2Y_{2a-1}(c_0),\qquad c=D_{2a-1}(c_0),\\
g=\mathfrak e_{2a-1,2a-1}(c_0),\\
\iota=Y_{4a-2}(2c_0)
=\left\langle
\bigl(Y_{2a-1}(c_0)+2^{2a-1}g\bigr)^2
\right\rangle_{2^{4a-2}}^{+},\\
I_{a,t,F}
=\left\langle5^{2a-t-F}\iota\right\rangle_{2^{4a-2}}^{+},\\
\delta_1=\left\langle\iota(D^2-D_{4a-2}(2c_0))\right\rangle_M,\\
n_d=\left\langle U^{d+1}\sum_{q=0}^{d}(-MD)^q
\right\rangle_{M^{d+1}}^{+},\quad d=2,3,\\
\theta_d=\left(
\frac{rn_d-U^{d+1}}{M^{d+1}}
\right)\bmod2.
\end{gathered}}
\tag{12.1}
\]

P0、P1 和六条零商族所需的不是三种不同移动逆元，而是 (12.1) 的不同
窗口及有限读出。由此，本轮已经完成唯一目标所允许的最低交付之一：

\[
\boxed{
\text{八个残余族的全部高位障碍统一成一个固定的二进逆元数字递推。}
}
\tag{12.2}
\]

但是，P0 的比例长度零字仍未被排除；P1 没有参数无关的小模分离定理；六条
零商族也没有固定有限状态的空接受图。故不能分类为 GFPmB-1、B-2 或 B-3。
排印修正不破坏继承结论，故也不分类为 B-6。

最终分类为

\[
\boxed{
\mathrm{GFPmB\text{-}4}:
\quad
\mathcal F_{P-}\text{ 的八个残余族获得统一二进 Bezout 塔和共同高位字正规形，}
\text{但仍有随 }a\text{ 移动的比例长度禁字残余。}
}
\]

没有得到固定有限自动机或周期覆盖，故不生成状态证书、独立验证器或 SHA-256
证书包。本文到此停止，不研究低 \(\varphi\)、B、C、\(\gamma>1\)、
非本原 C2/C5、Q 或严格层。
