# 三项十进制拼接平方和问题：临界 G 模板 A2 低 \(\varphi\) 第一深带负根报告

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

中的第一深带负根区域

\[
\boxed{
\mathcal L_{\mathrm{d1},-}:
\quad
\sigma=-1,\qquad
2\varphi<3(a-\varphi)\le4\varphi.
}
\tag{0.1}
\]

接受 PR6、SD6、GA2-6、GE2-1、GAL-2、GALS\((+)\)-3、
GALS((-))-3 与 GALD1((+))-3 中同本分支相容的冻结结论。本文不研究
第一深带正根、\(3(a-\varphi)>4\varphi\) 的更深终端系统、浅正负根、高
\(\varphi\) 的 \(\mathcal F_{P-}\)、B、C、\(\gamma>1\)、非本原
C2/C5、Q 或严格层。

本轮得到以下严格结论。

1. 负根 Möbius involution 严格分解为模 \(C\) 的平移反射低块和模
   \(\Omega\) 的商 involution；商系数继续满足单位行列式恒等式，正向、
   反向商矩阵严格互逆。
2. 第一深带有 \(\Omega\mid C\)，故商 involution 再次退化为显式仿射
   反射
   \[
   L=\langle\Theta_u-T\rangle_\Omega.
   \]
   因而逐位 Hensel 树完全消失。
3. 原 involution 的唯一固定点同时是低块和商层固定点，并被精确负根门
   删除；其余状态均为非平凡二循环。商层固定点本身通常不是原固定点。
4. 商层基础余数具有闭式，第一次二进下降产生严格正缺陷
   \[
   2^\delta10^\mu=zr-\mathcal D_{u,T},\qquad
   \mathcal D_{u,T}>0.
   \]
5. 缺陷与 \(r\) 互素，离散对数目标统一塌缩为
   \[
   2^{2a+h}10^{\mu+2a+\Delta}\equiv-1\pmod r.
   \]
   每个固定局部状态至多剩一条完整有限指数同余段。
6. 共轭和差满足
   \[
   v_2(q-r)=2a+1,\quad v_5(q-r)=2\varphi,
   \quad v_2(q+r)=1,\quad v_5(q+r)=0,
   \]
   且 \(q=r\) 不可能；\(q<r\) 只可能发生在最小 \(z\) 端点。
7. 从商图可抽取任意更深负根的带符号块递归：每层输入低块唯一决定输出
   低块，单位行列式与正反矩阵互逆性逐层保持，末层在剩余深度不超过
   \(2\varphi\) 时反射化。

现有离散对数、Jacobi、和差、赋值与严格大小门没有统一关闭任一低块室、
商进位室或边界射线，也没有给 \(a,\Delta\) 绝对上界。因此准确分类为

\[
\boxed{
\mathrm{GALD1}((-))\text{-}3:
\quad
\text{完成两级仿射反射、正缺陷下降、一般负根块递归和每状态唯一有限指数段，}
\text{但仍有无界残余。}
}
\tag{0.2}
\]

没有找到合法原题六元组，也没有发现 GALD1((+))-3、GALS((-))-3、
GALS((+))-3、GAL-2、GE2-1、GA2-6、PR6 或 SD6 的继承错误。

---

## 1. 参数范围与第一深带整数化

定义

\[
\boxed{\Delta=a-\varphi\ge1.}
\tag{1.1}
\]

第一深带条件严格等价于

\[
\boxed{
\left\lfloor\frac{2a}{5}\right\rfloor+1
\le\Delta\le
\left\lfloor\frac{4a}{7}\right\rfloor,
\qquad
\varphi=a-\Delta.
}
\tag{1.2}
\]

该区间从 \(a=4\) 开始才可能非空。置

\[
\boxed{
M=2^{2a},\qquad
C=5^{2\varphi},\qquad
\Lambda=5^{3\Delta},\qquad
B=MC.
}
\tag{1.3}
\]

定义剩余深度

\[
\boxed{\chi=3\Delta-2\varphi>0,\qquad \Omega=5^\chi.}
\tag{1.4}
\]

由指数相加，

\[
C\Omega
=5^{2\varphi+3\Delta-2\varphi}
=5^{3\Delta}
=\Lambda,
\]

故

\[
\boxed{\Lambda=C\Omega.}
\tag{1.5}
\]

第一深带上界 \(3\Delta\le4\varphi\) 等价于
\(\chi\le2\varphi\)，所以

\[
\boxed{\Omega\mid C.}
\tag{1.6}
\]

定义

\[
\boxed{
\Gamma=\frac C\Omega
=5^{4\varphi-3\Delta}\in\mathbb Z_{\ge1}.
}
\tag{1.7}
\]

边界 \(3\Delta=4\varphi\) 等价于

\[
\boxed{
(a,\Delta,\varphi)=(7t,4t,3t),\qquad
\Omega=C,\quad\Gamma=1,\qquad t\ge1.
}
\tag{1.8}
\]

它是一条无界整数射线，完整包含在本文内。

尾窗沿用

\[
\mathcal H(a)=
\{h\ge0:2^{2a-2}\le5^{h+1},\ 5^h<2^{2a-1}\},
\tag{1.9}
\]

\[
h\in\mathcal H(a),\qquad
e=2a+\Delta+h.
\]

置

\[
\boxed{\delta=\Delta+h,\qquad e=2a+\delta.}
\tag{1.10}
\]

---

## 2. 负根基础数据与模 \(C\) 的低块反射

定义

\[
\boxed{x=\langle2C^{-1}\rangle_M,}
\tag{2.1}
\]

\[
\boxed{Cx=2+Mc,}
\tag{2.2}
\]

\[
\boxed{
\rho=Cx-1=1+Mc,
\qquad
\eta=cx.
}
\tag{2.3}
\]

继承系统并可直接复核

\[
0<x<M,\qquad0<c<C,\qquad0<\rho<B,
\tag{2.4}
\]

\[
\boxed{\rho^2=1+B\eta.}
\tag{2.5}
\]

精确五进门与终端模 \(8\) 门分别是

\[
\boxed{x+M\tau\equiv2\text{ 或 }3\pmod5,}
\tag{2.6}
\]

\[
\boxed{c+J+\tau\equiv1\pmod2,\qquad J\in\{1,\ldots,9\}.}
\tag{2.7}
\]

对每个 \(0\le\tau<\Lambda=C\Omega\)，唯一写成

\[
\boxed{
\tau=u+CT,
\qquad0\le u<C,quad0\le T<\Omega.
}
\tag{2.8}
\]

因 \(5\mid C\)，根门只看低块：

\[
\boxed{x+Mu\equiv2\text{ 或 }3\pmod5.}
\tag{2.9}
\]

定义

\[
\boxed{
\vartheta=\langle\eta\rangle_C\in\{0,\ldots,C-1\}.
}
\tag{2.10}
\]

由 \(Mc=Cx-2\)，乘以 \(x\) 得

\[
M\eta=Cx^2-2x\equiv-2x\pmod C.
\]

所以

\[
\boxed{M\vartheta\equiv-2x\pmod C.}
\tag{2.11}
\]

