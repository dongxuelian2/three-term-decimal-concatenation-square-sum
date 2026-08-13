# 三项十进制拼接平方和问题：临界 G 模板 A2 低 \(\varphi\) 深五进提升报告

日期：2026-08-06（Asia/Tokyo）

本文严格研究

\[
\boxed{
G_{\mathrm{prim}},\qquad
\gamma=1,\qquad
\mathrm{A2},\qquad
a\ge3,\qquad
1\le\varphi<a.
}
\]

接受 PR6、SD6、GA2-6、GE2-1 以及 v3 总账中与本分支相容的冻结结论。
高 \(\varphi\) 的 \(\mathcal F_{P-}\)、B、C、\(\gamma>1\)、非本原
C2/C5、Q 与严格层均不在本文范围内。

本轮得到完整的参数化深提升定理：

1. 全部终端候选恰分成正、负两个模 \(B=d^2\) 的公共平方根族；
2. 模 \(\Lambda=5^{3(a-\varphi)}\) 的自由提升是一个显式 Möbius
   involution；
3. 固定深提升状态后，自由的 \(q,s,L\) 被唯一压成一个非负仿射参数
   \(y\)；
4. 每个状态的全部 \(S\)-单位指数先形成一个完整指数同余类，再被判别式
   大小门截成有限同余段；
5. involution 可逐个五进数字 Hensel 提升：首层恰有两个合法数字，之后
   每层每个节点恰有五个子提升；
6. 两个符号各有唯一固定点，但固定点都被精确五进根门删除，故通过两项
   五进门的局部状态全部组成二循环。

这给出覆盖全部 \((a,\varphi)\) 与全部深度
\(3(a-\varphi)\) 的有限字母递推系统，因而最终分类为

\[
\boxed{\mathrm{GAL\text{-}2}.}
\]

这里的“有限递推族”是指有限个参数化递推模式和固定数字字母表，不是说
最终叶节点数一致有界。事实上，每个符号在深度 \(3\Delta\) 上仍恰有
\(2\cdot5^{3\Delta-1}\) 个通过五进判别式门的有向状态。因此本文没有
证明 \(\Delta\) 绝对有界，也没有关闭正根或负根族。

---

## 1. 低 \(\varphi\) 重参数化

定义

\[
\boxed{\Delta=a-\varphi\ge1.}
\tag{1.1}
\]

沿用 A2 尾窗坐标

\[
h=\varphi+e-3a,
\qquad
h\in\mathcal H(a),
\tag{1.2}
\]

其中

\[
\boxed{
\mathcal H(a)=
\left\{
h\ge0:
2^{2a-2}\le5^{h+1},\quad
5^h<2^{2a-1}
\right\}.
}
\tag{1.3}
\]

于是

\[
\boxed{e=3a+h-\varphi=2a+\Delta+h.}
\tag{1.4}
\]

置

\[
\boxed{
M=2^{2a},\qquad
C=5^{2\varphi},\qquad
\Lambda=5^{3\Delta},\qquad
B=MC.
}
\tag{1.5}
\]

由于 A2 中 \(d=2^a5^\varphi\)，有

\[
\boxed{B=2^{2a}5^{2\varphi}=d^2.}
\tag{1.6}
\]

又因 \(\varphi=a-\Delta\)，

\[
3a-\varphi=2a+\Delta=2\varphi+3\Delta.
\tag{1.7}
\]

继承公式

\[
Z=2^{2a-1}5^{3a-\varphi}
\]

严格化为

\[
\boxed{Z=\frac{B\Lambda}{2},\qquad 2Z=B\Lambda.}
\tag{1.8}
\]

因此终端方程与严格窗口分别成为

\[
\boxed{qr=1+B\Lambda N,}
\tag{1.9}
\]

\[
\boxed{
JB\Lambda<r<(J+1)B\Lambda,
\qquad J\in\{1,\ldots,9\}.
}
\tag{1.10}
\]

定义放大 \(S\)-单位

\[
\boxed{\widetilde N=\Lambda N.}
\tag{1.11}
\]

由 \(N=2^m5^{m-e}\) 与 (1.4) 得

\[
\begin{aligned}
\widetilde N
&=2^m5^{m-e+3\Delta}\\
&=\boxed{2^m5^{m-2\varphi-h}}.
\end{aligned}
\tag{1.12}
\]

若令

\[
\mu=m-e\ge0,
\]

则同一量也可写成

\[
\boxed{
\widetilde N=2^{e+\mu}5^{\mu+3\Delta}.
}
\tag{1.13}
\]

这些等式没有使用近似对数或有限参数前缀。

---

## 2. 模 \(B\) 的两个共同平方根

GE2-1 已证明

\[
v_2(k^2-1)=2a.
\tag{2.1}
\]

继承的 Jacobi 锁定给 \(k\equiv1\pmod8\)。因为

\[
v_2(k-1)+v_2(k+1)=2a,
\]

而 \(k\equiv1\pmod8\) 给 \(v_2(k+1)=1\)，故

\[
\boxed{v_2(k-1)=2a-1,}
\tag{2.2}
\]

从而

\[
\boxed{k\equiv1+\frac M2\pmod M.}
\tag{2.3}
\]

由 (1.8)，\(C\Lambda\) 为奇数，故

\[
Z=\frac M2(C\Lambda)\equiv\frac M2\pmod M.
\]

于是

\[
\boxed{r=k-Z\equiv1\pmod M.}
\tag{2.4}
\]

另一方面，GA2-6 已严格证明

\[
v_5(k^2-1)=2\varphi.
\tag{2.5}
\]

