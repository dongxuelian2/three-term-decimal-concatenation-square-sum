# 三项十进制拼接平方和问题：临界 G 模板 A2 高 \(\varphi\) 主二进室负符号族报告

日期：2026-08-01（Asia/Tokyo）

本文严格限定于

\[
\boxed{
\mathcal F_{P-}:
\quad
G_{\mathrm{prim}},\quad
\gamma=1,\quad
\mathrm{A2},\quad
a\ge3,\quad
t=\varphi-a\ge0,\quad
t<\frac a2,\quad
\mathrm P_2,\quad
\sigma=-1.
}
\]

接受 `critical_G_A2_high_phi_single_lift_campaign.md` 的 GA2H-2 双向正规形、
`critical_G_A2_unit_determinant_campaign.md` 的 GA2-6 终端系统与大小门，
以及 PR6、SD6、GA1-1、GFP-1 和 v3 总账中与本分支相容的继承结论。
本文不研究 \(\mathcal F_{E-}\)、\(\varphi<a\)、B、C、\(\gamma>1\)、
C2/C5、Q 或严格层。

本轮严格完成了：

1. 非平凡公共根正规形及全部恢复公式；
2. 指数的三层穷尽和第三层精确上界；
3. \(B\)-进 involution 下降及每一步的非负性审计；
4. 全部下降余项的统一正性窗口 \(0<E_i<r\)；
5. 每个三层状态至多再作一次的溢出下降；
6. 最终商变量的唯一 CRT 走廊证书。

但是，现有结构不能把最后的、随 \(a\) 移动的 CRT 余数递推统一删除。
特别地，题设建议用于第三层的全局间隙

\[
0<\frac N{B^2}-E_2<r
\]

本身并非对全部允许状态成立；第 7.3 节给出一个通过全部局部门和精确大小门的
整数反例（它不是终端解）。因此本文不能诚实地分类为 GFPm-1 或 GFPm-2。
最终分类是

\[
\boxed{\mathrm{GFPm\text{-}3}.}
\]

这里的“残余”已经不含自由 \(q,s,L\) 搜索：对每个递推状态，最后的
\(L\) 被唯一标准余数决定；无界性只剩随 \(a\) 移动的有限递推。

---

## 1. 参数、尾窗与局部门

置

\[
M=4^a,\qquad
C=5^{2a-t},\qquad
B=MC=2Z,
\tag{1.1}
\]

\[
e=2a-t+h,\qquad
h\in\mathcal H(a),
\tag{1.2}
\]

其中

\[
\mathcal H(a)=
\left\{h\ge0:
2^{2a-2}\le5^{h+1},\quad
5^h<2^{2a-1}
\right\}.
\tag{1.3}
\]

和 GFP-1 中相同，\(a\ge3\) 时

\[
\boxed{1\le h\le a-1.}
\tag{1.4}
\]

本分支还需要下面一个以后保证二进整除的加强。

### 引理 1.1

\[
\boxed{h\ge t.}
\tag{1.5}
\]

**证明。** 若 \(h<t\)，因二者为整数，\(h+1\le t\)，于是

\[
2^{2a-2}\le5^{h+1}\le5^t<5^{a/2}.
\]

但对 \(a\ge3\)，

\[
5^{a/2}<2^{2a-2}
\]

等价于 \(5^a<2^{4a-4}\)；它在 \(a=3\) 时为 \(125<256\)，以后
右、左之比每步再乘 \(16/5>1\)。矛盾。\(\square\)

定义

\[
\boxed{
x=\left\langle2C^{-1}\right\rangle_M
\in\{0,\ldots,M-1\}.
}
\tag{1.6}
\]

对 \(J\in\{1,\ldots,9\}\)，置

\[
U=JM+x,
\tag{1.7}
\]

并保留全部局部门

\[
v_5\!\left(U+\frac M2\right)=3t,
\tag{1.8}
\]