负根 involution 为

\[
\lambda_\tau=
\left\langle
-(\eta+\rho\tau)(\rho+B\tau)^{-1}
\right\rangle_\Lambda.
\tag{2.12}
\]

模 \(C\) 有

\[
\rho=Cx-1\equiv-1\pmod C,
\qquad B\equiv0\pmod C,
\]

故

\[
\lambda_\tau
\equiv-(\eta-u)(-1)^{-1}
\equiv\eta-u
\equiv\vartheta-u\pmod C.
\]

定义标准低块

\[
\boxed{
\bar u=\langle\vartheta-u\rangle_C
\in\{0,\ldots,C-1\}.
}
\tag{2.13}
\]

存在唯一 \(\epsilon_u\in\{0,1\}\) 使

\[
\boxed{u+\bar u=\vartheta+\epsilon_uC.}
\tag{2.14}
\]

两个互斥低块室为

\[
\boxed{
0\le u\le\vartheta
\Longrightarrow
\bar u=\vartheta-u,quad\epsilon_u=0,
}
\tag{2.15a}
\]

\[
\boxed{
\vartheta<u<C
\Longrightarrow
\bar u=\vartheta+C-u,quad\epsilon_u=1.
}
\tag{2.15b}
\]

于是 \(\lambda_\tau\) 唯一写成

\[
\boxed{
\lambda_\tau=\bar u+CL,
\qquad0\le L<\Omega.
}
\tag{2.16}
\]

由 (2.11)、(2.13)，

\[
x+M\bar u
\equiv x+M(\vartheta-u)
\equiv-(x+Mu)\pmod C.
\]

因此

\[
\boxed{x+M\bar u\equiv-(x+Mu)\pmod C.}
\tag{2.17}
\]

模 \(5\) 时两个合法数字 \(2,3\) 被交换，低块反射严格保持精确负根门。

---

## 3. 低块基础数字与原层固定点

由 (2.10) 定义

\[
\boxed{g=\frac{\eta-\vartheta}{C}\in\mathbb Z_{\ge0}.}
\tag{3.1}
\]

再定义

\[
\boxed{s_C=\frac{\eta+\rho\vartheta}{C}.}
\tag{3.2}
\]

使用 \(\eta=\vartheta+Cg\) 与 \(\rho=Cx-1\)，

\[
\eta+\rho\vartheta
=\vartheta+Cg+(Cx-1)\vartheta
=C(g+x\vartheta),
\]

故

\[
\boxed{s_C=g+x\vartheta\in\mathbb Z_{\ge0}.}
\tag{3.3}
\]

事实上 \(\eta=cx>0\)，而 \(\rho\vartheta\ge0\)，所以 (3.2) 的正分子
给出更强结论

\[
\boxed{s_C>0.}
\tag{3.4}
\]

GAL-2 的负根固定点方程为

\[
B\tau^2+2\rho\tau+\eta\equiv0\pmod\Lambda.
\]

整数恒等式

\[
B\tau^2+2\rho\tau+\eta
=(x+M\tau)(c+C\tau)
\tag{3.5}
\]

与 \(5\nmid c\) 说明第二因子是五进单位，故固定点唯一：

\[
\boxed{
\tau_*=\langle-xM^{-1}\rangle_\Lambda.
}
\tag{3.6}
\]

其低块为

\[
u_*=\langle-xM^{-1}\rangle_C.
\tag{3.7}
\]

由 (2.11)，

\[
2u_*\equiv-2xM^{-1}\equiv\vartheta\pmod C,
\]

所以

\[
\boxed{u_*=\bar u_*.}
\tag{3.8}
\]

但

\[
\boxed{x+M\tau_*\equiv0\pmod\Lambda,}
\tag{3.9}
\]

特别地模 \(5\) 为零，违反 (2.6)。原 involution 的唯一固定点被精确负根
门删除。

必须区分：对任意低块 \(u\)，商反射都有一个商层固定点；只有当
\(u=\bar u\) 且商坐标也固定时，才是原层固定点。

---

## 4. 商 Möbius 图、单位行列式与互逆矩阵

原 involution 图等价于

\[
\eta+\rho(\tau+\lambda_\tau)+B\tau\lambda_\tau
\equiv0\pmod\Lambda.
\tag{4.1}
\]

把 (2.8)、(2.14)、(2.16) 代入并除出一个 \(C\)：

\[
\boxed{
\eta+\rho(\tau+\lambda_\tau)+B\tau\lambda_\tau
=C\,H_u(T,L),
}
\tag{4.2}
\]

其中

\[
\boxed{
H_u(T,L)=\eta_u+\alpha_uT+\beta_uL+\mathcal BTL,
}
\tag{4.3}
\]

\[
\boxed{
\eta_u=s_C+\epsilon_u\rho+Mu\bar u,
}
\tag{4.4}
\]

\[
\boxed{
\alpha_u=\rho+B\bar u,
\qquad
\beta_u=\rho+Bu,
\qquad
\mathcal B=BC=MC^2.
}
\tag{4.5}
\]

因 \(\Lambda=C\Omega\)，(4.1) 与 (4.2) 严格等价于

\[
\boxed{H_u(T,L)\equiv0\pmod\Omega.}
\tag{4.6}
\]

下面独立核对单位行列式。展开得

\[
\begin{aligned}
\alpha_u\beta_u-\mathcal B\eta_u
={}&\rho^2+\rho B(u+\bar u)+B^2u\bar u\\
&-MC^2(s_C+\epsilon_u\rho+Mu\bar u).
\end{aligned}
\]

利用 \(u+\bar u=\vartheta+\epsilon_uC\)、
\(Cs_C=\eta+\rho\vartheta\) 和 \(B=MC\)，全部交叉项消去，剩下

\[
\rho^2-B\eta=1.
\]

所以

\[
\boxed{\alpha_u\beta_u-\mathcal B\eta_u=1.}
\tag{4.7}
\]

交换低块时 \(\epsilon_{\bar u}=\epsilon_u\)，从而

\[
\boxed{
\eta_{\bar u}=\eta_u,
\qquad
\alpha_{\bar u}=\beta_u,
\qquad
\beta_{\bar u}=\alpha_u.
}
\tag{4.8}
\]

定义

\[
\boxed{
\mathcal M_u=
\begin{pmatrix}
-\alpha_u&-\eta_u\\
\mathcal B&\beta_u
\end{pmatrix}.
}
\tag{4.9}
\]

由 (4.7)–(4.8) 逐项相乘，得到整数矩阵恒等式

\[
\boxed{\mathcal M_{\bar u}\mathcal M_u=I.}
\tag{4.10}
\]

全部分母模 \(5\) 都同余于 \(\rho\equiv-1\)，所以 (4.10) 在模
\(\Omega\) 的分式线性作用中严格给出两个低块纤维间的互逆商图。

---

## 5. 第一深带中的商反射退化

由 \(\Omega\mid C\)，

\[
B\equiv\mathcal B\equiv0\pmod\Omega,
\qquad
\rho=Cx-1\equiv-1\pmod\Omega.
\tag{5.1}
\]

因此