因为 \(5\nmid2\)，\(k-1\) 与 \(k+1\) 不可能同时被 5 整除，所以存在
唯一

\[
\boxed{\sigma\in\{+1,-1\}}
\]

使

\[
\boxed{v_5(k-\sigma)=2\varphi.}
\tag{2.6}
\]

由 \(C\Lambda\mid Z\)，

\[
\boxed{r\equiv k\equiv\sigma\pmod C.}
\tag{2.7}
\]

联合 (2.4)、(2.7)，\(r\) 位于模 \(B=MC\) 的唯一 CRT 根类

\[
\boxed{r\equiv\rho_\sigma\pmod B.}
\tag{2.8}
\]

### 2.1 正根

正根显然为

\[
\boxed{\rho_+=1,\qquad\eta_+=0.}
\tag{2.9}
\]

### 2.2 负根

定义

\[
x=\left\langle2C^{-1}\right\rangle_M,
\qquad
Cx=2+Mc.
\tag{2.10}
\]

因为 \(M\ge64\)，\(x=0\) 会迫使 \(M\mid2\)，故 \(x>0\)。又因
\(C\ge25\)，有 \(Cx>2\)，所以 \(c>0\)。由 \(x<M\) 还得

\[
Mc=Cx-2<CM=B,
\qquad 0<c<C.
\tag{2.11}
\]

置

\[
\boxed{\rho_-=Cx-1=1+Mc,\qquad\eta_-=cx.}
\tag{2.12}
\]

则

\[
0<\rho_-<CM=B,
\tag{2.13}
\]

并且

\[
\rho_-^2-1=Cx(Cx-2)=MC(cx)=B\eta_-.
\]

故两个符号统一满足

\[
\boxed{
0<\rho_\sigma<B,
\qquad
\rho_\sigma^2=1+B\eta_\sigma.
}
\tag{2.14}
\]

后文写 \(\rho=\rho_\sigma\)、\(\eta=\eta_\sigma\)。

由 (1.9)，\(qr\equiv1\pmod B\)。而 \(r\equiv\rho\pmod B\)、
\(\rho^2\equiv1\pmod B\)，故

\[
\boxed{q\equiv r\equiv\rho\pmod B.}
\tag{2.15}
\]

---

## 3. 深提升坐标与完整终端公式

由 \(0<\rho<B\)、\(q,r>0\) 及 (2.15)，唯一写成

\[
\boxed{
r=\rho+BV,\qquad
q=\rho+BL,
}
\tag{3.1}
\]

其中 \(V,L\in\mathbb Z_{\ge0}\)。

把 \(r=\rho+BV\) 代入严格窗口 (1.10)。由于端点均为 \(B\) 的倍数，
而 \(0<\rho<B\)，逐端取整恰得

\[
\boxed{J\Lambda\le V\le(J+1)\Lambda-1.}
\tag{3.2}
\]

定义

\[
\boxed{
\tau=V-J\Lambda,
\qquad0\le\tau<\Lambda.
}
\tag{3.3}
\]

于是

\[
\boxed{V=J\Lambda+\tau,}
\tag{3.4}
\]

\[
\boxed{r=\rho+B(J\Lambda+\tau).}
\tag{3.5}
\]

将 (3.1) 代入 (1.9)，并使用 \(\rho^2=1+B\eta\)：

\[
\begin{aligned}
qr
&=(\rho+BL)(\rho+BV)\\
&=1+B\{\eta+\rho(V+L)+BLV\}.
\end{aligned}
\]

与 \(qr=1+B\widetilde N\) 比较，严格得到

\[
\boxed{
\widetilde N=\eta+\rho(V+L)+BLV.
}
\tag{3.6}
\]

定义

\[
E_V=\eta+\rho V.
\tag{3.7}
\]

则

\[
\boxed{\widetilde N=E_V+Lr.}
\tag{3.8}
\]

反向地，任取满足 (3.2) 的 \(V\) 和任意 \(L\ge0\)，以 (3.1)、
(3.6) 定义 \(r,q,\widetilde N\)，便逐项恢复

\[
qr=1+B\widetilde N,
\qquad
JB\Lambda<r<(J+1)B\Lambda.
\]

所以 (3.6)–(3.8) 是完整双向终端公式，不只是必要同余。

---

## 4. 内层余数、Möbius involution 与仿射恢复

继承欧几里得关系为

\[
N=Jq+s.
\tag{4.1}
\]

把 \(V=J\Lambda+\tau\) 代入 (3.6)，并减去
\(J\Lambda q=J\Lambda(\rho+BL)\)，得到

\[
\boxed{
\Lambda s=\eta+\rho(\tau+L)+BL\tau.
}
\tag{4.2}
\]

定义

\[
\boxed{R_\tau=\rho+B\tau,}
\qquad
\boxed{A_\tau=\eta+\rho\tau.}
\tag{4.3}
\]

则

\[
\boxed{\Lambda s=A_\tau+LR_\tau.}
\tag{4.4}
\]

因为 \(\rho\equiv\pm1\pmod5\)、\(5\mid B\)，

\[
\boxed{\gcd(R_\tau,\Lambda)=1.}
\tag{4.5}
\]

所以整除条件唯一决定

\[
L\equiv-A_\tau R_\tau^{-1}\pmod\Lambda.
\tag{4.6}
\]

定义标准代表

\[
\boxed{
\lambda_\tau=
\left\langle-A_\tau R_\tau^{-1}\right\rangle_\Lambda
\in\{0,\ldots,\Lambda-1\}.
}
\tag{4.7}
\]

由于 \(L\ge0\) 且 \(0\le\lambda_\tau<\Lambda\)，有严格双向等价

