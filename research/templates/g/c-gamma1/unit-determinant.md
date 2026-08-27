# 三项十进制拼接平方和问题：临界 (G) 模板本原 (gamma=1) 的 C 室单位行列式报告

日期：2026-08-07（Asia/Tokyo）

本文严格限定于

\[
\boxed{G_{\mathrm{prim}},\qquad \gamma=1,\qquad \mathrm C.}
\]

全文不返回 A、B、A2、低 \(\varphi\)、\(\gamma>1\)、非本原 C2/C5、
Q、O 或严格层。接受 GP3、CD6、PR6、SD6 与 E4 的 C1/C2/C3 室。

---

## 0. 裁决

本轮严格关闭整个 C3 室：

\[
\boxed{
G_{\mathrm{prim}},\ \gamma=1,\ \mathrm{C3}
\Longrightarrow\text{无完整候选}.
}
\tag{0.1}
\]

记该分支定理为

\[
\boxed{\mathrm{GC3\text{-}1}.}
\tag{0.2}
\]

C1、C2 尚未整体关闭，但二者都已与 C3 一起获得同一个双 Euclid 因子
走廊：

\[
\boxed{qr=1+10^A5^S=1+2^A5^{A+S}.}
\tag{0.3}
\]

所有自由的 \(s,\rho_0,k\) 均被消去；固定外层尺度与因子 \(q\) 后，
它们由

\[
s=5^R-Jq,\qquad
\rho_0=\frac{1+10^A5^S}{q}-JZ,\qquad
k=\frac{1+10^A5^S}{q}+Z
\tag{0.4}
\]

唯一恢复。

本轮还得到两个新的无界结构定理。

1. C2 的完整候选只能落入两条二进支路：
   \[
   \boxed{
   \begin{array}{ll}
   \eta_2=1,&A=2a-2,\quad q\equiv1\pmod{2^{a-1}},\\[1mm]
   \eta_2=2+v_2(R),&A=2a-3-v_2(R),\quad
   q\equiv-1\pmod{2^{a-1}}.
   \end{array}}
   \tag{0.5}
   \]
2. C1 写成 \(\eta_2=A+d\) 后，\(d\) 对每个外层状态有显式有限界，
   并且 \(W\) 与 \(r\) 分别落入有限奇数区间和单一 CRT 同余类。

因此最终分类为

\[
\boxed{
\mathrm{GCU\text{-}2}:
\quad \mathrm{C3}\text{ 完整关闭；}
\ \mathrm{C1},\mathrm{C2}\text{ 获得统一因子、二进与 CRT 走廊。}
}
\tag{0.6}
\]

没有找到合法原题六元组。

---

## 1. 继承系统与 C 本原边界

PR6 的本原 C 边界恰为

\[
\boxed{b_1=1,\qquad v=1,\qquad c=m,\qquad e<m.}
\tag{1.1}
\]

因此

\[
u=2^m5^e,\qquad R:=m-e\ge1,\qquad N=5^R,
\tag{1.2}
\]

\[
T=10^m=uN,
\tag{1.3}
\]

\[
b_2=uq,\qquad b_3=gu.
\tag{1.4}
\]

正余数正规形为

\[
N=Jq+s,\qquad J\in\{1,\ldots,9\},
\qquad1\le s<q,
\tag{1.5}
\]

\[
q\rho_0-E_0s=\gamma,
\qquad0<\rho_0<E_0.
\tag{1.6}
\]

全文只取 \(\gamma=1\)。

---

## 2. C 尺度的严格塌缩

在 C 中

\[
E=Y=2^n5^n,
\tag{2.1}
\]

而

\[
d=2^{\min(a,n)}5^{\min(\varphi,n)},
\qquad
g=2^a5^\varphi g_*,
\tag{2.2}
\]

其中 \(\gcd(g_*,10)=1\)。故

\[
\gamma=\frac gd
=2^{a-\min(a,n)}
5^{\varphi-\min(\varphi,n)}g_*.
\tag{2.3}
\]

三个因子均为正整数。由 \(\gamma=1\) 必须逐项有

\[
\boxed{g_*=1,\qquad a\le n,\qquad \varphi\le n.}
\tag{2.4}
\]

因此

\[
\boxed{d=g=2^a5^\varphi.}
\tag{2.5}
\]

定义