\[
\alpha_u\equiv\beta_u\equiv-1\pmod\Omega,
\]

而商条件 (4.6) 退化为

\[
\eta_u-T-L\equiv0\pmod\Omega.
\]

定义

\[
\boxed{
\Theta_u=\langle\eta_u\rangle_\Omega
\in\{0,\ldots,\Omega-1\}.
}
\tag{5.2}
\]

由 \(\eta_{\bar u}=\eta_u\)，

\[
\boxed{\Theta_{\bar u}=\Theta_u.}
\tag{5.3}
\]

商 involution 的唯一标准代表为

\[
\boxed{L=\langle\Theta_u-T\rangle_\Omega.}
\tag{5.4}
\]

定义唯一 \(\epsilon_{u,T}\in\{0,1\}\) 使

\[
\boxed{T+L=\Theta_u+\epsilon_{u,T}\Omega.}
\tag{5.5}
\]

两个互斥商反射室为

\[
\boxed{
0\le T\le\Theta_u
\Longrightarrow
L=\Theta_u-T,quad\epsilon_{u,T}=0,
}
\tag{5.6a}
\]

\[
\boxed{
\Theta_u<T<\Omega
\Longrightarrow
L=\Theta_u+\Omega-T,quad\epsilon_{u,T}=1.
}
\tag{5.6b}
\]

式 (5.4)–(5.6) 对每个 \((u,T)\) 唯一给出输出块与进位，不含任何
逐位选择。因此

\[
\boxed{\text{第一深带负根不再需要逐位 Hensel 递推。}}
\tag{5.7}
\]

---

## 6. 固定点、二循环与终端奇偶门

块坐标中的原 involution 是

\[
\boxed{(u,T)\longmapsto(\bar u,L).}
\tag{6.1}
\]

原固定点必须同时满足

\[
u=\bar u,
\qquad
T=L.
\tag{6.2}
\]

第一式模 \(C\) 有唯一解 \(u=u_*\)，第二式模 \(\Omega\) 也有唯一解

\[
T=T_*:=\langle2^{-1}\Theta_{u_*}\rangle_\Omega.
\tag{6.3}
\]

由原 involution 固定点的唯一性，(6.2)–(6.3) 正是 (3.6) 的块坐标。
它已由 (3.9) 删除。其余通过根门的状态全部组成非平凡二循环。

对任意 \(u\)，商反射本身都有唯一固定坐标

\[
\boxed{T_u^\dagger=\langle2^{-1}\Theta_u\rangle_\Omega.}
\tag{6.4}
\]

若 \(u\ne\bar u\)，状态
\((u,T_u^\dagger)\) 与 \((\bar u,T_u^\dagger)\) 仍构成非平凡原层
二循环。因此不得把 (6.4) 自动误作原固定点。

因 \(C,\Omega\) 均为奇数，

\[
\tau\equiv u+T\pmod2,
\qquad
\lambda_\tau\equiv\bar u+L\pmod2.
\]

结合 (2.14)、(5.5)，得到

\[
\boxed{
\tau+\lambda_\tau
\equiv
\vartheta+\epsilon_u+\Theta_u+\epsilon_{u,T}
\pmod2.
}
\tag{6.5}
\]

记

\[
p_{u,J}=\langle1-c-J-u\rangle_2,
\tag{6.6}
\]

则当前端点通过终端门当且仅当 \(T\equiv p_{u,J}\pmod2\)。再记

\[
S_{u,T}=\langle
\vartheta+\epsilon_u+\Theta_u+\epsilon_{u,T}
\rangle_2.
\tag{6.7}
\]

一个二循环的精确判别为：

\[
\boxed{
\begin{array}{c|c}
S_{u,T}=1&\text{两端奇偶相反，终端门恰保留一端}\;\\
S_{u,T}=0, T\equiv p_{u,J}\pmod2&\text{两端同时保留}\;\\
S_{u,T}=0, T\not\equiv p_{u,J}\pmod2&\text{两端同时删除}.
\end{array}}
\tag{6.8}
\]

所以不能声称每个二循环自动留下一个端点。

---

## 7. 不遍历 \(\Lambda\) 个 \(\tau\) 的精确状态计数

### 7.1 两个低块进位室

对 \(d\in\{2,3\}\)，定义

\[
\alpha_d=\langle M^{-1}(d-x)\rangle_5.
\tag{7.1}
\]

再定义

\[
F_5(X;\alpha)=
\begin{cases}
0,&X<\alpha,\\[1mm]
\left\lfloor\dfrac{X-\alpha}{5}\right\rfloor+1,&X\ge\alpha.
\end{cases}
\tag{7.2}
\]

根门低块集合为

\[
\mathcal U=
\{0\le u<C:x+Mu\equiv2,3\pmod5\},
\qquad |\mathcal U|=\frac{2C}{5}.
\tag{7.3}
\]

两个低块进位室的精确有向低块数为

\[
\boxed{
U_0=\sum_{d\in\{2,3\}}F_5(\vartheta;\alpha_d),
\qquad
U_1=\frac{2C}{5}-U_0.
}
\tag{7.4}
\]

### 7.2 商进位、奇偶门与 \(A\)-大小室

定义

\[
\pi_p(X)=\#\{0\le t\le X:t\equiv p\pmod2\},
\qquad p\in\{0,1\},
\tag{7.5}
\]

其中 \(X<0\) 时取零；\(X\ge0\) 时

\[
\pi_p(X)=
\begin{cases}
0,&X<p,\\[1mm]
\left\lfloor\dfrac{X-p}{2}\right\rfloor+1,&X\ge p.
\end{cases}
\]

令

\[
\Pi_p(A,B)=\pi_p(B)-\pi_p(A-1).
\tag{7.6}
\]

对固定 \(u\)，两个商室区间是

\[
I_{u,0}=[0,\Theta_u],
\qquad
I_{u,1}=[\Theta_u+1,\Omega-1].
\tag{7.7}
\]

第 8 节将定义 \(\Sigma_u\)，这里先记

\[
A_{u,f}=J+f+\Sigma_u,
\qquad f\in\{0,1\}.
\tag{7.8}
\]

则同时区分低块进位 \(e\)、商进位 \(f\)、终端奇偶门和
\((k-1)M<A_{u,T}\le kM\) 大小室的精确有向状态数为

\[
\boxed{
\mathcal N_{e,f,k}(J)
=
\sum_{\substack{u\in\mathcal U\\ \epsilon_u=e}}
\mathbf1_{(k-1)M<A_{u,f}\le kM}\,
\Pi_{p_{u,J}}(I_{u,f}).
}
\tag{7.9}
\]

这里 \(\Pi_p([A,B])\) 表示 (7.6)；空区间贡献零。式 (7.9) 只对
\(2C/5\) 个低块作闭式区间计数，不遍历 \(C\Omega=\Lambda\) 个
\(\tau\)。它也明确允许任意 \(k\ge1\)，没有预设 \(A_{u,T}<M\)。

### 7.3 原固定点、商固定点与零/一/双端循环

原图有且只有一个固定点，但根门后固定点数为零。根门前，它位于唯一低块
自配对 \(u_*\) 和唯一商固定坐标 \(T_*\)。