\[
\boxed{
\Lambda\mid A_\tau+LR_\tau
\Longleftrightarrow
L=\lambda_\tau+\Lambda y,
\quad y\in\mathbb Z_{\ge0}.
}
\tag{4.8}
\]

这包括 \(\lambda_\tau=0,y=0\)。

### 4.1 involution

模 \(\Lambda\) 定义

\[
\boxed{
f(\tau)=
-\frac{\eta+\rho\tau}{\rho+B\tau}.
}
\tag{4.9}
\]

其矩阵为

\[
\mathcal M=
\begin{pmatrix}
-\rho&-\eta\\
B&\rho
\end{pmatrix}.
\tag{4.10}
\]

由 \(\rho^2-B\eta=1\) 逐项相乘：

\[
\boxed{\mathcal M^2=I.}
\tag{4.11}
\]

全部分母均为五进单位，所以矩阵恒等式确实在整个
\(\mathbb Z/\Lambda\mathbb Z\) 上定义了

\[
\boxed{f(f(\tau))=\tau\pmod\Lambda.}
\tag{4.12}
\]

而 (4.7) 正是

\[
\boxed{\lambda_\tau=f(\tau)}
\]

的标准代表。

### 4.2 固定点的完整分类

固定点方程为

\[
\boxed{
B\tau^2+2\rho\tau+\eta\equiv0\pmod\Lambda.
}
\tag{4.13}
\]

其导数

\[
2B\tau+2\rho\equiv2\rho\not\equiv0\pmod5
\]

处处为五进单位。因此每个符号在每个精度 \(5^n\) 上恰有一个固定点，
且该固定点逐层唯一提升。

正根中，(4.13) 因式分解为

\[
\tau(2+B\tau)\equiv0\pmod\Lambda.
\]

第二因子为五进单位，故

\[
\boxed{\tau_+^*=0.}
\tag{4.14}
\]

负根中可使用 \(Mc=Cx-2\) 得到整数恒等式

\[
\boxed{
B\tau^2+2\rho\tau+\eta
=(x+M\tau)(c+C\tau).
}
\tag{4.15}
\]

而 \(c\equiv-2M^{-1}\not\equiv0\pmod5\)，所以第二因子也是五进单位。
因此唯一固定点为

\[
\boxed{
\tau_-^*=\left\langle-xM^{-1}\right\rangle_\Lambda.
}
\tag{4.16}
\]

第 6 节将证明两个固定点都被精确根门删除。故全部通过两项五进门的局部
状态都是二循环，没有被错误删除的固定点。第 7 节的终端模 8 门未必保持
每个二循环；它作为独立奇偶筛附加，而不改变 involution 本身。

### 4.3 自由 \(q,s,L\) 的完全消除

定义

\[
\boxed{
s_0(\tau)=
\frac{A_\tau+\lambda_\tau R_\tau}{\Lambda}.
}
\tag{4.17}
\]

分子按 (4.7) 被 \(\Lambda\) 整除。又因
\(A_\tau,\lambda_\tau,R_\tau\ge0\)，有

\[
s_0(\tau)\in\mathbb Z_{\ge0}.
\]

等号要求同时 \(A_\tau=0\) 与 \(\lambda_\tau=0\)。负根中
\(\eta>0\)，故不可能；正根中恰为 \(\tau=0\)。所以

\[
\boxed{
s_0=0
\Longleftrightarrow
(\sigma,\tau)=(+,0).
}
\tag{4.18}
\]

该状态将在第 6 节删除。因此全部真实局部状态自动满足 \(s_0>0\)。

再定义

\[
\boxed{q_0=\rho+B\lambda_\tau,}
\tag{4.19}
\]

\[
\boxed{N_0=Jq_0+s_0.}
\tag{4.20}
\]

将 \(L=\lambda_\tau+\Lambda y\) 代回，得到

\[
\boxed{q=q_0+B\Lambda y,}
\tag{4.21}
\]

\[
\boxed{s=s_0+R_\tau y,}
\tag{4.22}
\]

\[
\boxed{N=N_0+ry.}
\tag{4.23}
\]

其中 (4.23) 可由

\[
J(B\Lambda)y+R_\tau y
=\{B(J\Lambda+\tau)+\rho\}y=ry
\]

直接核对。因此

\[
\boxed{N=Jq+s}
\tag{4.24}
\]

恒成立。

在 \(y=0\) 时，(4.17)–(4.20) 与 (3.6) 给

\[
\boxed{q_0r=1+B\Lambda N_0.}
\tag{4.25}
\]

再给 \(q\) 增加 \(B\Lambda y\)，两边同时增加
\(B\Lambda ry\)，故

\[
\boxed{qr=1+B\Lambda N}
\tag{4.26}
\]

与 (4.17)–(4.23) 双向等价。

特别地，(4.25) 模 \(r\) 给

\[
B\Lambda N_0\equiv-1\pmod r.
\]

因 \(\gcd(B\Lambda,r)=1\)，得到比“先检查、不互素则删除”更强的结论：

\[
\boxed{\gcd(N_0,r)=1}
\tag{4.27}
\]

对每个局部状态自动成立，不存在这一类删除状态。

真实状态中 \(s=s_0+R_\tau y>0\)。继承终端窗口定理于是自动给

\[
\boxed{0<s<q,}
\tag{4.28}
\]

无需把 \(s<q\) 重新列作假设。

因此对固定

\[
(a,\varphi,h,J,\sigma,\tau)
\]

自由的 \(q,s,L\) 全部被唯一压成一个 \(y\in\mathbb Z_{\ge0}\)。