\[
W=\frac{U+M/2}{5^{3t}},
\qquad
-2W\equiv1\text{ 或 }4\pmod5,
\tag{1.9}
\]

\[
v_2(k^2-1)=2a,
\qquad
\frac{k^2-1}{2^{2a}}\equiv3\text{ 或 }7\pmod8.
\tag{1.10}
\]

这里还保留 GA2H-2 的精确整数范围

\[
125^t<22\cdot2^{2a-1}.
\tag{1.11}
\]

---

## 2. 非平凡公共根正规形

### 2.1 \(x\ne0\) 与 Bezout 坐标

若 \(x=0\)，则 (1.6) 给 \(M\mid2\)，但 \(M\ge64\)，矛盾。因此

\[
\boxed{x\ne0.}
\tag{2.1}
\]

由 \(Cx\equiv2\pmod M\)，唯一存在整数 \(c\) 使

\[
\boxed{Cx=2+Mc.}
\tag{2.2}
\]

因 \(C>2\)、\(x>0\)，有 \(Cx>2\)，故 \(c>0\)。又因 \(x<M\)，

\[
Mc=Cx-2<CM=B,
\]

所以

\[
\boxed{1\le c<C.}
\tag{2.3}
\]

定义

\[
\boxed{\rho=Cx-1=1+Mc,}
\qquad
\boxed{\eta=cx.}
\tag{2.4}
\]

于是

\[
\begin{aligned}
\rho^2-1
&=(Cx-1)^2-1\\
&=Cx(Cx-2)\\
&=Cx\,Mc\\
&=MC\,cx=B\eta.
\end{aligned}
\]

故

\[
\boxed{\rho^2=1+B\eta.}
\tag{2.5}
\]

由 (2.3)，

\[
0<\rho=1+Mc\le1+M(C-1)<B,
\tag{2.6}
\]

并且

\[
0<\eta=cx<cM<1+cM=\rho.
\tag{2.7}
\]

### 2.2 \(r,q,N\) 的双向正规形

负符号主室中

\[
r=-1+CU.
\]

把 \(U=JM+x\) 和 \(Cx-1=\rho\) 代入，得到

\[
\boxed{r=\rho+BJ.}
\tag{2.8}
\]

终端方程为

\[
qr=1+BN.
\tag{2.9}
\]

模 \(B\) 使用 \(r\equiv\rho\) 得

\[
q\rho\equiv1\pmod B.
\]

再乘 \(\rho\)，并用 \(\rho^2\equiv1\pmod B\)，得到

\[
\boxed{q\equiv\rho\pmod B.}
\tag{2.10}
\]

因 \(q>0\) 且 \(0<\rho<B\)，唯一写成

\[
\boxed{q=\rho+BL,\qquad L\in\mathbb Z_{\ge0}.}
\tag{2.11}
\]

将 (2.8)、(2.11) 代入 (2.9)：

\[
\begin{aligned}
N
&=\frac{(\rho+BL)(\rho+BJ)-1}{B}\\
&=\frac{\rho^2-1}{B}+\rho(J+L)+BJL\\
&=\eta+\rho(J+L)+BJL.
\end{aligned}
\]

因此

\[
\boxed{N=\eta+\rho(J+L)+BJL.}
\tag{2.12}
\]

定义

\[
\boxed{E=\eta+\rho J.}
\tag{2.13}
\]

则

\[
\boxed{N=E+Lr,\qquad r\mid N-E.}
\tag{2.14}
\]

恢复公式是

\[
\boxed{
L=\frac{N-E}{r},\qquad
q=\rho+BL.
}
\tag{2.15}
\]

最后

\[
\boxed{s=N-Jq=\eta+\rho L.}
\tag{2.16}
\]

由 \(\eta>0\)、\(L\ge0\)，有 \(s>0\)。并且

\[
\begin{aligned}
q-s
&=(\rho+BL)-(\eta+\rho L)\\
&=(\rho-\eta)+L(B-\rho)>0
\end{aligned}
\]