\[
A=n-a\ge0,\qquad F=n-\varphi\ge0,
\qquad\Delta=a-\varphi.
\tag{2.6}
\]

则

\[
F-A=\Delta,
\qquad F=A+\Delta,
\tag{2.7}
\]

\[
\boxed{Z=\frac{Y}{d}=2^A5^F
=2^A5^{A+\Delta}=10^A5^\Delta.}
\tag{2.8}
\]

式 (2.8) 的最后一种写法允许 \(\Delta<0\)，但整数定义始终是
\(Z=2^A5^F\)，且必须保留

\[
A\ge0,\qquad F=A+\Delta\ge0.
\tag{2.9}
\]

本轮从未假设 \(\varphi<a\) 或 \(\varphi\ge a\)。

---

## 3. 两个十进制窗口与尾窗定理

### 3.1 第二块

由 \(T=uN\)、\(b_2=uq\) 与

\[
\frac T{10}\le b_2<T
\]

得到

\[
\frac N{10}\le q<N.
\tag{3.1}
\]

再使用 \(N=Jq+s\)、\(1\le s<q\)，有

\[
Jq<N<(J+1)q.
\]

所以精确窗口为

\[
\boxed{
\frac{5^R}{J+1}<q<\frac{5^R}{J},
\qquad J\in\{1,\ldots,9\}.
}
\tag{3.2}
\]

两个端点均严格。

### 3.2 第三块

由 \(Y=dZ\)、\(b_3=du\) 与

\[
\frac Y{10}\le b_3<Y
\]

得到

\[
\boxed{\frac Z{10}\le u<Z,}
\tag{3.3}
\]

即

\[
\boxed{1<\frac Zu\le10.}
\tag{3.4}
\]

定义

\[
S=\Delta+R=a-\varphi+m-e.
\tag{3.5}
\]

由于 \(e=m-R\)，

\[
\frac Zu
=2^{A-m}5^{A+\Delta-e}
=2^{A-m}5^{A-m+S}
=10^{A-m}5^S.
\tag{3.6}
\]

故 (3.4) 等价于

\[
\boxed{10^{m-A}<5^S\le10^{m-A+1}.}
\tag{3.7}
\]

### 3.3 整数尾窗函数

定义唯一整数 \(H(S)\) 满足

\[
\boxed{10^{H(S)}<5^S\le10^{H(S)+1}.}
\tag{3.8}
\]

唯一性来自相邻十进制幂区间的互斥覆盖。比较只使用整数幂；不需要、也
不允许用浮点对数决定 \(H(S)\)。特别地，

\[
H(0)=-1,
\tag{3.9}
\]

并且对 \(t>0\)，

\[
\boxed{H(-t)=-H(t)-1.}
\tag{3.10}
\]

由 (3.7)–(3.8) 的唯一性，

\[
\boxed{m-A=H(S),\qquad m=A+H(S).}
\tag{3.11}
\]

因此

\[
\boxed{
e=A+H(S)-R,
\quad n=a+A,
\quad \varphi=a+R-S,
\quad F=A+S-R.
}
\tag{3.12}
\]

全部合法性条件为

\[
\boxed{
\begin{gathered}
a\ge1,\qquad A\ge0,\qquad R\ge1,\\
A+H(S)\ge2,\qquad A+H(S)\ge R,\\
a+R-S\ge0,\qquad A+S-R\ge0.
\end{gathered}}
\tag{3.13}
\]

这里分别对应 \(m\ge2,e\ge0,\varphi\ge0,F\ge0\)。

### 3.4 统一线性尾带

若 \(S>0\)，精确整数不等式

\[
5^{10}=9{,}765{,}625<10^7
\]

给出

\[
H(S)<\frac{7S}{10}.
\tag{3.14}
\]

由 \(R\le A+H(S)\) 与 \(S\le a+R\)，得到

\[
3R<10A+7a.
\tag{3.15}
\]

若 \(S\le0\)，则 \(H(S)\le-1\)，从而 \(R\le A-1\)，也满足
(3.15)。故全部 C 室统一满足

\[
\boxed{3R<10A+7a.}
\tag{3.16}
\]

这给每个固定 \((a,A)\) 的严格有限 \(R\)-带，但没有给 C1/C2 的
绝对 \(a\) 上界。

---

## 4. 双 Euclid 终端因子定理

PR6 在 \(\gamma=1\) 中给出