---

## 5. 端点 \(\lambda_\tau=0\)、\(L=0\) 与 \(y=0\)

由 involution，

\[
\lambda_\tau=0
\Longleftrightarrow
\tau=f(0).
\tag{5.1}
\]

正根中 \(f(0)=0\)，而 \(\tau=0\) 将被精确根门删除，所以真实正根状态
总有

\[
\boxed{\lambda_\tau>0.}
\tag{5.2}
\]

负根中

\[
f(0)=\left\langle-\eta\rho^{-1}\right\rangle_\Lambda
\tag{5.3}
\]

可能通过也可能不通过首位门；不能统一删除。当它通过时，\(f(0)\) 与
\(0\) 构成合法二循环，其中一端满足 \(\lambda_\tau=0\)。

由 (4.8)，

\[
L=0
\Longleftrightarrow
\lambda_\tau=0,quad y=0.
\tag{5.4}
\]

所以 \(L=0\) 只可能出现在上述负根特殊状态，且必须保留。此时

\[
q=\rho,qquad s=s_0>0,qquad N=N_0.
\]

一般的 \(y=0\) 也不能删除；它对应指数方程中
\(2^e10^\mu=N_0\)。同样，\(m=e\) 即 \(\mu=0\) 是合法端点，
只能由完整指数条件决定是否存在。

---

## 6. 精确五进根类与判别式剩余

### 6.1 正根

此时 \(\rho=1\)、\(\eta=0\)。由 (3.5) 与 \(Z=B\Lambda/2\)，

\[
\boxed{
k-1=B\left(J\Lambda+\tau+\frac\Lambda2\right).
}
\tag{6.1}
\]

括号虽以半整数记号书写，但原式中的 \(B\Lambda/2\) 是整数。取五进赋值
时，\(J\Lambda\) 与 \(\Lambda/2\) 都被 5 整除，故

\[
\boxed{
v_5(k-1)=2\varphi
\Longleftrightarrow
5\nmid\tau.
}
\tag{6.2}
\]

特别地 \(\tau=0\) 删除，正根唯一固定点随之删除。

又因 \(k+1\equiv2\pmod5\)，

\[
\boxed{
\frac{k^2-1}{5^{2\varphi}}
\equiv2M\tau\pmod5.
}
\tag{6.3}
\]

所以判别式剩余门严格等价于

\[
\boxed{2M\tau\equiv1\text{ 或 }4\pmod5.}
\tag{6.4}
\]

由于 \(M=2^{2a}\equiv(-1)^a\pmod5\)，无论 \(a\) 奇偶，(6.4)
都恰留下

\[
\boxed{\tau\equiv2\text{ 或 }3\pmod5.}
\tag{6.5}
\]

因此 (6.2) 在保留状态中自动满足。

### 6.2 负根

此时 \(\rho=Cx-1\)。同样计算得

\[
\boxed{
k+1=C\left[x+M\left(J\Lambda+\tau+\frac\Lambda2\right)\right].
}
\tag{6.6}
\]

于是

\[
\boxed{
v_5(k+1)=2\varphi
\Longleftrightarrow
5\nmid(x+M\tau).
}
\tag{6.7}
\]

又因 \(k-1\equiv-2\pmod5\)，

\[
\boxed{
\frac{k^2-1}{5^{2\varphi}}
\equiv-2(x+M\tau)\pmod5.
}
\tag{6.8}
\]

故判别式剩余门为

\[
\boxed{-2(x+M\tau)\equiv1\text{ 或 }4\pmod5.}
\tag{6.9}
\]

等价地，首位数字满足

\[
\boxed{x+M\tau\equiv2\text{ 或 }3\pmod5.}
\tag{6.10}
\]

即

\[
\tau\equiv M^{-1}(2-x)
\quad\text{或}\quad
M^{-1}(3-x)pmod5.
\tag{6.11}
\]

负根固定点满足 \(x+M\tau_-^*\equiv0\pmod\Lambda\)，所以也恰被
(6.7)–(6.10) 删除。

### 6.3 involution 保持精确五进根门

正根的定义同余直接给

\[
\boxed{
\lambda_\tau(1+B\tau)\equiv-\tau\pmod\Lambda.
}
\tag{6.12}
\]

因为括号为五进单位，

\[
v_5(\lambda_\tau)=v_5(\tau).
\tag{6.13}
\]

模 5 更有 \(\lambda_\tau\equiv-\tau\)，所以 (6.4) 的两个剩余
\(1,4\) 被互换，门整体保持。

负根中有更强的同余恒等式：

\[
\boxed{
(x+M\lambda_\tau)(\rho+B\tau)
\equiv x+M\tau\pmod\Lambda.
}
\tag{6.14}
\]

其证明是把 \(\lambda_\tau R_\tau\equiv-A_\tau\) 乘以 \(M\)，
再用

\[
x\rho-M\eta=x,
\qquad
xB-M\rho=M.
\]

由于 \(R_\tau\) 为五进单位，(6.7) 被保持；又因
\(R_\tau\equiv\rho\equiv-1\pmod5\)，

\[
x+M\lambda_\tau\equiv-(x+M\tau)\pmod5.
\tag{6.15}
\]

所以 (6.9) 的 \(1,4\) 同样互换。由此，involution 不会把一个精确
正根或负根状态送出其符号族。

---

## 7. 二进尺度与剩余模 8 门

由 \(r\equiv1\pmod M\) 及 \(Z\equiv M/2\pmod M\)，

\[
\boxed{k=r+Z\equiv1+\frac M2\pmod M.}
\tag{7.1}
\]