因为 (2.6)–(2.7) 的两个括号都严格为正。因此

\[
\boxed{0<s<q.}
\tag{2.17}
\]

这里没有遗漏 \(L=0\)：此时

\[
q=\rho,\qquad s=\eta,
\]

而 (2.7) 正好给 \(0<s<q\)。所以 (2.8)–(2.17) 是完整双向正规形。

### 2.3 基础间隙

由 (2.7)、(2.6)，

\[
E=\eta+\rho J<(J+1)\rho<\rho+JB=r.
\]

故

\[
\boxed{0<E<r.}
\tag{2.18}
\]

这将作为全部下降层正性归纳的初值。

---

## 3. 指数上界与三层穷尽

令

\[
\nu=m-e\ge0.
\tag{3.1}
\]

由 \(e=2a-t+h\)，

\[
\boxed{N=2^{2a-t+h+\nu}5^\nu.}
\tag{3.2}
\]

### 3.1 纯整数大小比较

继承门为

\[
20\cdot10^m<194029Z^2Y,
\qquad
Z=2^{2a-1}5^{2a-t},
\qquad
Y=10^{3a}.
\tag{3.3}
\]

当 \(t=0\) 时，\(Z^2Y=10^{7a}/4\)。若 \(m\ge7a+4\)，则

\[
80\cdot10^m\ge800000\cdot10^{7a}
>194029\cdot10^{7a},
\]

与 (3.3) 矛盾。因此

\[
\boxed{t=0\Longrightarrow m\le7a+3.}
\tag{3.4}
\]

当 \(t\ge1\) 时，

\[
\frac{Z^2Y}{10^{7a}}=\frac1{4\cdot5^{2t}}\le\frac1{100}.
\]

若 \(m\ge7a+3\)，把 (3.3) 同除以 \(10^{7a}\) 并乘以 \(100\)，
会要求

\[
2000000<194029,
\]

不可能。因此

\[
\boxed{t\ge1\Longrightarrow m\le7a+2.}
\tag{3.5}
\]

没有使用浮点对数决定端点。

### 3.2 \(\nu<6a\) 与第三层上界

由 (3.4)–(3.5)，

\[
\nu\le
\begin{cases}
5a+3-h,&t=0,\\
5a+t+2-h,&t\ge1.
\end{cases}
\tag{3.6}
\]

当 \(t=0\) 时，(1.4) 给 \(\nu\le5a+2<6a\)。当 \(t\ge1\) 时，

\[
\nu\le5a+t+1<6a,
\]

因为 \(t<a/2\) 且 \(a>2\) 给 \(t+1<a\)。故

\[
\boxed{\nu<6a.}
\tag{3.7}
\]

对 \(\nu\) 关于 \(2a\) 作唯一欧几里得分解：

\[
\boxed{
\nu=2aj+v,
\qquad
j\in\{0,1,2\},
\qquad
0\le v<2a.
}
\tag{3.8}
\]

若 \(j=2\)，由 (3.6) 进一步得到

\[
\boxed{
0\le v\le
\begin{cases}
a+3-h,&t=0,\\
a+t+2-h,&t\ge1.
\end{cases}}
\tag{3.9}
\]

式 (3.8)–(3.9) 严格穷尽全部允许指数。

---

## 4. \(B\)-进 involution 下降

当 \(\nu=2aj+v\) 时，

\[
\boxed{
\frac N{B^j}
=2^{2a-t+h+v}5^{v+tj}.
}
\tag{4.1}
\]

定义

\[
E_0=E.
\tag{4.2}
\]

对每个 \(i<j\)，规范定义

\[
\boxed{
\lambda_i=\left\langle-E_i\rho\right\rangle_B
\in\{0,\ldots,B-1\},
}
\tag{4.3}
\]

\[
\boxed{
E_{i+1}=\frac{E_i+\lambda_i r}{B}.
}
\tag{4.4}
\]

### 4.1 整除性