\[
q\rho_0-E_0s=1,
\tag{4.1}
\]

\[
qM_0-E_0N=1,
\tag{4.2}
\]

\[
qk-1=Z(q+N),
\tag{4.3}
\]

而 C 中 \(E_0=Z\)。定义

\[
r=M_0=k-Z.
\tag{4.4}
\]

则

\[
\boxed{qr-ZN=1,\qquad qr=1+ZN.}
\tag{4.5}
\]

又由 \(N=Jq+s\)、\(M_0=JZ+\rho_0\)，

\[
r=JZ+\rho_0,
\qquad JZ<r<(J+1)Z,
\tag{4.6}
\]

\[
(J+1)Z<k<(J+2)Z.
\tag{4.7}
\]

而

\[
ZN=2^A5^{F+R}=2^A5^{A+S}=10^A5^S.
\tag{4.8}
\]

即使 \(S<0\)，最后一式也是整数，因为

\[
A+S=F+R\ge1.
\tag{4.9}
\]

所以

\[
\boxed{qr=1+10^A5^S=1+2^A5^{A+S}.}
\tag{4.10}
\]

### 定理 4.1：终端因子走廊的真正双向性

固定满足 (3.13) 的 \((a,A,R,S,J)\)，并令

\[
N=5^R,\qquad Z=2^A5^{A+S-R},
\qquad P=1+10^A5^S.
\]

则以下两类对象一一对应：

1. 满足 (4.1)–(4.7) 与两个分母窗口的单位行列式终端状态；
2. 满足
   \[
   \boxed{q\mid P,\qquad q\text{ 为奇正因子},\qquad
   \frac{5^R}{J+1}<q<\frac{5^R}{J}}
   \tag{4.11}
   \]
   的因子 \(q\)。

正向由 (4.10) 与 (3.2) 立即得到。

反向令

\[
r=P/q,
\quad s=N-Jq,
\quad \rho_0=r-JZ,
\quad k=r+Z.
\tag{4.12}
\]

由 (4.11)，

\[
0<s<q,
\]

故 \(1\le s<q\)。又

\[
\frac rZ=\frac Nq+\frac1{qZ}>J.
\]

而

\[
(J+1)Z-r
=\frac{Z((J+1)q-N)-1}{q}
=\frac{Z(q-s)-1}{q}>0,
\]

其中最后一步使用合法尾窗给出的 \(Z>u\ge1\)，故 \(Z\ge2\)。因此

\[
0<\rho_0<Z.
\]

最后

\[
q\rho_0-Zs
=q(r-JZ)-Z(N-Jq)
=qr-ZN=1.
\tag{4.13}
\]

并且

\[
qk-1=q(r+Z)-1=Z(q+N).
\tag{4.14}
\]

所以恢复完全成立。

这里的“一一对应”只指单位行列式、Euclid 余数和两个分母窗口。E4 的
C1/C2/C3 赋值门、判别式、第三分子窗口与逐项既约仍须后置检查；不能把
(4.11) 单独称为原题候选。

---

## 5. Farey 关系与精确 CRT 走廊

由 \(qr-ZN=1\)，

\[
\boxed{
\frac rZ-\frac Nq=\frac1{qZ},
\qquad
J<\frac Nq<\frac rZ<J+1.
}
\tag{5.1}
\]

因此 \(N/q\) 与 \(r/Z\) 是同一整数商 \(J\) 下的相邻既约分数。
这本身不产生矛盾，但特殊分母给出两个同步同余。

令

\[
\eta_2=v_2(q+N).
\tag{5.2}
\]

则

\[
q\equiv-N\pmod{2^{\eta_2}}.
\]

把它代入 \(qr=1+ZN\)，得到