因此 \(v_2(k-1)=2a-1\)、\(v_2(k+1)=1\)，自动得到

\[
\boxed{v_2(k^2-1)=2a.}
\tag{7.2}
\]

这与 GE2-1 完全相容，并证明低 \(\varphi\) 深提升不再产生新的二进分室。

完整候选还须保留 GA2-6 的主室剩余门

\[
\frac{k^2-1}{M}\equiv3\text{ 或 }7\pmod8.
\tag{7.3}
\]

令

\[
c_\sigma=
\begin{cases}
0,&\sigma=+,\\
c,&\sigma=-.
\end{cases}
\]

由 \(\rho=1+Mc_\sigma\) 得

\[
k=1+\frac M2W,
\]

其中

\[
W=2c_\sigma+2C(J\Lambda+\tau)+C\Lambda
\tag{7.4}
\]

为奇数。因 \(a\ge3\)，\(M/4\equiv0\pmod8\)，故

\[
\frac{k^2-1}{M}\equiv W\pmod8.
\tag{7.5}
\]

又因 \(C\equiv1\pmod8\)、\(\Lambda\equiv1\pmod4\)，(7.3)
等价于一个简单终端奇偶门

\[
\boxed{c_\sigma+J+\tau\equiv1\pmod2.}
\tag{7.6}
\]

该门不产生新二进根类，只在 Hensel 叶节点上保留一个奇偶状态。逐层提升
\(\tau_{n+1}=\tau_n+u5^n\) 时，由于 \(5^n\) 为奇数，奇偶状态按

\[
\tau_{n+1}\equiv\tau_n+u\pmod2
\tag{7.7}
\]

更新。因此它也只需要固定二字母状态，不破坏第 9 节的有限字母递推。

---

## 8. 正根族的进一步结构

正根中

\[
\boxed{
\lambda_\tau=
\left\langle-\tau(1+B\tau)^{-1}\right\rangle_\Lambda,
}
\tag{8.1}
\]

\[
\boxed{
s_0=\frac{\tau+\lambda_\tau+B\tau\lambda_\tau}{\Lambda}.
}
\tag{8.2}
\]

由 (6.5)，\(\tau\) 是五进单位；由 (6.12)，\(\lambda_\tau\) 也是
五进单位。所以 \(\lambda_\tau\ne0\)，证明了题设的第一个优先目标。

再由 (6.12)，

\[
\tau+\lambda_\tau
\equiv B\tau^2(1+B\tau)^{-1}\pmod\Lambda.
\tag{8.3}
\]

右端在未达到模数深度时有精确五进阶 \(2\varphi\)。若
\(2\varphi\ge3\Delta\)，则 \(\tau+\lambda_\tau\) 被 \(\Lambda\)
整除；而两项都位于 \(\{1,\ldots,\Lambda-1\}\)，故其和只能等于
\(\Lambda\)。因此统一得到

\[
\boxed{
v_5(\tau+\lambda_\tau)=\min(2\varphi,3\Delta).
}
\tag{8.4}
\]

此外，因 \(B\) 为偶数、\(\Lambda\) 为奇数，(8.2) 给

\[
\boxed{s_0\equiv\tau+\lambda_\tau\pmod2.}
\tag{8.5}
\]

但 (8.4)–(8.5) 没有给 \(s_0\) 的统一奇偶值，也没有与
\(N_0=J(1+B\lambda_\tau)+s_0\) 产生矛盾。

Jacobi 路线在此同样保持相容：\(q,r\equiv1\pmod M\) 已给
\(q,r\equiv1\pmod8\)，而五进判别式门只交换 \(2,3\) 两个首位数字。
外部奇素数或离散对数门仍随 \(r\) 移动。判别式大小门只截断每个固定状态
的指数，不给 \(a\) 或 \(\Delta\) 的绝对界。因此本轮不能严格关闭正根族。

---

## 9. 逐五进数字的 Hensel 递推

定义对称多项式

\[
\boxed{
G(T,L)=\eta+\rho(T+L)+BTL.
}
\tag{9.1}
\]

模 \(5^n\) 的 involution 图恰为

\[
G(\tau_n,\lambda_n)\equiv0\pmod{5^n}.
\tag{9.2}
\]

取标准代表

\[
0\le\tau_n,\lambda_n<5^n
\]

并定义精确进位

\[
\boxed{
H_n=\frac{G(\tau_n,\lambda_n)}{5^n}\in\mathbb Z.
}
\tag{9.3}
\]

从精度 \(n\) 提升到 \(n+1\)，写

\[
\tau_{n+1}=\tau_n+u5^n,
\qquad
\lambda_{n+1}=\lambda_n+v5^n,
\tag{9.4}
\]

其中

\[
u,v\in\{0,1,2,3,4\}.
\]

逐项展开：

\[
\begin{aligned}
G(\tau_{n+1},\lambda_{n+1})/5^n
={}&H_n+u(\rho+B\lambda_n)+v(\rho+B\tau_n)\\
&+Buv5^n.
\end{aligned}
\tag{9.5}
\]

由于 \(5\mid B\)，模 5 后只有

\[
H_n+\rho(u+v)\equiv0\pmod5.
\]

所以对每个自由输入数字 \(u\)，输出数字被唯一强迫为

\[
\boxed{
v\equiv-u-\rho^{-1}H_n\pmod5,
\qquad0\le v\le4.
}
\tag{9.6}
\]

新的精确进位为

\[
\boxed{
H_{n+1}=
\frac{
H_n+u(\rho+B\lambda_n)+v(\rho+B\tau_n)+Buv5^n
}{5}.
}
\tag{9.7}
\]