每个 \(u\in\mathcal U\) 有一个商固定坐标 (6.4)。根门后的商固定有向
状态数是 \(2C/5\)，对应 \(C/5\) 个原层非平凡二循环；通过终端门的
数目为

\[
\sum_{u\in\mathcal U}
\mathbf1_{T_u^\dagger\equiv p_{u,J}\ (2)}.
\tag{7.10}
\]

为对全部二循环计数，取每个根门二循环中首位数字为 \(2\) 的唯一代表：

\[
\mathcal U_2=
\{0\le u<C:x+Mu\equiv2\pmod5\},
\qquad |\mathcal U_2|=\frac C5.
\tag{7.11}
\]

因此根门后原二循环总数恰为

\[
\boxed{\frac C5\Omega=\frac\Lambda5.}
\tag{7.12}
\]

对 \(f\in\{0,1\}\) 置

\[
s_{u,f}=\langle\vartheta+\epsilon_u+\Theta_u+f\rangle_2,
\qquad
n_{u,f}=|I_{u,f}|.
\tag{7.13}
\]

则终端奇偶门保留一端、两端、零端的二循环数分别为

\[
\boxed{
N_1(J)=
\sum_{u\in\mathcal U_2}\sum_{f=0}^1
\mathbf1_{s_{u,f}=1}\,n_{u,f},
}
\tag{7.14}
\]

\[
\boxed{
N_2(J)=
\sum_{u\in\mathcal U_2}\sum_{f=0}^1
\mathbf1_{s_{u,f}=0}\,
\Pi_{p_{u,J}}(I_{u,f}),
}
\tag{7.15}
\]

\[
\boxed{
N_0(J)=
\sum_{u\in\mathcal U_2}\sum_{f=0}^1
\mathbf1_{s_{u,f}=0}\,
\{n_{u,f}-\Pi_{p_{u,J}}(I_{u,f})\}.
}
\tag{7.16}
\]

并有精确核对

\[
\boxed{N_0(J)+N_1(J)+N_2(J)=\frac\Lambda5.}
\tag{7.17}
\]

这一区分完整覆盖两个低块室、两个商进位室、商固定点、被删原固定点及
奇偶门的零/一/双端行为。它是块参数化计数，不是叶节点数绝对有界结论。

---

## 8. 商层基础余数闭式与终端恒等式

定义

\[
\boxed{
g_u=\frac{\eta_u-\Theta_u}{\Omega}\in\mathbb Z_{\ge0},
}
\tag{8.1}
\]

\[
\boxed{\Sigma_u=g_u+\Gamma x\Theta_u,}
\tag{8.2}
\]

\[
\boxed{S_u(T,L)=\bar uT+uL+CTL.}
\tag{8.3}
\]

由

\[
\eta_u=\Theta_u+g_u\Omega,
\qquad
T+L=\Theta_u+\epsilon_{u,T}\Omega,
\]

以及

\[
1+\rho=Cx=\Gamma\Omega x,
\]

把 (4.3) 除以 \(\Omega\)，逐项得到

\[
\boxed{
s_0
=\frac{H_u(T,L)}{\Omega}
=\Sigma_u+\rho\epsilon_{u,T}+M\Gamma S_u(T,L).
}
\tag{8.4}
\]

这不是形式类比，而是原正整数余数

\[
s_0=
\frac{\eta+\rho(\tau+\lambda_\tau)+B\tau\lambda_\tau}{\Lambda}.
\tag{8.5}
\]

因 \(\eta>0\)、\(\rho>0\) 且其余量非负，

\[
\boxed{s_0>0.}
\tag{8.6}
\]

定义

\[
\boxed{
V=J\Lambda+\tau
=JC\Omega+u+CT,
}
\tag{8.7}
\]

\[
\boxed{r=\rho+BV,}
\tag{8.8}
\]

\[
\boxed{q_0=\rho+B(\bar u+CL),}
\tag{8.9}
\]

\[
\boxed{N_0=Jq_0+s_0.}
\tag{8.10}
\]

直接展开并使用 \(\rho^2=1+B\eta\) 与 (8.5)，得到

\[
\boxed{q_0r=1+B\Lambda N_0.}
\tag{8.11}
\]

令 \(R_\tau=\rho+B\tau\)。由内层恒等式

\[
q_0R_\tau=1+B\Lambda s_0.
\]

而 \(0<R_\tau<B\Lambda\)，所以

\[
\boxed{0<s_0<q_0.}
\tag{8.12}
\]

同理由 \(0<q_0<B\Lambda\) 与 (8.11) 得

\[
\boxed{0<N_0<r.}
\tag{8.13}
\]

完整仿射恢复为

\[
\boxed{q=q_0+B\Lambda y,}
\tag{8.14}
\]

\[
\boxed{s=s_0+(\rho+B\tau)y,}
\tag{8.15}
\]

\[
\boxed{N=N_0+ry,}
\tag{8.16}
\]

\[
\boxed{y\in\mathbb Z_{\ge0}.}
\tag{8.17}
\]

式 (8.11)、(8.14)–(8.16) 与终端方程
\(qr=1+B\Lambda N\)、\(N=Jq+s\) 严格双向。

还需记录两个零端点。由 \(s_C>0\)，有 \(\eta_u>0\)。若
\(\Sigma_u=0\)，则 \(g_u=\Theta_u=0\)，从而 \(\eta_u=0\)，矛盾。
因此

\[
\boxed{\Sigma_u>0.}
\tag{8.18}
\]

---

## 9. 第一次二进下降与严格正缺陷

真实指数写成

\[
\boxed{
N=2^e10^\mu,
\qquad e=2a+\delta,
\qquad \mu\ge0.
}
\tag{9.1}
\]

所以 \(M\mid N\)。由

\[
\rho\equiv1\pmod M,
\qquad
M\mid M\Gamma S_u,
\]

式 (8.4)、(8.10) 给

\[
N_0\equiv J+\epsilon_{u,T}+\Sigma_u\pmod M.
\]

定义原正整数

\[
\boxed{
A_{u,T}=J+\epsilon_{u,T}+\Sigma_u\ge1.
}
\tag{9.2}
\]

不把它预先约成模 \(M\) 的标准数字。由
\(N=N_0+ry\)、\(r\equiv1\pmod M\)，

\[
\boxed{y\equiv-A_{u,T}\pmod M.}
\tag{9.3}
\]

所以唯一写成

\[
\boxed{y=Mz-A_{u,T},}
\tag{9.4}
\]

其中

\[
\boxed{
z\ge z_0:=\left\lceil\frac{A_{u,T}}M\right\rceil.
}
\tag{9.5}
\]

定义

\[
\boxed{
\mathcal D_{u,T}
=\frac{A_{u,T}r-N_0}{M}.
}
\tag{9.6}
\]

由 (8.13) 与 \(A_{u,T}\ge1\)，

\[
A_{u,T}r-N_0\ge r-N_0>0.
\]

故

\[
\boxed{\mathcal D_{u,T}>0.}
\tag{9.7}
\]

为得到显式闭式，使用