\[
\boxed{
r\equiv-Z-N^{-1}\pmod{2^{\eta_2}},
\qquad
k=r+Z\equiv-N^{-1}\pmod{2^{\eta_2}}.
}
\tag{5.3}

特别地，模 \(2^{\min(A,\eta_2)}\)，

\[
\boxed{r\equiv-5^{-R}\pmod{2^{\min(A,\eta_2)}}.}
\tag{5.4}
\]

另一方面，模 \(N=5^R\)，

\[
\boxed{r\equiv q^{-1}\pmod{5^R}.}
\tag{5.5}
\]

因为两个模数互素，(5.3)、(5.5) 唯一决定

\[
r\pmod{2^{\eta_2}5^R}.
\tag{5.6}
\]

再加 \(JZ<r<(J+1)Z\)，固定 \((q,\eta_2)\) 后的 CRT 候选数至多为

\[
\boxed{
\left\lceil\frac{Z-1}{2^{\eta_2}5^R}\right\rceil.
}
\tag{5.7}
\]

在 C1 中 \(\eta_2\ge A\)。若 \(F\le R\)，则

\[
Z=2^A5^F\le2^{\eta_2}5^R,
\]

故每个 \((q,\eta_2)\) 至多只有一个 CRT 代表。这是与 A2 的“固定
低块＋唯一 CRT corridor”最接近的 C 专用版本；若 \(F>R\)，走廊宽度
仍可随 \(F-R\) 增长，所以不能误报为全部 C1 的唯一性。

---

## 6. C1/C2/C3 的统一 A 坐标

定义

\[
\eta_2=v_2(q+5^R)\ge1,
\tag{6.1}
\]

\[
\lambda=v_2(kq-1).
\tag{6.2}
\]

由 \(qk-1=Z(q+N)\) 与 \(v_2(Z)=A\)，

\[
\boxed{\lambda=A+\eta_2.}
\tag{6.3}
\]

### 6.1 C1

E4 的

\[
\lambda<2\eta_2+1,
\qquad2a>n
\]

分别等价于

\[
A\le\eta_2,
\qquad A<a.
\]

所以

\[
\boxed{0\le A\le a-1,\qquad \eta_2\ge A.}
\tag{6.4}
\]

### 6.2 C3

由 \(n=2a\)、\(a=\eta_2+1\)、\(\lambda=2a-1\)，

\[
\boxed{A=a,\qquad\eta_2=a-1,\qquad\kappa=1.}
\tag{6.5}
\]

因为 \(\eta_2\ge1\)，C3 必有 \(a\ge2\)。

### 6.3 C2

由 \(\lambda=2a-1\) 与 \(a\ge\eta_2+2\)，

\[
\boxed{
a+1\le A\le2a-2,
\qquad
\eta_2=2a-1-A.
}
\tag{6.6}
\]

C2 非空必须有 \(a\ge3\)。

因此三个室确实形成连续 A 走廊

\[
\boxed{0\le A\le2a-2,}
\tag{6.7}
\]

其中 \(A<a,A=a,A>a\) 依次为 C1、C3、C2。该式只是完备
重参数化；只有 C3 在本轮被关闭。

---

## 7. 二进商 W 与 C1 的有限 d 走廊

令

\[
W=\frac{q+5^R}{2^{\eta_2}}.
\tag{7.1}
\]

则 \(W\) 为正奇数，且

\[
q=2^{\eta_2}W-5^R.
\tag{7.2}
\]

把 (3.2) 代入，得到严格开区间

\[
\boxed{
\frac{J+2}{J+1}\frac{5^R}{2^{\eta_2}}
<W<
\frac{J+1}{J}\frac{5^R}{2^{\eta_2}}.
}
\tag{7.3}
\]

区间长度为

\[
\boxed{\frac{5^R}{2^{\eta_2}J(J+1)}.}
\tag{7.4}
\]

故长度不超过 \(2\) 时至多含一个奇整数；一般 C2/C3 的 \(R\) 仍可
使该长度很大，所以不能无条件声称“每状态至多一个 W”。

在 C1 中写

\[
\eta_2=A+d,\qquad d\ge0,\qquad A+d\ge1.
\tag{7.5}
\]

由

\[
2^{\eta_2}W=q+5^R<2\cdot5^R
\]

得到精确整数界

\[
\boxed{
A\le\eta_2\le
\left\lfloor\log_2(2\cdot5^R-1)\right\rfloor,
}
\tag{7.6}
\]

其中右端在理论和代码中都由整数倍增比较确定。于是

\[
\boxed{
\max(0,1-A)\le d\le
\left\lfloor\log_2(2\cdot5^R-1)\right\rfloor-A.
}
\tag{7.7}
\]

固定 \(d\) 后，(7.3) 给出有限个显式奇 \(W\)；固定 \(W\) 后
\(q,r,s,\rho_0,k\) 全部唯一。随着 \(d\) 接近上端，区间只能容纳
很小的奇数，\(W=1\) 的精确条件为

\[
\boxed{
\frac{J+2}{J+1}5^R<2^{A+d}
<\frac{J+1}{J}5^R.
}
\tag{7.8}
\]

这完成了 C1 所要求的显式有限 corridor；但 \(R\) 随外层参数移动，
所以 \(d\) 尚无参数无关的绝对上界。

---

## 8. 完整尺度恢复带来的新二进刚性

令

\[
K=k^2-1.
\tag{8.1}
\]

SD6 的完整尺度恢复要求

\[
d=\frac{K}{\gcd(K,L_\varepsilon)}.
\tag{8.2}
\]

因此任何完整候选首先必须满足

\[
\boxed{d\mid K.}
\tag{8.3}
\]

### 8.1 C2/C3 的平方根门

在 C2/C3 中 \(A\ge a\)，所以 \(2^a\mid Z\)。由

\[
qr=1+ZN,qquad k=r+Z
\]

可得

\[
qk\equiv1\pmod{2^a}.
\tag{8.4}
\]

再由 \(2^a\mid K\)，

\[
k^2\equiv1\pmod{2^a}.
\]

将 (8.4) 平方，得到

\[
\boxed{q^2\equiv1\pmod{2^a}.}
\tag{8.5}
\]

当 \(a\ge3\) 时，模 \(2^a\) 的平方根分类给出

\[
\boxed{q\equiv\pm1\pmod{2^{a-1}}.}
\tag{8.6}
\]

### 8.2 C2 的两条支路

C2 中 \(1\le\eta_2\le a-2\)。

若 \(q\equiv1\pmod{2^{a-1}}\)，因为 \(5^R\equiv1\pmod4\)，

\[
\eta_2=v_2(q+5^R)=1.
\tag{8.7}
\]

若 \(q\equiv-1\pmod{2^{a-1}}\)，则

\[
\eta_2=v_2(5^R-1).
\]

LTE 对全部 \(R\ge1\) 给

\[
v_2(5^R-1)=2+v_2(R).
\tag{8.8}
\]

联合 \(A=2a-1-\eta_2\)，得到 (0.5)。因此 C2 的整个二维
\((A,\eta_2)\) 区第一次塌缩为两条显式支路，而不是任意移动高位数字。

### 8.3 判别式二进门

在 C 中

\[
\mathcal R=(ua_1)^2+a_2^2.
\]

因为 \(u\) 为偶数且 \(\gcd(a_2,b_2)=1\)，\(a_2\) 为奇数，故

\[
\mathcal R\text{ 为奇数}.
\tag{8.9}
\]

又

\[
H_1=a_1T+10a_2,
\qquad v_2(H_1)=1.
\tag{8.10}
\]

令

\[
\mathscr A=ZH_1,
\qquad B=v_2(\mathscr A)=A+1,
\qquad \alpha=v_2(K).
\tag{8.11}
\]

完整判别式为

\[
w_0^2=\mathscr A^2-K\mathcal R.
\tag{8.12}
\]

对 C2/C3，\(B>A\ge a\)。若 \(\alpha\ge2B\)，则平方性强迫
\(2^B\mid w_0\)，从而 \(2^B\mid L_+,L_-\)。但

\[
L_+L_-=KQ,
\qquad
Q=k^2\mathcal R-\mathscr A^2\text{ 为奇数}.
\]

尺度恢复又要求两个共轭因子的二进赋值为 \(\alpha-a\) 与 \(a\)，
其中一个恰为 \(a<B\)，矛盾。因此

\[
\boxed{\alpha<2(A+1).}
\tag{8.13}
\]

此时 (8.12) 的两项赋值不同，

\[
v_2(w_0^2)=\alpha.
\]

所以

\[
\boxed{
a\le\alpha<2(A+1),
\qquad \alpha\equiv0\pmod2
}
\tag{8.14}
\]

是 C2/C3 完整候选的统一必要条件。

---

## 9. C3 的绝对有限化与关闭

### 9.1 绝对外层界

C3 有

\[
A=a,\qquad \eta_2=a-1.
\]

对 \(a\ge3\)，(8.6) 与

\[
2^{a-1}\mid q+5^R
\]

排除正根号支路，并迫使

\[
5^R\equiv1\pmod{2^{a-1}}.
\]

由 (8.8)，

\[
\boxed{2^{a-3}\mid R.}
\tag{9.1}
\]

而 (3.16) 在 \(A=a\) 时给

\[
\boxed{3R<17a.}
\tag{9.2}
\]

若 \(a=9\)，(9.1) 给 \(R\ge64\)，(9.2) 给 \(R<51\)，矛盾。
此后 \(2^{a-3}\) 每步加倍，而 \(17a/3\) 的相邻比小于 \(2\)，故
矛盾保持。于是

\[
\boxed{2\le a\le8.}
\tag{9.3}
\]

连同

\[
1\le R\le\left\lfloor\frac{17a-1}{3}\right\rfloor,
\qquad R-a\le S\le a+R,
\tag{9.4}
\]

C3 成为绝对有限外层区域。

### 9.2 规范有限证书

独立生成器按以下顺序精确检查：

1. (9.3)–(9.4)；
2. 整数尾窗 (3.8) 与全部合法性条件；
3. 九个严格 \(J\)-窗口；
4. \(q\mid1+10^A5^S\) 的全部奇因子；
5. \(\eta_2=a-1\)；
6. \(d\mid K\)；
7. E4 的 \(\kappa=1\)；
8. 判别式与完整二进尺度门。

计数为

\[
\boxed{
2106\longrightarrow49\longrightarrow26\longrightarrow11\longrightarrow0.
}
\tag{9.5}
\]

最后 11 个状态如下。

| \(a\) | \(R\) | \(S\) | \(J\) | \(q\) | \(k\) | \(v_2(K)\) | 删除门 |
|---:|---:|---:|---:|---:|---:|---:|---|
| 2 | 4 | 5 | 9 | 69 | 5029 | 3 | 判别式赋值为奇数 |
| 2 | 5 | 6 | 2 | 1201 | 1801 | 4 | 归一化判别式 \(\equiv7\pmod8\) |
| 2 | 6 | 8 | 1 | 11069 | 6029 | 3 | 判别式赋值为奇数 |
| 2 | 8 | 10 | 1 | 308941 | 5661 | 3 | 判别式赋值为奇数 |
| 2 | 11 | 13 | 6 | 7998841 | 17761 | 6 | \(\alpha=2(A+1)\) 尺度溢出 |
| 3 | 2 | 5 | 8 | 3 | 1166667 | 3 | 判别式赋值为奇数 |
| 3 | 4 | 6 | 2 | 251 | 87251 | 3 | 判别式赋值为奇数 |
| 3 | 4 | 7 | 2 | 267 | 417603 | 3 | 判别式赋值为奇数 |
| 3 | 6 | 9 | 1 | 10147 | 317483 | 3 | 判别式赋值为奇数 |
| 3 | 6 | 9 | 7 | 1971 | 1115931 | 3 | 判别式赋值为奇数 |
| 3 | 15 | 18 | 8 | 3402750127 | 1246063 | 5 | 判别式赋值为奇数 |

九个奇赋值状态立即不可能为平方。尺度溢出状态由 (8.13) 删除。唯一
剩余的偶赋值状态满足 \(v_2(K)=4\)、\(v_2(\mathscr A)=3\)。除以
\(2^4\) 后，利用

\[
\mathcal R\equiv1\pmod8,
\qquad K/16\equiv5\pmod8,
\qquad \mathscr A^2/16\equiv4\pmod8,
\]

得到

\[
\frac{\mathscr A^2-K\mathcal R}{16}
\equiv7\pmod8,
\]

仍非平方。该计算与 \(a_1\in\{1,\ldots,8\}\) 及任意合法奇
\(a_2\) 无关，故不是有限遍历中分子块。

因此 (0.1) 得证。

证书验证同时包含六个破坏测试：删除一个因子、篡改 \(J\)、错误
\(H(S)\)、错误 C 室标签、错误判别式符号和把严格窗口改成相邻端点；
六项均被拒绝。

---

## 10. C2 的当前严格停止点

C2 尚未关闭。当前完备必要链为

\[
\boxed{
\begin{gathered}
a\ge3,\qquad a+1\le A\le2a-2,\\
3R<10A+7a,\qquad
R-A\le S\le a+R,\\
\eta_2=2a-1-A,\\
\eta_2=1\ \text{或}\ \eta_2=2+v_2(R),\\
q=2^{\eta_2}W-5^R,\quad W\text{ 为 (7.3) 中的奇数},\\
q\mid1+10^A5^S,\\
a\le v_2(k^2-1)<2(A+1),\quad v_2(k^2-1)\text{ 为偶数}.
\end{gathered}}
\tag{10.1}
\]

有限诊断 \(a\le5\) 中，C2 有

\[
7749\text{ 个合法外层状态},quad
474\text{ 个 E4 因子状态},quad
77\text{ 个满足 }d\mid K\text{ 的状态},
\]

单个外层状态最多出现 15 个因子。该数据只说明“每状态至多一个 W”在
一般 C2 中不成立；它不承担任何无界排除。

两条支路在任意 \(a\) 都有合法尾窗外层参数，因此 (10.1) 没有给
C2 的绝对 \(a\) 上界。完整判别式与第三块尺度恢复仍是下一道实质门。

---

## 11. C1 的当前严格停止点

C1 的统一正规形为

\[
\boxed{
\begin{gathered}
a\ge1,\qquad0\le A\le a-1,\\
3R<10A+7a,\qquad R-A\le S\le a+R,\\
\eta_2=A+d,\qquad d\text{ 满足 (7.7)},\\
W\text{ 为 (7.3) 中的奇数},\\
q=2^{A+d}W-5^R,\\
q\mid1+10^A5^S,\\
r\text{ 满足 (5.3)、(5.5) 与 }JZ<r<(J+1)Z.
\end{gathered}}
\tag{11.1}
\]

所以 C1 不再留下无结构的“移动高位二进数字”：高提升量 \(d\) 有显式
外层有限界；每个 \(d\) 的 \(W\) 位于显式奇数区间；每个 \(W\) 唯一
决定因子 \(q\)，而 \(r\) 落在单一 CRT 类。

有限诊断 \(a\le5\) 中，C1 有

\[
6183\text{ 个合法外层状态},quad
349\text{ 个 E4 因子状态},quad
57\text{ 个满足 }d\mid K\text{ 的状态},
\]

单个外层状态最多两个因子。仍然只作诊断，不外推。

---

## 12. 因子式的代数分解与 primitive-divisor 路线

写

\[
P=1+2^A5^{A+S},
\qquad g_0=\gcd(A,A+S).
\tag{12.1}
\]

若 \(g_0\) 含奇因子 \(d>1\)，令

\[
X=2^{A/d}5^{(A+S)/d}.
\]

则

\[
\boxed{P=X^d+1=(X+1)(X^{d-1}-X^{d-2}+\cdots-X+1).}
\tag{12.2}
\]

这是强制 cyclotomic 分解。但 \(q\) 只要求是 \(P\) 的窗口因子；其素
因子可以分配在 (12.2) 的两个因子之间，现有窗口并不强迫 \(X+1\) 或
任一 primitive prime divisor 整体进入 \(q\) 或整体进入 \(r\)。

因此不能从 Zsigmondy 型“存在新素数”直接推出该素数违反 \(q<5^R\) 或
\(r<(J+1)Z\)。本轮没有使用未审计例外的 primitive-divisor 结论，
也没有把数值中的大素因子现象升级为证明。

---

## 13. 完整判别式与第三块恢复

对每个通过终端因子走廊的状态，定义

\[
\mathcal R=(ua_1)^2+a_2^2,
\tag{13.1}
\]

\[
H_1=a_1T+10a_2,
\tag{13.2}
\]

其中

\[
a_1\in\{1,\ldots,8\},
\qquad10^{m-2}\le a_2<10^{m-1},
\qquad\gcd(a_2,uq)=1.
\tag{13.3}
\]

完整约化判别式为

\[
\boxed{w_0^2=Z^2H_1^2-K\mathcal R.}
\tag{13.4}
\]

置

\[
L_\pm=ZH_1\pm kw_0.
\tag{13.5}
\]

真正候选必须存在至少一个 \(L_\varepsilon>0\)，满足

\[
\boxed{
d=\frac K{\gcd(K,L_\varepsilon)},
\qquad
a_3=\frac{L_\varepsilon}{\gcd(K,L_\varepsilon)}
\in[Y,10Y).
}
\tag{13.6}
\]

同时保留 SD6 的互补尺度

\[
\boxed{
L_\varepsilon=\frac Kd a_3,
\qquad
L_{-\varepsilon}=d\mathscr R_3,
}
\tag{13.7}
\]

\[
\boxed{Ka_3+d^2\mathscr R_3=2YH_1.}
\tag{13.8}
\]

不得预设 \(L_-\) 为正；不得把 \(d\mid K\) 加强成 \(d^2\mid K\)；
不得仅凭判别式平方称为原题候选。最终还要检查

\[
\gcd(a_3,du)=1,
\]

原球面方程、拼接方程与全部数字块窗口。

C3 的关闭发生在 (13.4)–(13.8) 之前或之中，故已覆盖判别式平方、
\(w_0=0\)、负共轭因子及第三块尺度恢复。C1/C2 则仍须真正通过这层。

---

## 14. 主动审计

1. **\(A=0\)：** 允许，只出现在 C1；此时 \(P=1+5^S\) 为偶数，
   只取其奇因子 \(q\)，而 \(r\) 可以为偶数。
2. **\(F=0\)：** 保留；整数式使用 \(Z=2^A5^F\)。
3. **\(\Delta<0\)：** 保留；不把 \(10^A5^\Delta\) 单独当作整数定义。
4. **\(S=0\)：** \(H(0)=-1\)，没有误写成 \(0\)。
5. **\(H(S)<0\)：** 由 (3.13) 与其他指数联合判断，不预先删除。
6. **\(e=0\)、\(R=1\)：** 均在尾窗与证书中保留。
7. **\(a=n\)、\(\varphi=n\)：** 分别对应 \(A=0\)、\(F=0\)，均保留。
8. **C1 的 \(A=0\)：** (5.4) 退化为模 \(1\) 陈述，但完整 CRT
   (5.3)、(5.5) 仍有效。
9. **\(A=a-1,a\)：** 分别归 C1 与 C3；没有重叠。
10. **C3 小 \(a\)：** \(a=1\) 因 \(\eta_2\ge1\) 为空；证书从
    \(a=2\) 开始。
11. **C2 端点：** \(A=2a-2\) 正是 \(\eta_2=1\) 支路；
    \(A=a+1\) 只有满足 (0.5) 时才存活。
12. **\(W=1\)：** 未删除，精确条件为 (7.8)。
13. **\(J=1,9\)：** 因子定理、C3 证书均含两个端点商。
14. **\(q,r\) 窗口：** 全部端点严格；证书破坏测试专门检查。
15. **\(q=r\)：** 未预先排除；若出现，由因子枚举与后置门判断。
16. **共轭符号：** 只要求至少一个 \(L_\varepsilon>0\)；不预设
    \(L_->0\)。
17. **\(w_0=0\)：** 包含在判别式和尺度溢出证明中。
18. **平方但恢复失败：** 按 (13.6) 删除，不误报为候选。
19. **第三块端点：** \(a_3=Y\) 允许，\(a_3=10Y\) 禁止。
20. **终端状态与原题候选：** (4.11) 只是一道分母终端门。
21. **重参数化与关闭：** (6.7) 不是关闭；只有 GC3-1 是本轮新关闭。

---

## 15. 文件、验证与最终状态

本报告配套：

- `generate_G_C3_factor_certificate.py`：独立生成 C3 规范证书；
- `verify_G_C3_factor_certificate.py`：不导入生成器的验证器；
- `critical_G_C3_terminal_certificate.json`：规范证书；
- `critical_G_C3_terminal_certificate.sha256`：SHA-256。

验证命令：

```bash
python3 verify_G_C3_factor_certificate.py --destruction-tests
```

规范证书 SHA-256：

```text
c0e67cbd97bd5b0dc4471b491cf380d0379813384f29a4af9a170119f0856e9d
```

最终状态为

\[
\boxed{
\begin{array}{c|c}
\mathrm{C3}&\text{由 GC3-1 完整关闭}\;\\
\mathrm{C2}&\text{两条二进支路＋因子走廊＋偶 }v_2(K)\text{ 门，仍开放}\;\\
\mathrm{C1}&d\text{ 有限走廊＋奇 }W\text{ 区间＋CRT 走廊，仍开放}.
\end{array}}
\tag{15.1}
\]

因此

\[
\boxed{\mathrm{GCU\text{-}2}.}
\]

全文到此停止，不返回 A2，不研究 B、\(\gamma>1\)、非本原 C2/C5、
Q、O 或严格层。