式 (9.4)、(9.6)、(9.7) 是完整双向 Hensel 递推：

- 每个 \(u\) 恰有一个 \(v\)；
- 每个模 \(5^{n+1}\) 的图点约到模 \(5^n\) 后必回到唯一父点；
- 因而每个父点恰有五个子提升，没有遗漏或重复。

递推从精度零的

\[
\tau_0=\lambda_0=0,
\qquad H_0=\eta
\tag{9.8}
\]

开始。第一步只允许第 6 节给出的两个 \(u\) 数字；以后每一步允许全部
五个 \(u\) 数字。

### 9.1 固定点与二循环的提升

若精度 \(n\) 的节点固定，即 \(\tau_n=\lambda_n\)，则固定子节点还要求
\(u=v\)。由 (9.6)，这对 \(u\) 给出唯一线性方程，所以五个子节点中
恰有一个固定，另外四个组成两个二循环。

若父节点属于非平凡二循环，交换
\((\tau_n,\lambda_n)\) 后，(9.5)–(9.7) 也交换 \((u,v)\)。每个二循环
因此恰提升成五个二循环。

精度 1 时，正根的两个数字 \(2,3\) 被 \(f\) 交换；负根的两个
\(x+M\tau\) 数字 \(2,3\) 也被 (6.15) 交换。所以每个符号在精度 1
上恰有一个合法二循环。归纳得到：

\[
\boxed{
\begin{array}{c|c|c}
\text{精度 }n\ge1&\text{五进合法有向状态数}&\text{二循环数}\\ \hline
\sigma=+&2\cdot5^{n-1}&5^{n-1}\\
\sigma=-&2\cdot5^{n-1}&5^{n-1}
\end{array}
}
\tag{9.9}
\]

取 \(n=3\Delta\)，每个符号恰有

\[
\boxed{2\cdot5^{3\Delta-1}}
\]

个通过五进判别式门的深提升状态。

### 9.2 能力边界

递推字母表固定为

\[
\boxed{u\in\{0,1,2,3,4\},}
\]

\(v\) 由 (9.6) 唯一决定；再附加第 7 节的二状态奇偶更新即可恢复全部
主室剩余门。因此正、负根分别构成一个参数化递推走廊，而不是
\(5^{3\Delta}\) 次无结构搜索。

但精确进位 \(H_n\) 与外部参数 \((a,\varphi)\) 仍移动；本文没有把它们
压成固定有限状态自动机。更重要的是，(9.9) 表明局部五进门本身没有大规模
删除：每增加一位，状态数仍乘 5。因此它不能推出 \(\Delta\) 绝对有界。

---

## 10. 每个深提升状态的完整指数级数

真实 \(N\) 必须满足

\[
\boxed{N=N_0+ry=2^m5^{m-e}.}
\tag{10.1}
\]

令 \(\mu=m-e\ge0\)，则

\[
\boxed{2^e10^\mu=N_0+ry.}
\tag{10.2}
\]

第 4.3 节已经证明 \(\gcd(N_0,r)=1\)。又因
\(r\equiv1\pmod M\) 且 \(r\equiv\pm1\pmod5\)，

\[
\gcd(r,10)=1.
\]

所以 (10.2) 模 \(r\) 严格等价于

\[
\boxed{
10^\mu\equiv2^{-e}N_0\pmod r.
}
\tag{10.3}
\]

令

\[
M_r=\operatorname{ord}_r(10).
\tag{10.4}
\]

若右端不属于 \(\langle10\rangle\subset(\mathbb Z/r\mathbb Z)^\times\)，
该状态整体删除。若属于，则存在唯一

\[
\mu_0\in\{0,\ldots,M_r-1\}
\]

使全部整数解恰为

\[
\boxed{\mu\equiv\mu_0\pmod{M_r}.}
\tag{10.5}
\]

对每个这样的指数，唯一恢复

\[
\boxed{
y=\frac{2^e10^\mu-N_0}{r}.
}
\tag{10.6}
\]

为准确处理 \(y\ge0\)，定义 \(\mu_*\) 为同余类 (10.5) 中满足

\[
\mu\ge0,
\qquad
2^e10^\mu\ge N_0
\tag{10.7}
\]

的最小整数。左端随 \(\mu\) 严格增长，所以 \(\mu_*\) 存在且唯一。
于是全部非负仿射解恰为

\[
\boxed{
\mu=\mu_*+tM_r,
\qquad t\in\mathbb Z_{\ge0},
}
\tag{10.8}
\]

并由 (10.6) 唯一恢复 \(y\)。这证明 \(y\in\mathbb Z_{\ge0}\) 与原仿射
恢复双向等价，而不是只检查若干指数样本。

### 10.1 完全整数化的大小截断

继承必要门为

\[
20\cdot10^m<194029Z^2Y,
\qquad Y=10^{3a}.
\tag{10.9}
\]

置

\[
\mathscr T=194029Z^2,10^{3a},
\qquad
Q=\left\lfloor\frac{\mathscr T-1}{20}\right\rfloor.
\tag{10.10}
\]

严格不等式 (10.9) 等价于

\[
10^m\le Q.
\]

定义十进制整数位数函数

\[
\lfloor\log_{10}Q\rfloor
=\max\{j\in\mathbb Z_{\ge0}:10^j\le Q\}.
\]

则最大指数可完全整数化为

\[
\boxed{
m_{\max}=\lfloor\log_{10}Q\rfloor.
}
\tag{10.11}
\]

它满足相邻阈值复核