\[
A_{u,T}-J=\epsilon_{u,T}+\Sigma_u,
\]

以及 (8.4)、\(\rho-1=Mc\)、\(B=MC=M\Gamma\Omega\)。逐项化简

\[
A_{u,T}r-N_0
=(A_{u,T}-J)\rho+B(A_{u,T}V-J\lambda_\tau)-s_0
\]

后得到

\[
\boxed{
\mathcal D_{u,T}
=c\Sigma_u
+\Gamma\left[
\Omega\left(
A_{u,T}V-J(\bar u+CL)
\right)
-S_u(T,L)
\right].
}
\tag{9.8}
\]

将 (9.4) 代入 (8.16)：

\[
N=N_0+r(Mz-A_{u,T})
=M(zr-\mathcal D_{u,T}).
\]

再用 \(N/M=2^\delta10^\mu\)，得到

\[
\boxed{
2^\delta10^\mu=zr-\mathcal D_{u,T}.
}
\tag{9.9}
\]

反向地，固定局部状态，任取满足 (9.5)、\(\mu\ge0\) 与 (9.9) 的
整数 \((z,\mu)\)，用 (9.4) 定义 \(y\)。则 \(y\ge0\)，且

\[
N_0+ry=M2^\delta10^\mu=2^e10^\mu.
\]

再由 (8.14)–(8.16) 唯一恢复 \(q,s,N\)。所以 (9.9) 与原仿射终端状态
严格双向，不只是必要同余。

特别地

\[
\boxed{\mathcal D_{u,T}=0\text{ 不可能}.}
\tag{9.10}
\]

---

## 10. 缺陷互素性、统一离散对数与完整有限指数段

由 (9.6)，

\[
M\mathcal D_{u,T}=A_{u,T}r-N_0.
\tag{10.1}
\]

式 (8.11) 自动给 \(\gcd(N_0,r)=1\)，而
\(r\equiv1\pmod M\) 给 \(\gcd(M,r)=1\)。若某素数同时整除
\(\mathcal D_{u,T}\) 与 \(r\)，由 (10.1) 也整除 \(N_0\)，矛盾。
因此

\[
\boxed{\gcd(\mathcal D_{u,T},r)=1.}
\tag{10.2}
\]

核心方程模 \(r\) 给

\[
\boxed{
10^\mu\equiv-2^{-\delta}\mathcal D_{u,T}\pmod r.
}
\tag{10.3}
\]

另一方面，(8.11) 给

\[
B\Lambda N_0\equiv-1\pmod r,
\]

而 (10.1) 给

\[
M\mathcal D_{u,T}\equiv-N_0\pmod r.
\]

消去 \(N_0\)，得到

\[
\boxed{
\mathcal D_{u,T}
\equiv(MB\Lambda)^{-1}
=(M^2C^2\Omega)^{-1}
\pmod r.
}
\tag{10.4}
\]

因

\[
M^2C^2\Omega
=2^{4a}5^{2\varphi+3\Delta}
=2^{4a}5^{2a+\Delta},
\]

(10.3) 严格等价于

\[
\boxed{
2^{2a+h}10^{\mu+2a+\Delta}\equiv-1\pmod r.
}
\tag{10.5}
\]

这与浅负根和第一深带正根的统一目标完全一致。

由 \(r\equiv1\pmod M\)、\(r\equiv-1\pmod5\)，有
\(\gcd(r,10)=1\)。令

\[
\boxed{P_r=\operatorname{ord}_r(10).}
\tag{10.6}
\]

若 (10.3) 的右端不属于
\(\langle10\rangle\subset(\mathbb Z/r\mathbb Z)^\times\)，删除整个
状态。若属于，则存在唯一 \(\mu_0\in\{0,\ldots,P_r-1\}\) 使

\[
\boxed{\mu\equiv\mu_0\pmod{P_r}.}
\tag{10.7}
\]

每个指数唯一恢复

\[
\boxed{
z=\frac{\mathcal D_{u,T}+2^\delta10^\mu}{r}.
}
\tag{10.8}
\]

### 10.1 精确下端

定义

\[
y_0=Mz_0-A_{u,T}\in\{0,\ldots,M-1\},
\tag{10.9}
\]

\[
\boxed{D_0=z_0r-\mathcal D_{u,T}.}
\tag{10.10}
\]

由 (10.1)，

\[
MD_0=y_0r+N_0>0,
\]

所以

\[
\boxed{D_0>0.}
\tag{10.11}
\]

式 (10.8) 满足 \(z\ge z_0\) 当且仅当

\[
2^\delta10^\mu\ge D_0.
\]

定义完全整数化下端

\[
\boxed{
\mu_{\min}
=\min\{v\in\mathbb Z_{\ge0}:2^\delta10^v\ge D_0\}.
}
\tag{10.12}
\]

等号端点完整保留。

### 10.2 严格大小门与上端

继承大小门为

\[
20\cdot10^m<194029\,\mathfrak Z^2Y,
\qquad
\mathfrak Z=\frac{B\Lambda}{2},
\qquad
Y=10^{3a},
\qquad
m=e+\mu.
\tag{10.13}
\]

置

\[
\mathscr X=194029\,\mathfrak Z^2Y,
\tag{10.14}
\]

\[
\boxed{
Q_\mu=
\left\lfloor
\frac{\mathscr X-1}{20\cdot10^e}
\right\rfloor.
}
\tag{10.15}
\]

若 \(Q_\mu<1\)，该状态为空。否则定义

\[
\boxed{
\mu_{\max}
=\max\{v\in\mathbb Z_{\ge0}:10^v\le Q_\mu\}.
}
\tag{10.16}
\]

它满足严格相邻阈值

\[
\boxed{
20\cdot10^{e+\mu_{\max}}
<\mathscr X
\le20\cdot10^{e+\mu_{\max}+1}.
}
\tag{10.17}
\]

### 10.3 唯一完整有限指数段

若离散对数存在，定义

\[
t_{\min}
=\max\left(
0,
\left\lceil\frac{\mu_{\min}-\mu_0}{P_r}\right\rceil
\right),
\tag{10.18}
\]

\[
t_{\max}
=\left\lfloor\frac{\mu_{\max}-\mu_0}{P_r}\right\rfloor.
\tag{10.19}
\]

若 \(t_{\min}>t_{\max}\)，状态为空；否则全部指数恰为

\[
\boxed{
\mu=\mu_0+tP_r,
\qquad
t_{\min}\le t\le t_{\max}.
}
\tag{10.20}
\]

每个指数由 (10.8)、(9.4)、(8.14)–(8.16) 唯一恢复全部终端整数。
这是完整有限同余段，不是有限采样 \(\mu\)。对应的准确整数上端为

\[
\boxed{
z\le
z_{\max}:=
\left\lfloor
\frac{\mathcal D_{u,T}+2^\delta10^{\mu_{\max}}}{r}
\right\rfloor.
}
\tag{10.21}
\]

这里必须使用 \(\le\)；若最大指数恰整除，等号可以发生。

---

## 11. 原商、共轭和差与精确赋值