模 \(B\) 有

\[
r\equiv\rho,
\qquad
\lambda_i\equiv-E_i\rho,
\qquad
\rho^2\equiv1.
\]

因此

\[
E_i+\lambda_i r
\equiv E_i-E_i\rho^2
\equiv0\pmod B.
\]

所以 (4.4) 始终为整数。

### 4.2 中间商的非负性

从

\[
N=E_0+L_0r,
\qquad L_0=L\ge0,
\]

开始。假设

\[
\frac N{B^i}=E_i+L_ir,
\qquad L_i\ge0,
\]

且 \(i<j\)。因 \(B\mid N/B^i\)，模 \(B\) 得

\[
L_i\rho\equiv-E_i\pmod B,
\]

故

\[
L_i\equiv-E_i\rho\equiv\lambda_i\pmod B.
\]

\(\lambda_i\) 是最小非负代表，而 \(L_i\ge0\)，所以唯一写成

\[
\boxed{L_i=\lambda_i+BL_{i+1},\qquad L_{i+1}\ge0.}
\tag{4.5}
\]

把 (4.4)–(4.5) 代入并除以 \(B\)，得到

\[
\frac N{B^{i+1}}=E_{i+1}+L_{i+1}r.
\]

归纳即得

\[
\boxed{
\frac N{B^j}=E_j+L_jr,
\qquad L_j\in\mathbb Z_{\ge0}.
}
\tag{4.6}
\]

反向地，从任意 \(L_j\ge0\) 依次定义

\[
L_i=\lambda_i+BL_{i+1}
\]

便保持所有 \(L_i\ge0\)，并逐层恢复 \(N=E_0+L_0r\)。所以 (4.6)
是严格双向等价，不是单向筛。

### 4.3 所有下降余项都严格落在 \((0,r)\)

由 (2.18)，\(0<E_0<r\)。若 \(0<E_i<r\)，则

\[
0<E_i+\lambda_ir
<r+(B-1)r=Br.
\]

除以 \(B\) 得

\[
\boxed{0<E_{i+1}<r.}
\tag{4.7}
\]

因此对本报告中出现的全部下降层，统一有

\[
\boxed{0<E_i<r.}
\tag{4.8}
\]

这严格证明了题设要求在第一、第二层尝试的余项窗口；它甚至对可能出现的
一次额外下降仍成立。

### 4.4 低阶闭式递推

由 (4.4)，

\[
BE_{i+1}\equiv E_i\pmod r.
\]

又因 \(\gcd(B,r)=1\)（由 \(r\equiv\rho\pmod B\)、
\(\rho^2\equiv1\pmod B\)），并且 \(0<E_{i+1}<r\)，所以

\[
\boxed{
E_{i+1}=\left\langle B^{-1}E_i\right\rangle_r^+,
\qquad
E_i=\left\langle B^{-i}E\right\rangle_r^+,
}
\tag{4.9}
\]

其中 \(\langle\cdot\rangle_r^+\) 表示 \(\{1,\ldots,r-1\}\) 中的正代表。
同时

\[
\boxed{
\lambda_i=\frac{BE_{i+1}-E_i}{r}.
}
\tag{4.10}
\]

这是 \((\lambda_i,E_i)\) 的低阶闭式递推。它是一条随 \(r(a,t,J)\)
移动的模旋转，而不是固定模数的周期。

---

## 5. 至多一次溢出下降与唯一 CRT 走廊

三层下降后记

\[
P_j=\frac N{B^j}
=2^{A_j}5^{F_j},
\tag{5.1}
\]

其中

\[
A_j=2a-t+h+v,
\qquad
F_j=v+tj,
\qquad
c_0=2a-t=v_5(B).
\tag{5.2}
\]

由 \(h\ge t\)，始终有 \(A_j\ge2a\)。因此

\[
B\mid P_j
\iff
F_j\ge c_0.
\tag{5.3}
\]

定义