\[
\boxed{
20\cdot10^{m_{\max}}<\mathscr T
\le20\cdot10^{m_{\max}+1}.
}
\tag{10.12}
\]

因此每个固定深提升状态的全部真实指数恰为

\[
\boxed{
m=e+\mu_*+tM_r,
\quad
0\le t\le
\left\lfloor
\frac{m_{\max}-e-\mu_*}{M_r}
\right\rfloor.
}
\tag{10.13}
\]

若 \(m_{\max}<e+\mu_*\)，该状态为空。式 (10.13) 是完整有限同余段；
先有无界同余类 (10.5)，再由严格大小门截断，没有对无界指数作有限采样。

---

## 11. 覆盖全部 \((a,\varphi)\) 的外层递推

低 \(\varphi\) 的外层参数恰为

\[
a\ge3,
\qquad
1\le\Delta\le a-1,
\qquad
\varphi=a-\Delta.
\tag{11.1}
\]

尾窗本身可沿 \(a\) 递推。令

\[
H_a=\max\{h:5^h<2^{2a-1}\}.
\tag{11.2}
\]

则 \(H_3=2\)，并且因为右端每步乘 4 而 \(4<5\)，

\[
\boxed{
H_{a+1}=
\begin{cases}
H_a+1,&5^{H_a+1}<2^{2a+1},\\
H_a,&\text{否则}.
\end{cases}
}
\tag{11.3}
\]

随后

\[
\boxed{
\mathcal H(a)=
\{H_a\}\cup
\{H_a-1:5^{H_a}\ge2^{2a-2}\}.
}
\tag{11.4}
\]

给定 \((a,\Delta)\)，正根系数立即显式；负根的 \(x\) 是唯一解

\[
Cx\equiv2\pmod{2^{2a}},
\qquad0\le x<2^{2a},
\tag{11.5}
\]

可由扩展 Euclid 或标准奇数逆元 Hensel–Newton 提升唯一生成，不含搜索
分支。随后第 9 节从两个首位数字和固定五字母表生成全部
\((\tau,\lambda_\tau)\)，第 7 节附加奇偶状态，第 4 节恢复唯一仿射族，
第 10 节恢复完整有限指数段。

所以全部低 \(\varphi\) 终端状态被下列有限个参数化递推模式覆盖：

\[
\boxed{
\begin{array}{c|c|c|c}
\text{符号}&\text{首位条件}&\text{后继字母}&\text{终端附加门}\\ \hline
+&\tau_1\in\{2,3\}&u\in\{0,1,2,3,4\}&J+\tau+c_+=1\pmod2\\
-&x+M\tau_1\in\{2,3\}&u\in\{0,1,2,3,4\}&J+\tau+c_-=1\pmod2
\end{array}
}
\tag{11.6}
\]

其中每一步的 \(v,H_{n+1}\) 由 (9.6)–(9.7) 唯一决定。

这正是 GAL-2 所要求的“覆盖全部 \(\Delta\) 的显式 Hensel 递推族”。
它不是固定叶节点表，也不声称 \(a\) 或 \(\Delta\) 有界。

---

## 12. 完整生成顺序与充分性边界

全部低 \(\varphi\) 终端候选必须、且在终端层面只须按下列顺序生成。

1. 取 \(a\ge3\)、\(1\le\Delta\le a-1\)，置
   \(\varphi=a-\Delta\)。
2. 由 (11.3)–(11.4) 取 \(h\in\mathcal H(a)\)，置
   \(e=2a+\Delta+h\)。
3. 取 \(J\in\{1,\ldots,9\}\) 与 \(\sigma\in\{+,-\}\)，构造
   \(M,C,\Lambda,B,\rho,\eta\)。
4. 由第 9 节 Hensel 递推生成精度 \(3\Delta\) 的
   \((\tau,\lambda_\tau)\)，首层施加第 6 节门，终层施加 (7.6)。
5. 用 (3.5)、(4.17)–(4.20) 构造 \(r,q_0,s_0,N_0\)。
6. 解 (10.3)。若无离散对数则删除；若有，则用 (10.13) 生成完整有限
   指数段，并以 (10.6)、(4.21)–(4.23) 恢复 \(y,q,s,N\)。
7. 最后进入继承的 \(a_1,a_2\) 有限窗口、判别式平方、两个恢复符号、
   精确 gcd 尺度、\(a_3\) 窗口、三个逐项既约条件及原题直接回代。

第 1–6 步在终端层严格双向；第 7 步仍是原题完整候选不可省略的恢复门。
本文没有把终端状态误报为合法六元组。

---

## 13. 主动审计

### 13.1 \(\rho_+=1\) 的端点

它是模 \(B\) 的标准正根，满足 \(0<1<B\)。写
\(q=1+BL\)、\(r=1+BV\) 时，正整数同余类不会产生负商。

### 13.2 \(\rho_-\) 的标准区间

第 2.2 节证明 \(x>0\)、\(0<c<C\)，从而
\(0<\rho_-=1+Mc<B\)。没有把非标准 CRT 代表带入窗口取整。

### 13.3 \(\tau=0\)

正根中它违反 \(v_5(k-1)=2\varphi\)；负根中不能自动删除，必须按
(6.9) 检查。若负根 \(\tau=0\) 通过，它与 \(f(0)\) 构成二循环。

### 13.4 \(\lambda_\tau=0\)

正根真实状态不可能发生；负根可能发生，且只发生在
\(\tau=f(0)\)。本文完整保留。

### 13.5 \(s_0=0\)

恰为正根 \(\tau=0\)，已由精确根门删除。其余状态均有 \(s_0>0\)。

### 13.6 \(y=0\)、\(L=0\)