为避免与商层变量 \(L\) 淆乱，定义原 GAL-2 商

\[
\boxed{\mathscr L=\lambda_\tau+\Lambda y.}
\tag{11.1}
\]

代入 \(\lambda_\tau=\bar u+CL\)、\(\Lambda=C\Omega\) 与
\(y=Mz-A_{u,T}\)，得到

\[
\boxed{
\mathscr L
=\bar u+C\{L+\Omega(Mz-A_{u,T})\}.
}
\tag{11.2}
\]

同时

\[
\boxed{V=u+C(T+J\Omega).}
\tag{11.3}
\]

于是

\[
q=\rho+B\mathscr L,
\qquad
r=\rho+BV,
\tag{11.4}
\]

\[
q-r=B(\mathscr L-V),
\qquad
q+r=2\rho+B(\mathscr L+V).
\tag{11.5}
\]

### 11.1 \(q=r\) 与符号

若 \(q=r\)，则 \(\mathscr L=V\)。模 \(\Lambda\) 得
\(\lambda_\tau=\tau\)，即原 involution 固定点；该点已由根门删除。
所以

\[
\boxed{q=r\text{ 不可能}.}
\tag{11.6}
\]

更精确地，

\[
\mathscr L-V
=\lambda_\tau-\tau+\Lambda(y-J),
\]

故

\[
\boxed{
\begin{array}{c|c}
y\le J-1&q<r\\
y\ge J+1&q>r\\
y=J&\operatorname{sgn}(q-r)=\operatorname{sgn}(\lambda_\tau-\tau).
\end{array}}
\tag{11.7}
\]

若 \(z\ge z_0+1\)，则 \(y=y_0+M\ge M>J\)，故

\[
\boxed{q<r\text{ 只可能发生在最小 }z=z_0.}
\tag{11.8}
\]

最小端点本身不能先验删除；特别地，\(y=0\) 当且仅当

\[
\boxed{M\mid A_{u,T},\qquad z=z_0=A_{u,T}/M.}
\tag{11.9}
\]

此时 \(q<r\)。

### 11.2 五进赋值

由 (2.17) 模 \(5\)，

\[
M(\lambda_\tau-\tau)
\equiv-2(x+M\tau)\not\equiv0\pmod5.
\]

又 \(\mathscr L-V\equiv\lambda_\tau-\tau\pmod5\)，所以

\[
\boxed{v_5(q-r)=2\varphi.}
\tag{11.10}
\]

而 \(\rho\equiv-1\pmod5\)、\(5\mid B\) 给

\[
\boxed{v_5(q+r)=0.}
\tag{11.11}
\]

### 11.3 二进赋值的完整模 \(4\) 计算

先有 \(q+r\equiv2\pmod4\)，所以

\[
\boxed{v_2(q+r)=1.}
\tag{11.12}
\]

对差，令

\[
W=\mathscr L-V
=\bar u-u+C(L-T)+C\Omega(Mz-A_{u,T}-J).
\tag{11.13}
\]

需要精确证明 \(W\equiv2\pmod4\)。先记录

\[
C\equiv\Omega\equiv\Gamma\equiv1\pmod4,
\qquad
x\equiv2\pmod4,
\qquad
\rho\equiv1\pmod4.
\tag{11.14}
\]

由 \(\eta=cx=\vartheta+Cg\)，

\[
\vartheta+g\equiv2c\pmod4.
\]

结合 \(s_C=g+x\vartheta\)，得到

\[
s_C\equiv2c+\vartheta\pmod4.
\tag{11.15}
\]

又由 \(\eta_u=\Theta_u+g_u\Omega\) 与 (4.4)，

\[
g_u\equiv s_C+\epsilon_u-\Theta_u\pmod4.
\]

故

\[
\Sigma_u=g_u+\Gamma x\Theta_u
\equiv s_C+\epsilon_u+\Theta_u\pmod4.
\tag{11.16}
\]

现在使用两层进位式与 \(A_{u,T}=J+\epsilon_{u,T}+\Sigma_u\)，

\[
\begin{aligned}
W
&\equiv
\vartheta+\epsilon_u+\Theta_u-\Sigma_u
-2(u+T+J)\pmod4\\
&\equiv-2c-2(u+T+J)\pmod4.
\end{aligned}
\]

终端门 \(c+J+u+T\equiv1\pmod2\) 最终给

\[
\boxed{W\equiv2\pmod4.}
\tag{11.17}
\]

因此

\[
\boxed{v_2(q-r)=2a+1.}
\tag{11.18}
\]

式 (11.10)–(11.12)、(11.18) 是精确赋值，不是下界。

### 11.4 和差平方路线

把 (11.5) 代入

\[
(q-r)^2=(q+r)^2-4qr
\]

并使用 \(qr=1+B\Lambda N\)，只得到已有终端乘积的恒等回代。奇素数部分
仍随 \(\mathscr L-V\) 移动，没有新的固定平方分解或关闭门。

---

## 12. 任意更深负根的带符号块递归

第一深带的直接反射退化依赖 \(\Omega\mid C\)。当剩余深度超过
\(2\varphi\) 时，应从第 4 节的商图继续剥取 \(C\)-块，而不能把
(5.4) 直接用于整个更深区。

设某层图为

\[
G_j(X,Y)
=\eta_j+\alpha_jX+\beta_jY+\gamma_jXY
\equiv0\pmod{5^{n_j}},
\tag{12.1}
\]

并满足

\[
\boxed{
\alpha_j\beta_j-\gamma_j\eta_j=1,
\qquad
\alpha_j\equiv\beta_j\equiv-1\pmod C,
\qquad
C\mid\gamma_j.
}
\tag{12.2}
\]

若 \(n_j>2\varphi\)，写

\[
X=v+CX',
\qquad
Y=w+CY',
\qquad
0\le v,w<C.
\tag{12.3}
\]

模 \(C\) 时 (12.1) 退化为

\[
\eta_j-v-w\equiv0\pmod C.
\]

定义

\[
\theta_j=\langle\eta_j\rangle_C,
\]

则输出低块唯一为

\[
\boxed{w=\langle\theta_j-v\rangle_C.}
\tag{12.4}
\]

定义下一层系数

\[
\boxed{
\eta_{j+1}
=\frac{\eta_j+\alpha_jv+\beta_jw+\gamma_jvw}{C},
}
\tag{12.5}
\]

\[
\boxed{
\alpha_{j+1}=\alpha_j+\gamma_jw,
\qquad
\beta_{j+1}=\beta_j+\gamma_jv,
\qquad
\gamma_{j+1}=C\gamma_j.
}
\tag{12.6}
\]

式 (12.4) 保证 (12.5) 为整数。直接展开得到

\[
\frac{G_j(v+CX',w+CY')}{C}
=\eta_{j+1}+\alpha_{j+1}X'
+\beta_{j+1}Y'+\gamma_{j+1}X'Y'.
\tag{12.7}
\]

剩余模数为

\[
\boxed{n_{j+1}=n_j-2\varphi.}
\tag{12.8}
\]

而