\[
\epsilon_j=
\begin{cases}
1,&F_j\ge c_0,\\
0,&F_j<c_0,
\end{cases}
\qquad
d=j+\epsilon_j.
\tag{5.4}
\]

若 \(\epsilon_j=1\)，再按第 4 节作一次、且只作一次 \(B\)-下降。
置

\[
\widehat P=\frac N{B^d}
=2^{\widehat A}5^{\widehat F},
\qquad
\widehat E=E_d,
\qquad
\widehat L=L_d,
\tag{5.5}
\]

其中

\[
\widehat A=A_j-2a\epsilon_j,
\qquad
\widehat F=F_j-c_0\epsilon_j.
\tag{5.6}
\]

若 \(\epsilon_j=0\)，显然 \(0\le\widehat F<c_0\)。若
\(\epsilon_j=1\)，由 \(v\le2a-1\)、\(j\le2\) 得

\[
\widehat F
=v+t(j+1)-2a
\le t(j+1)-1
\le3t-1<c_0,
\]

最后一步来自 \(t<a/2\)。所以

\[
\boxed{0\le\widehat F<c_0,\qquad d\le3.}
\tag{5.7}
\]

这证明每个原三层状态最多只需一次溢出下降，不会产生新的无界下降深度。

### 定理 5.1：唯一 CRT 走廊

任何终端状态都必须满足

\[
\widehat P=\widehat E+\widehat Lr,
\qquad
0<\widehat E<r,
\qquad
\widehat L\ge0.
\tag{5.8}
\]

并且

\[
\boxed{0\le\widehat L<5^{\widehat F}.}
\tag{5.9}
\]

**证明。** 因 \(r=\rho+BJ>B\)，

\[
\widehat L<\frac{\widehat P}{r}<\frac{\widehat P}{B}
=2^{\widehat A-2a}5^{\widehat F-c_0}.
\]

由 \(h\le a-1\)、\(v<2a\)，无论 \(\epsilon_j=0\) 或 \(1\)，均有

\[
\widehat A-2a<3a.
\]

又因 \(c_0=2a-t>3a/2\)，而

\[
2^{3a}<5^{3a/2}
\]

等价于 \(64^a<125^a\)，所以

\[
2^{\widehat A-2a}<5^{c_0}.
\]

代回即得 (5.9)。\(\square\)

因为 \(\widehat F<c_0\)，有

\[
r\equiv-1\pmod{5^{\widehat F}}.
\]

把 (5.8) 模 \(5^{\widehat F}\) 化简，并使用 (5.9)，得到唯一值

\[
\boxed{
\widehat L
=\left\langle\widehat E\right\rangle_{5^{\widehat F}}
\in\{0,\ldots,5^{\widehat F}-1\}.
}
\tag{5.10}
\]

这里当 \(\widehat F=0\) 时模数为 \(1\)，按规范定义右端为 \(0\)；
这正是必须保留的 \(\widehat L=0\) 边界。

再令

\[
g_2=\min(\widehat A,2a).
\]

因为 \(r\equiv1\pmod{2^{g_2}}\) 且 \(2^{g_2}\mid\widehat P\)，还必须有

\[
\boxed{
\widehat L\equiv-\widehat E\pmod{2^{g_2}}.
}
\tag{5.11}
\]

因此每个状态不再需要枚举 \(L\)。定义

\[
\ell_*=\left\langle\widehat E\right\rangle_{5^{\widehat F}}.
\tag{5.12}
\]

该状态为终端状态，当且仅当

\[
\boxed{
\ell_*\equiv-\widehat E\pmod{2^{g_2}},
\qquad
\widehat P=\widehat E+\ell_*r.
}
\tag{5.13}
\]

若 (5.13) 成立，反向使用 (4.5) 唯一恢复全部 \(L_i\)，再由 (2.15)–(2.17)
恢复 \(q,s\)。所以 (5.13) 是双向的规范 CRT 走廊证书。

---

## 6. 三层的准确状态