二者均未先验删除。\(L=0\) 只可能是负根的
\(\lambda_\tau=0,y=0\) 状态；\(y=0\) 一般由完整指数等式决定。

### 13.7 \(\gcd(N_0,r)\)

不是一个需要枚举检查的开放门；(4.25) 自动给
\(B\Lambda N_0\equiv-1\pmod r\)，故始终为 1。

### 13.8 involution 分母

\(R_\tau\equiv\rho\equiv\pm1\pmod5\)，所以在每个精度上都是单位。
不存在分母为零的例外。

### 13.9 固定点

每个符号恰有一个，分别由 (4.14)、(4.16) 给出；两者是被精确根门证明
删除，不是因“involution 默认无固定点”而遗漏。

### 13.10 正负根判别式符号

正根使用 \(k+1\equiv2\)，得到 \(+2M\tau\)；负根使用
\(k-1\equiv-2\)，得到 \(-2(x+M\tau)\)。符号没有互换。

### 13.11 \(m=e\)

对应 \(\mu=0\)，完整包含在 (10.5)–(10.13) 中。

### 13.12 大小门端点

使用 \((\mathscr T-1)/20\) 的整数下取整处理严格不等式；
(10.12) 同时核对接受端与相邻拒绝端。

### 13.13 每个 \(\tau\) 有限与全体有限

每个固定 \(\tau\) 的指数段有限，但 (9.9) 随 \(\Delta\) 指数增长。
本文没有把前者误报为全体状态有限。

### 13.14 有限 \(\Delta\) 前缀

机器证书只承担公式、端点与实现回归；GAL-2 的无界完备性来自第 9、11 节
符号递推，不来自证书前缀。

### 13.15 是否发现继承错误或原题解

没有发现 GE2-1、GA2-6、PR6 或 SD6 的错误，也没有找到合法原题六元组。

---

## 14. 独立生成器、验证器与规范证书

随报告生成：

- `critical_G_A2_low_phi_deep_lift_generator.py`：按第 9 节递推生成有限
  回归前缀，并独立以闭式 Möbius 图比较；
- `critical_G_A2_low_phi_deep_lift_verifier.py`：不导入生成器，独立重建
  根、Hensel 进位、二循环、仿射恒等式、模 8 奇偶门与大小阈值；
- `critical_G_A2_low_phi_deep_lift_certificate.json`：规范有界回归证书；
- `critical_G_A2_low_phi_deep_lift_SHA256SUMS.txt`：交付文件哈希。

规范证书默认覆盖

\[
3\le a\le4,
\qquad
1\le\Delta\le2,
\qquad
\sigma\in\{+,-\},
\]

共八个参数—符号摘要。它记录每层状态数、二循环数、唯一固定点、
\(\lambda=0\) 计数、状态与仿射恢复的规范 SHA-256、尾窗及严格
\(m_{\max}\) 阈值。

验证器的破坏测试包括：

1. 删除一个状态；
2. 篡改最高五进数字；
3. 用错误 involution 代替 \(f\)；
4. 交换正负根符号；
5. 把严格大小门移动到相邻指数。

这些破坏均必须被拒绝。证书不承担 \(a\ge5\) 或 \(\Delta\ge3\) 的证明；
其作用是独立复核符号递推的实现。

---

## 15. 最终分类与停止点

本轮严格建立：

\[
\boxed{
\begin{gathered}
B=d^2,\qquad Z=B\Lambda/2,\qquad
qr=1+B\Lambda N;\\
q\equiv r\equiv\rho_\sigma\pmod B,\qquad
\rho_\sigma^2=1+B\eta_\sigma;\\
r=\rho+B(J\Lambda+\tau),\qquad
q=\rho+BL;\\
\widetilde N=\eta+\rho(V+L)+BLV;\\
\Lambda s=A_\tau+LR_\tau;\\
L=\lambda_\tau+\Lambda y,\qquad
\lambda_\tau=f(\tau),\qquad f^2=1;\\
q=q_0+B\Lambda y,\qquad
s=s_0+R_\tau y,\qquad
N=N_0+ry;\\
\gcd(N_0,r)=1;\\
10^\mu\equiv2^{-e}N_0\pmod r,\qquad
\mu\equiv\mu_0\pmod{\operatorname{ord}_r(10)};\\
\tau_{n+1}=\tau_n+u5^n,\qquad
\lambda_{n+1}=\lambda_n+v5^n,\\
v\equiv-u-\rho^{-1}H_n\pmod5.
\end{gathered}
}
\tag{15.1}
\]

正、负根各有一个首层二循环；每个二循环逐层产生五个二循环。两符号的
固定点都由精确五进根门删除。通过两项五进门的状态形成完整二循环图；
终端模 8 门再以独立奇偶状态筛选。由此，正、负根均被压成覆盖全部
\(\Delta\) 的显式有限字母 Hensel 递推族。

但每个符号在深度 \(3\Delta\) 上仍有
\(5^{3\Delta-1}\) 个二循环；现有 Jacobi、模 8、外部素数和大小门均未
统一关闭任一符号，也未给 \(\Delta\) 绝对界。因此准确分类为

\[
\boxed{
\mathrm{GAL\text{-}2}:
\quad
\text{低 }\varphi\text{ 区完成深提升 involution、仿射恢复、}
\text{每状态指数段及覆盖全部深度的 Hensel 递推。}
}
\]

没有找到合法原题六元组，也没有发现继承错误。本文到此停止，不研究高
\(\varphi\) 的 \(\mathcal F_{P-}\)、B、C、\(\gamma>1\)、C2/C5、
Q 或严格层。