\[
\begin{aligned}
\alpha_{j+1}\beta_{j+1}-\gamma_{j+1}\eta_{j+1}
={}&(\alpha_j+\gamma_jw)(\beta_j+\gamma_jv)\\
&-\gamma_j(\eta_j+\alpha_jv+\beta_jw+\gamma_jvw)\\
=&1.
\end{aligned}
\]

所以

\[
\boxed{
\alpha_{j+1}\beta_{j+1}-\gamma_{j+1}\eta_{j+1}=1.
}
\tag{12.9}
\]

由 \(C\mid\gamma_j\)，还保持

\[
\boxed{
\alpha_{j+1}\equiv\beta_{j+1}\equiv-1\pmod C,
\qquad
C\mid\gamma_{j+1}.
}
\tag{12.10}
\]

正向矩阵与交换 \(\alpha_j,\beta_j\) 后的反向矩阵分别为

\[
\mathcal M_j=
\begin{pmatrix}-\alpha_j&-\eta_j\\ \gamma_j&\beta_j\end{pmatrix},
\qquad
\mathcal M_j^\vee=
\begin{pmatrix}-\beta_j&-\eta_j\\ \gamma_j&\alpha_j\end{pmatrix}.
\]

由 (12.2)，

\[
\boxed{\mathcal M_j^\vee\mathcal M_j=I.}
\tag{12.11}
\]

交换输入、输出低块后，(12.5) 不变而 (12.6) 交换
\(\alpha_{j+1},\beta_{j+1}\)，所以正向、反向商图逐层严格互逆。

当最终剩余深度 \(0<n_j\le2\varphi\) 时，模数 \(5^{n_j}\mid C\)，
于是末层退化为

\[
\boxed{
Y=\langle\eta_j-X\rangle_{5^{n_j}}.
}
\tag{12.12}
\]

对原负根，第一低块由第 2 节给出。之后以

\[
(\eta_0,\alpha_0,\beta_0,\gamma_0)
=(\eta_u,\alpha_u,\beta_u,\mathcal B),
\qquad n_0=\chi
\tag{12.13}
\]

进入上述递归。把 \(\chi\) 唯一写成

\[
\chi=q(2\varphi)+r_0,
\qquad q\ge0,
\qquad0<r_0\le2\varphi,
\tag{12.14}
\]

并在整除时取 \(r_0=2\varphi\)，连续应用 (12.3)–(12.11) 共
\(q\) 次，再以 (12.12) 终结，即得到任意深度负根 involution 的一般
块正规形：

* 每个输入块唯一决定输出块；
* 每层都是状态依赖的平移反射；
* 单位行列式和正反互逆性逐层保持；
* 不存在逐位 Hensel 输出分支；
* 最后一块总是显式仿射反射。

本节只外推 involution 的块递归，不把第 9–11 节的第一深带终端缺陷、
赋值或指数段未经证明外推到更深带。

---

## 13. 完整生成顺序与终端充分性边界

第一深带负根的全部终端候选必须、且在终端层面只须按以下顺序生成。

1. 取
   \[
   a\ge3,
   \qquad
   \left\lfloor\frac{2a}{5}\right\rfloor+1
   \le\Delta\le
   \left\lfloor\frac{4a}{7}\right\rfloor,
   \qquad
   \varphi=a-\Delta.
   \]
2. 取 \(h\in\mathcal H(a)\)，置
   \(\delta=\Delta+h\)、\(e=2a+\delta\)。
3. 构造 \(M,C,\Lambda,\Omega,\Gamma,B,x,c,\rho,\eta,\vartheta,s_C\)。
4. 取 \(J\in\{1,\ldots,9\}\) 及
   \[
   u\in\mathcal U,
   \qquad0\le T<\Omega,
   \qquad c+J+u+T\equiv1\pmod2.
   \]
   可用第 7 节的低块等差类和两个商区间生成，不枚举
   \(\Lambda\) 个 \(\tau\)。
5. 唯一计算
   \[
   \bar u,\epsilon_u,\eta_u,\Theta_u,L,\epsilon_{u,T},g_u,\Sigma_u.
   \]
6. 构造第 8、9 节的 \(s_0,q_0,N_0,r,A_{u,T},\mathcal D_{u,T}\)。
7. 检查 (10.3) 或统一式 (10.5)。若离散对数不存在，删除整个状态；若
   存在，按 (10.20) 生成唯一完整有限指数段。
8. 对每个指数用 (10.8)、(9.4)、(11.2)、(8.14)–(8.16) 唯一恢复
   \(z,y,\mathscr L,q,s,N\)。
9. 最后进入继承的十三首块、\(a_2\) 窗口、判别式平方、两个恢复符号、
   精确 gcd 尺度、\(a_3\) 窗口、三个逐项既约条件和原题直接回代。

第 1–8 步在终端层严格双向；第 9 步仍是完整原题候选不可省略的恢复门。
本文没有把终端状态误报为合法六元组。

---

## 14. 主动端点审计

### 14.1 \(\vartheta=0\)

完整允许。此时低块零进位室只有 \(u=0\)；但 \(u=0\) 是低块自配对，
由 (2.11) 给 \(x\equiv0\pmod5\)，故不通过根门。其余合法低块均位于
\(\epsilon_u=1\) 室。

### 14.2 \(u=0\)

不能一般预删；它是否通过根门由 \(x\equiv2,3\pmod5\) 决定。通过时
\(\bar u=\vartheta\)，并按终端奇偶门继续筛选。\(\vartheta=0\) 的自配对
特例已由 14.1 删除。

### 14.3 \(u=\vartheta\) 与 \(\bar u=0\)

两者严格等价，属于 \(\epsilon_u=0\) 的闭端点。它可以通过根门，不能
统一删除。即使 \(\bar u=0\)，原 \(\lambda_\tau=CL\) 仍可为正。

### 14.4 \(u=\bar u\)

模 \(C\) 只有唯一解 \(u=u_*\)。它满足
\(x+Mu_*\equiv0\pmod C\)，故被根门删除。

### 14.5 \(T=0\)

完整保留，位于商零进位室，\(L=\Theta_u\)。

### 14.6 \(T=\Theta_u\) 与 \(L=0\)

两者严格等价，属于商零进位室闭端点。此时
\(\lambda_\tau=\bar u\)；只有再有 \(\bar u=0\) 才是原层
\(\lambda_\tau=0\)。不得把商层 \(L=0\) 自动误作原层零商。

### 14.7 两个低块进位与两个商进位室

(2.15a)–(2.15b) 和 (5.6a)–(5.6b) 分别双向穷尽。精确计数见
(7.4)、(7.9)。

### 14.8 商层固定点

每个 \(u\) 恰有一个 (6.4)。当 \(u\ne\bar u\) 时它仍属于非平凡原层
二循环；根门后的商固定计数见 (7.10)。

### 14.9 原层唯一固定点

它恰为 (3.6)，块坐标同时满足 \(u=\bar u\)、\(T=L\)，并由精确根门
删除。

### 14.10 \(s_C=0\)

由 \(\eta>0\) 与 (3.2) 严格不可能；实际有 \(s_C>0\)。

### 14.11 \(\Sigma_u=0\)