### 6.1 第零层 \(j=0\)

本层为

\[
2^{2a-t+h+v}5^v=E+Lr,
\qquad0\le v<2a.
\tag{6.1}
\]

第 2.3 节已经证明

\[
\boxed{0<E<r.}
\]

若 \(v<2a-t\)，无需额外下降；若 \(v\ge2a-t\)（只可能在 \(t>0\)），
严格再下降一次。两种情形均由 (5.10)–(5.13) 唯一决定最后的商变量。

现有不等式不能把所有 \(a\) 上的 (5.13) 统一删除：
\(\widehat E\) 是模 \(r(a,t,J)\) 的移动逆幂余数，既没有固定模数周期，
也没有由现有尾窗推出的统一实数下界。故本层留下无界但每个 \(a\) 严格有限的
规范递推残余。

### 6.2 第一层 \(j=1\)

本层为

\[
2^{2a-t+h+v}5^{v+t}=E_1+L_1r,
\qquad0\le v<2a.
\tag{6.2}
\]

第 4.3 节给出题设要求的统一结论

\[
\boxed{0<E_1<r.}
\tag{6.3}
\]

若 \(v+t<2a-t\)，直接进入 CRT 走廊；若
\(v+t\ge2a-t\)，严格再下降一次。仍由 (5.13) 唯一判定。

所以第一层也不含自由 \(L_1\) 搜索，但 \(a\) 仍未绝对有界，移动余数递推
尚未被统一关闭。

### 6.3 第二层 \(j=2\)

本层为

\[
2^{2a-t+h+v}5^{v+2t}=E_2+L_2r,
\tag{6.4}
\]

其中 \(v\) 还满足 (3.9)，且

\[
\boxed{0<E_2<r.}
\tag{6.5}
\]

题设建议争取证明

\[
0<2^{2a-t+h+v}5^{v+2t}-E_2<r
\tag{6.6}
\]

来删除正整数 \(L_2\)。但 (6.6) 不能作为全体定理。下面给出一个完全精确、
并通过全部局部门和大小门的反例状态：

\[
(a,t,h,J,v)=(3,0,1,4,5).
\tag{6.7}
\]

此时

\[
M=64,quad C=15625,quad B=1000000,quad
x=50,quad c=12207,
\]

\[
\rho=781249,quad \eta=610350,quad
r=4781249,quad k=5281249.
\]

局部门逐项为

\[
v_5(U+M/2)=0=3t,qquad W=338\equiv3\pmod5,
\]

\[
\frac{k^2-1}{2^{2a}}\equiv7\pmod8,qquad
\frac{k^2-1}{5^{2(a+t)}}\equiv4\pmod5.
\]

又 \(\nu=4a+v=17\)、\(e=7\)、\(m=24\)，并且精确大小门为

\[
20\cdot10^{24}
<194029\cdot500000^2\cdot10^9.
\]

下降数据为

\[
E_0=3735346,quad \lambda_0=672846,
\]

\[
E_1=3217048,quad \lambda_1=467048,
\]

\[
E_2=2233076.
\]

而

\[
P_2=12800000,qquad
P_2-E_2=10566924>r.
\tag{6.8}
\]

所以 (6.6) 的统一版本为假。该状态仍不是终端状态，因为

\[
10566924=2r+1004426,
\]

并不被 \(r\) 整除。它的作用只是排除一条不合法的统一证明路线，不能被
误写成原题候选。

第二层的正确统一结论仍是 (5.13)：若 \(v+2t\ge2a-t\)，先作唯一一次
溢出下降；否则直接进入唯一 CRT 走廊。这里同样完整保留
\(\widehat L=0\) 的等式边界。

---

## 7. 辅助恒等式与对称因子式

### 7.1 三个基础模数

由定义直接有

\[
\boxed{r\equiv-1\pmod C,}
\qquad
\boxed{r\equiv1\pmod M,}
\qquad
\boxed{r\equiv\rho\pmod B.}
\tag{7.1}
\]

同时 (2.10) 给

\[
\boxed{q\equiv\rho\pmod B.}
\tag{7.2}
\]

所以 \(q,r\) 在全部层中始终保持同一个非平凡 involution 根类；下降没有
改变该根类。

还有两个有用的精确恒等式：

\[
\boxed{\rho r=1+BE,}
\tag{7.3}
\]

\[
\boxed{\rho E-J=\eta r.}
\tag{7.4}
\]

后者结合 (4.9) 给出

\[
\boxed{
(-1)^i\rho^{i+1}E_i\equiv J^{i+1}\pmod r.
}
\tag{7.5}
\]

这些同余是递推复核门，但现阶段不单独产生统一矛盾。

### 7.2 对称 \(q,r\) 方程

定义

\[
V=x+ML.
\tag{7.6}
\]

则

\[
\boxed{q=-1+CV,\qquad r=-1+CU.}
\tag{7.7}
\]

把 (7.7) 代入 \(qr=1+BN\)，展开并除以 \(C\)，得到

\[
\boxed{CUV-U-V=MN.}
\tag{7.8}
\]

反向展开 (7.8) 即恢复终端方程。因此 (7.8) 与终端因子系统双向等价。
它清楚展示两个因子都处于 \((-1\bmod C,\ 1\bmod M)\) 的同一 CRT 根类，
但没有把随 \(a\) 移动的 \(S\)-单位右端化为固定曲线。

---

## 8. 覆盖全部 \(a\) 的规范递推残余

本节明确说明 GFPm-3 中仍剩什么；它不是“对若干 \(a\) 做试验”。

令

\[
P_a=\left\langle5^{-2a}\right\rangle_{4^a}.
\tag{8.1}
\]

则

\[
\boxed{x_{a,t}=\left\langle2\cdot5^tP_a\right\rangle_{4^a}.}
\tag{8.2}
\]

继承 GA2H-2 的规范递推：若

\[
25^aP_a=1+Q_a4^a,
\]

取唯一 \(\delta_a\in\{0,1,2,3\}\) 使

\[
Q_a+\delta_a25^a\equiv0\pmod4,
\]

并置 \(\widehat P_a=P_a+\delta_a4^a\)，则

\[
\boxed{
P_{a+1}
=\left\langle25^{-1}\widehat P_a\right\rangle_{4^{a+1}},
\qquad P_3=57.
}
\tag{8.3}
\]

尾窗最大指标 \(H_a\) 和允许的最大 \(t\) 也分别由 GA2H-2 的
(6.10)–(6.12) 作一步整数递推。于是全部无界状态按下列有限程序生成：

1. 由 (8.3) 生成 \(P_a\)，由 (8.2) 生成全部允许 \(x_{a,t}\)；
2. 由 \(Cx=2+Mc\) 得 \(c\)，再得 \(\rho,\eta\)；
3. 对九个 \(J\) 检查 (1.8)–(1.10)；
4. 对至多两个 \(h\) 和三层 \((j,v)\) 使用 (3.8)–(3.9)；
5. 用 (4.9) 计算至多三个 \(E_i\)；
6. 用 (5.4) 判断是否作唯一一次溢出下降；
7. 最后只检查 (5.13) 的一个标准余数。

因此每个 \(a\) 的终端状态是严格有限的，且没有自由离散对数、自由 \(L\)
或自由提升深度。但是模数

\[
r(a,t,J)=\rho(a,t)+B(a,t)J
\]

仍随 \(a\) 移动，(4.9)–(5.13) 尚未化为固定有限状态自动机或由指数不等式
强迫的有限小端。这正是 GFPm-3，而不是 GFPm-2。

---

## 9. 主动审计

### 9.1 是否证明了 \(x\ne0\) 和 \(c>0\)

是。第 2.1 节分别使用 \(M\nmid2\) 及 \(C>2,x>0\)，并进一步证明
\(c<C\)、\(0<\eta<\rho<B\)。