会强迫 \(g_u=\Theta_u=0\)，进而 \(\eta_u=0\)，与
\(\eta_u\ge s_C>0\) 矛盾。故严格不可能。

### 14.12 \(s_0=0\)

由原正整数式 (8.5) 严格不可能；准确结论是 \(0<s_0<q_0\)。

### 14.13 \(A_{u,T}\ge M\)

完整保留。本文使用原正整数 \(A_{u,T}\)，下端为
\(z_0=\lceil A_{u,T}/M\rceil\)，状态计数 (7.9) 允许任意大小室。

### 14.14 \(y=0\)

不能统一删除；精确条件是 (11.9)。该端点若通过指数门，则有 \(q<r\)。

### 14.15 最小 \(z=z_0\)

完整保留。是否产生指数由 \(2^\delta10^\mu\ge D_0\)、离散对数和严格
大小门共同决定。

### 14.16 \(\mathcal D_{u,T}=0\)

由 \(A_{u,T}r-N_0\ge r-N_0>0\) 严格不可能。

### 14.17 \(q=r\)

强迫原 involution 固定点，已由根门删除，故严格不可能。

### 14.18 \(q-r<0\)

不能预删；只可能发生在最小 \(z\) 端点。准确符号字典见 (11.7)–(11.9)。

### 14.19 边界 \(3\Delta=4\varphi\)

给无界射线 (1.8)。此时 \(\Omega=C\)、\(\Gamma=1\)，全文公式仍成立，
没有空室或除零。

### 14.20 \(\mu=0\)

完整包含在 (10.7)、(10.12)、(10.16) 与 (10.20) 中。若它命中同余类和
两个阈值，必须保留。

### 14.21 大小门严格端点

使用 (10.15) 中的 \(\mathscr X-1\) 保留严格不等式；(10.17) 同时核对
接受端和相邻拒绝端。\(z_{\max}\) 使用 \(\le\)，不误写为严格上界。

### 14.22 商反射退化的作用域

(5.4) 只直接适用于 \(3\Delta\le4\varphi\)。更深区域必须使用第 12 节
的多块递归；本文没有把第一深带的终端缺陷公式外推到更深带。

---

## 15. 为什么不能升级为关闭或绝对有限化

本轮没有得到 GALD1((-))-1，原因是：

1. 统一离散对数目标 (10.5) 在 Jacobi 层相容；移动模数 \(r\) 与
   \(\operatorname{ord}_r(10)\) 未被固定。
2. 正缺陷严格保证下降方向一致，却不产生统一模矛盾。
3. \(q-r\) 的 \((2,5)\)-赋值虽完全固定，其符号与奇素数部分仍随最小
   端点和 \(\mathscr L-V\) 移动。
4. 和差平方路线只是终端乘积恒等回代，没有新平方门。
5. 严格大小门只逐状态截断 \(\mu\)，不约束全体移动模数。
6. 边界 \((a,\Delta,\varphi)=(7t,4t,3t)\) 是无界射线，现有关系与之
   相容。

本轮没有得到 GALD1((-))-2，因为 \(a,\Delta,u,T,r\) 仍未绝对
有界；也没有得到 GALD1((-))-4，因为两个低块室、两个商进位室和
边界射线均未被统一关闭。

但本轮严格达到 GALD1((-))-3：

* 原 Möbius involution 完成两级双向块分解；
* 两级均显式反射化，逐位 Hensel 树消失；
* 第一次二进下降具有严格正缺陷；
* 每个固定 \((a,\Delta,h,J,u,T)\) 至多只剩一条完整有限指数同余段；
* 每个指数唯一恢复全部终端整数；
* 状态计数、固定点、零/一/双端奇偶、\(A\)-大小室、\(y=0\)、和差符号
  与精确赋值均已显式封闭；
* 任意更深负根 involution 获得严格的一般块递归。

由于没有得到绝对有限边界，本文不生成伪造的生成器、有限证书或哈希包，
也不以任何有限参数前缀外推。

---

## 16. 最终分类与停止点

本轮严格建立

\[
\boxed{
\begin{gathered}
\Lambda=C\Omega,
\qquad
\Omega\mid C,
\qquad
\Gamma=C/\Omega,\\
\tau=u+CT,
\qquad
\lambda_\tau=\bar u+CL,\\
u+\bar u=\vartheta+\epsilon_uC,
\qquad
T+L=\Theta_u+\epsilon_{u,T}\Omega,\\
H_u(T,L)=\eta_u+\alpha_uT+\beta_uL+\mathcal BTL,\\
\alpha_u\beta_u-\mathcal B\eta_u=1,
\qquad
\mathcal M_{\bar u}\mathcal M_u=I,\\
\Theta_u=\langle\eta_u\rangle_\Omega,
\qquad
L=\langle\Theta_u-T\rangle_\Omega,\\
s_0=\Sigma_u+\rho\epsilon_{u,T}+M\Gamma S_u(T,L),\\
q_0r=1+B\Lambda N_0,
\qquad
N_0=Jq_0+s_0,
\qquad
0<s_0<q_0,
\qquad
0<N_0<r,\\
A_{u,T}=J+\epsilon_{u,T}+\Sigma_u,
\qquad
y=Mz-A_{u,T},\\
\mathcal D_{u,T}=(A_{u,T}r-N_0)/M>0,\\
2^\delta10^\mu=zr-\mathcal D_{u,T},
\qquad
\gcd(\mathcal D_{u,T},r)=1,\\
2^{2a+h}10^{\mu+2a+\Delta}\equiv-1\pmod r,\\
\mu=\mu_0+t\operatorname{ord}_r(10),
\qquad
t_{\min}\le t\le t_{\max},\\
z=\dfrac{\mathcal D_{u,T}+2^\delta10^\mu}{r},\\
\mathscr L=\bar u+C\{L+\Omega(Mz-A_{u,T})\},\\
q-r=B(\mathscr L-V)\ne0,
\qquad
q+r=2\rho+B(\mathscr L+V),\\
v_2(q-r)=2a+1,
\quad v_5(q-r)=2\varphi,
\quad v_2(q+r)=1,
\quad v_5(q+r)=0.
\end{gathered}}
\tag{16.1}
\]

全部允许状态由两个模 \(5\) 低块类、两个低块进位室和每低块两个显式商
区间生成；固定 \(J\) 的零/一/双端循环数由 (7.14)–(7.17) 精确给出；
每个状态的指数由一条完整有限同余段穷尽。不存在逐位 Hensel 输出树或
多分支指数树。

但外层 \((a,\Delta)\)、低块 \(u\)、商块 \(T\)、移动模数 \(r\) 与阶
\(\operatorname{ord}_r(10)\) 仍无界；两个低块室、两个商进位室和边界
射线均未关闭。因此最终分类为

\[
\boxed{\mathrm{GALD1}((-))\text{-}3.}
\]

本文到此停止，不研究第一深带正根、\(3\Delta>4\varphi\) 的更深终端
系统、浅正负根、高 \(\varphi\) 的 \(\mathcal F_{P-}\)、B、C、
\(\gamma>1\)、非本原 C2/C5、Q 或严格层。