### 9.2 是否遗漏 \(L=0\)

没有。原始 \(L=0\) 在第 2.2 节单独核对；下降后的
\(\widehat L=0\) 由 \(\widehat F=0\) 或标准余数为零完整保留。

### 9.3 是否未经证明假设中间 \(L_i\ge0\)

没有。第 4.2 节从最小非负代表的唯一性逐层证明
\(L_i=\lambda_i+BL_{i+1}\) 中 \(L_{i+1}\ge0\)，反向恢复也保持非负。

### 9.4 是否只检查有限多个 \(a\)

没有。第 1–5、7–8 节均为覆盖全部 \(a\ge3\) 的符号证明和显式递推。
第 6.3 节的单个数值状态只用于反驳错误的统一间隙 (6.6)，不承担任何
无界结论。

### 9.5 是否用浮点数决定 \(m,\nu,v\) 端点

没有。第 3 节只使用

\[
800000>194029,
\qquad
2000000>194029
\]

等整数比较。

### 9.6 是否把三层之外的新指数层遗漏

没有。\(\nu<6a\) 严格给出 \(j\in\{0,1,2\}\)。第 5 节出现的
\(d=3\) 不是新的 \(\nu\)-层，只是当 \(t>0\) 时
\(B=10^{2a}/5^t\) 较小而被强迫的唯一一次额外整除下降。

### 9.7 是否把局部状态当作终端候选

没有。第 6.3 节的状态通过局部门和大小门，但明确失败
\(r\mid P_2-E_2\)；它只证明某个拟议不等式为假。

### 9.8 是否发现 GA2H-2 或 GFP-1 的继承错误

没有。非平凡根正规形、三层缩放及局部门都与继承系统一致。发现的是本轮
拟议“第三层统一小间隙”不能成立，不是继承定理错误。

### 9.9 为什么不生成有限证书包

有限证书只允许承担由符号不等式严格强迫的小端。本文最后的 (5.13) 仍随
无界 \(a\) 移动；没有得到绝对有限边界。因此生成有限前缀证书并把它外推到
全部 \(a\) 会违反证明等级，本文没有这样做。

---

## 10. 最终分类与停止点

本文严格证明了题设要求的正规形

\[
\rho^2=1+B\eta,qquad
r=\rho+BJ,qquad
q=\rho+BL,
\]

\[
N=E+Lr,qquad
E=\eta+\rho J,qquad
s=\eta+\rho L,qquad
0<s<q,
\]

以及完整三层下降

\[
\frac N{B^j}=E_j+L_jr,qquad
j\in\{0,1,2\},qquad
0<E_j<r,quad L_j\ge0.
\]

每个状态至多再作一次溢出下降，之后终端条件双向压成唯一 CRT 走廊

\[
\ell_*=\left\langle\widehat E\right\rangle_{5^{\widehat F}},
\]

\[
\ell_*\equiv-\widehat E\pmod{2^{\min(\widehat A,2a)}},
\qquad
\widehat P=\widehat E+\ell_*r.
\]

这已经删除全部自由终端商，并把每个 \(a\) 压成有限、规范、可递推的整数边界。
但 \(r\) 与 \(E_i\) 的模旋转仍随 \(a\) 无界移动，现有论证没有把 (5.13)
统一证明为空，也没有把它强迫到绝对有限小端。

因此：

\[
\boxed{
\mathrm{GFPm\text{-}3}:
\quad
\mathcal F_{P-}\text{ 的三层 involution 下降和唯一 CRT 走廊成立，}
\text{但仍有随 }a\text{ 移动的无界递推残余。}
}
\]

没有找到合法原题解，也没有发现 GA2H-2 或 GFP-1 的继承错误。
本文到此停止，不研究 \(\mathcal F_{E-}\)、\(\varphi<a\)、B、C、
\(\gamma>1\)、C2/C5、Q 或严格层。
