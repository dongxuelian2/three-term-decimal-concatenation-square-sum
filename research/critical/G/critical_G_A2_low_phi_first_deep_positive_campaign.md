# 三项十进制拼接平方和问题：临界 G 模板 A2 低 \(\varphi\) 第一深带正根报告

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

中的第一深带正根区域

\[
\boxed{
\mathcal L_{\mathrm{d1},+}:
\quad
\sigma=+1,
\qquad
2\varphi<3(a-\varphi)\le4\varphi.
}
\tag{0.1}
\]

接受 PR6、SD6、GA2-6、GE2-1、GAL-2、GALS((+))-3、
GALS((-))-3 及 v3 总账中与本分支相容的冻结结论。第一深带负根、
\(3(a-\varphi)>4\varphi\) 的更深区域、浅正负根、高 \(\varphi\) 的
\(\mathcal F_{P-}\)、B、C、\(\gamma>1\)、非本原 C2/C5、Q 与严格层
均不在本文范围内。

本轮得到以下严格结论。

1. 模 \(\Lambda\) 的正根 Möbius involution 严格分解为一个模
   \(C\) 的补数低块和一个模 \(\Omega\) 的商 involution；
2. 第一深带中 \(\Omega\mid C\)，商 involution 严格退化为
   \(L=\langle\Theta_u-T\rangle_\Omega\) 的双室仿射反射；
3. 逐位 Hensel 树完全消失，全部允许状态组成交换低块的非平凡二循环；
4. 第一次二进下降产生有符号缺陷正规形
   \[
   2^\delta10^\mu=zr-\mathcal D_{u,T};
   \]
   缺陷为负当且仅当二进标准数字 \(a_{u,T}=0\)，其余状态缺陷为正；
5. 每个固定局部状态至多剩一条
   \(\operatorname{ord}_r(10)\)-同余类，并被严格大小门截成一条完整有限段；
6. 原商的共轭和差满足
   \[
   v_2(q-r)=2a+1,\quad v_5(q-r)=2\varphi,
   \quad v_2(q+r)=1,\quad v_5(q+r)=0,
   \]
   且 \(q=r\) 不可能；\(q<r\) 只可能发生在最小 \(z\) 端点；
7. 正根 Möbius 图还允许一个严格的一般块递归：第一块是补数，后续块是
   状态依赖的仿射反射，末块在剩余深度不超过 \(2\varphi\) 时反射化。

现有 Jacobi、和差、二进—五进赋值及大小门均未统一关闭任一商进位室，
也未给 \(a,\Delta\) 绝对界。因此准确分类为

\[
\boxed{
\mathrm{GALD1}((+))\text{-}3:
\quad
\text{完成低块—商反射分解、二进下降和每状态唯一有限指数段，}
\text{但仍有无界残余。}
}
\tag{0.2}
\]

没有找到合法原题六元组，也没有发现 GAL-2、GALS((+))-3、
GALS((-))-3、GE2-1、GA2-6、PR6 或 SD6 的继承错误。

---

## 1. 参数范围与第一深带整数化

定义

\[
\boxed{\Delta=a-\varphi\ge1.}
\tag{1.1}
\]

第一深带条件为

\[
2(a-\Delta)<3\Delta\le4(a-\Delta).
\]

因此它严格等价于

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

等价的 \(\varphi\) 写法是

\[
\boxed{
\left\lceil\frac{3a}{7}\right\rceil
\le\varphi\le
\left\lceil\frac{3a}{5}\right\rceil-1.
}
\tag{1.3}
\]

式 (1.2)–(1.3) 只使用整数上下取整；后文不以浮点数决定参数端点。
该区间从 \(a=4\) 开始才可能非空。

置

\[
\boxed{
M=2^{2a},\qquad
C=5^{2\varphi},\qquad
\Lambda=5^{3\Delta},\qquad
B=MC.
}
\tag{1.4}
\]

定义剩余深度

\[
\boxed{\chi=3\Delta-2\varphi>0,}
\qquad
\boxed{\Omega=5^\chi.}
\tag{1.5}
\]

由指数相加，严格有

\[
\boxed{\Lambda=C\Omega.}
\tag{1.6}
\]

第一深带上界 \(3\Delta\le4\varphi\) 等价于
\(\chi\le2\varphi\)，故

\[
\boxed{\Omega\mid C.}
\tag{1.7}
\]

定义

\[
\boxed{
\Gamma=\frac C\Omega=5^{4\varphi-3\Delta}\in\mathbb Z_{\ge1}.
}
\tag{1.8}
\]

边界 \(3\Delta=4\varphi\) 恰给

\[
\boxed{(a,\Delta,\varphi)=(7t,4t,3t),\quad
\Omega=C,\quad\Gamma=1,\qquad t\ge1.}
\tag{1.9}
\]

它是一条无界整数射线，完整包含在本文内。

尾窗仍为

\[
h\in\mathcal H(a),\qquad
e=2a+\Delta+h.
\tag{1.10}
\]

置

\[
\boxed{\delta=\Delta+h,\qquad e=2a+\delta.}
\tag{1.11}
\]

正根数据为

\[
\rho=1,\qquad\eta=0.
\tag{1.12}
\]

精确局部门为

\[
\boxed{\tau\equiv2\text{ 或 }3\pmod5,}
\tag{1.13}
\]

\[
\boxed{J+\tau\equiv1\pmod2,\qquad J\in\{1,\ldots,9\}.}
\tag{1.14}
\]

还需记录一个后文端点审计所用的纯大小事实。由
\(\varphi\ge3a/7\)，

\[
\chi=3a-5\varphi\le\frac{6a}{7}.
\]

而 \(5^6<4^7\)，所以

\[
\boxed{\Omega=5^\chi<4^a=M.}
\tag{1.15}
\]

---

## 2. 模 \(C\) 的低块—商双向分解

对每个标准代表

\[
0\le\tau<\Lambda=C\Omega
\]

唯一作欧几里得分解

\[
\boxed{\tau=u+CT,}
\tag{2.1}
\]

其中

\[
\boxed{0\le u<C,\qquad0\le T<\Omega.}
\tag{2.2}
\]

由根门 (1.13)，

\[
\boxed{u\equiv2\text{ 或 }3\pmod5,}
\tag{2.3}
\]

从而

\[
\boxed{0<u<C.}
\tag{2.4}
\]

GAL-2 的正根 involution 是

\[
\lambda_\tau
=
\left\langle
-\tau(1+B\tau)^{-1}
\right\rangle_\Lambda.
\tag{2.5}
\]

因为 \(C\mid B\)，模 \(C\) 有

\[
\lambda_\tau\equiv-\tau\equiv-u\pmod C.
\]

由 \(0<u<C\)，\(\lambda_\tau\) 的低块标准代表唯一为 \(C-u\)。
因此存在唯一 \(L\) 使

\[
\boxed{\lambda_\tau=C-u+CL,}
\tag{2.6}
\]

\[
\boxed{0\le L<\Omega.}
\tag{2.7}
\]

反向地，任取 (2.1)–(2.4) 并令 \(\lambda\) 具有 (2.6)–(2.7)
的形式，原 involution 图只剩下一条模 \(\Omega\) 条件；第 3 节将证明
它与原模 \(\Lambda\) 图严格等价。因此 (2.1)、(2.6) 是标准代表的双向
低块分解，不只是两个模 \(C\) 同余。

原 involution 的低块交换为

\[
\boxed{u\longleftrightarrow C-u.}
\tag{2.8}
\]

因 \(C\equiv0\pmod5\)，若 \(u\equiv2\pmod5\)，则
\(C-u\equiv3\pmod5\)，反之亦然。因此精确正根门在交换下保持。

---

## 3. 商 Möbius 图与互逆矩阵

原 involution 图等价于

\[
\tau+\lambda_\tau+B\tau\lambda_\tau\equiv0\pmod\Lambda.
\tag{3.1}
\]

把

\[
\tau=u+CT,
\qquad
\lambda_\tau=C-u+CL
\]

代入并逐项展开：

\[
\begin{aligned}
\tau+\lambda_\tau+B\tau\lambda_\tau
={}&C\{1+T+L\}\\
&+MC(u+CT)(C-u+CL)\\
={}&C\,H_u(T,L),
\end{aligned}
\tag{3.2}
\]

其中

\[
\boxed{
H_u(T,L)
=\eta_u+\alpha_uT+\beta_uL+\mathcal BTL,
}
\tag{3.3}
\]

\[
\boxed{\eta_u=1+Mu(C-u),}
\tag{3.4}
\]

\[
\boxed{\alpha_u=1+B(C-u),}
\tag{3.5}
\]

\[
\boxed{\beta_u=1+Bu,}
\tag{3.6}
\]

\[
\boxed{\mathcal B=BC=MC^2.}
\tag{3.7}
\]

由 \(\Lambda=C\Omega\)，(3.1) 与 (3.2) 严格等价于

\[
\boxed{H_u(T,L)\equiv0\pmod\Omega.}
\tag{3.8}
\]

因为

\[
\beta_u+\mathcal BT\equiv1\pmod5,
\]

它在模 \(\Omega\) 下是单位。因此每个 \(T\) 唯一决定

\[
\boxed{
L=f_u(T)
=
\left\langle
-(\eta_u+\alpha_uT)
(\beta_u+\mathcal BT)^{-1}
\right\rangle_\Omega.
}
\tag{3.9}
\]

定义矩阵

\[
\boxed{
\mathcal M_u=
\begin{pmatrix}
-\alpha_u&-\eta_u\\
\mathcal B&\beta_u
\end{pmatrix}.
}
\tag{3.10}
\]

低块交换时

\[
\alpha_{C-u}=\beta_u,
\qquad
\beta_{C-u}=\alpha_u,
\qquad
\eta_{C-u}=\eta_u.
\tag{3.11}
\]

并且

\[
\begin{aligned}
\alpha_u\beta_u-\mathcal B\eta_u
={}&\{1+MC(C-u)\}\{1+MCu\}\\
&-MC^2\{1+Mu(C-u)\}\\
=&1.
\end{aligned}
\]

故

\[
\boxed{\alpha_u\beta_u-\mathcal B\eta_u=1.}
\tag{3.12}
\]

逐项相乘立即得到整数矩阵恒等式

\[
\boxed{\mathcal M_{C-u}\mathcal M_u=I.}
\tag{3.13}
\]

全部分母均为五进单位，所以 (3.13) 在模 \(\Omega\) 的分式线性作用中
确实给出

\[
\boxed{f_{C-u}(f_u(T))=T\pmod\Omega.}
\tag{3.14}
\]

这就是原 involution 在两个低块纤维之间的精确商分解。

---

## 4. 第一深带中的商反射退化

由 \(\Omega\mid C\)，有

\[
B\equiv0\pmod\Omega,
\qquad
\mathcal B\equiv0\pmod\Omega.
\tag{4.1}
\]

所以

\[
\alpha_u\equiv\beta_u\equiv1\pmod\Omega,
\tag{4.2}
\]

而

\[
\eta_u=1+Mu(C-u)\equiv1-Mu^2\pmod\Omega.
\tag{4.3}
\]

定义标准平移数字

\[
\boxed{
\Theta_u=
\left\langle Mu^2-1\right\rangle_\Omega
\in\{0,\ldots,\Omega-1\}.
}
\tag{4.4}
\]

式 (3.9) 严格退化为

\[
\boxed{L=\left\langle\Theta_u-T\right\rangle_\Omega.}
\tag{4.5}
\]

由于 \(C\equiv0\pmod\Omega\)，

\[
M(C-u)^2-1\equiv Mu^2-1\pmod\Omega,
\]

故

\[
\boxed{\Theta_{C-u}=\Theta_u.}
\tag{4.6}
\]

定义唯一进位位

\[
\boxed{\epsilon_{u,T}\in\{0,1\}}
\tag{4.7}
\]

使

\[
\boxed{T+L=\Theta_u+\epsilon_{u,T}\Omega.}
\tag{4.8}
\]

两个互斥反射室为

\[
\boxed{
0\le T\le\Theta_u
\Longrightarrow
L=\Theta_u-T,
\quad\epsilon_{u,T}=0,
}
\tag{4.9a}
\]

\[
\boxed{
\Theta_u<T<\Omega
\Longrightarrow
L=\Theta_u+\Omega-T,
\quad\epsilon_{u,T}=1.
}
\tag{4.9b}
\]

式 (4.5)、(4.9a)–(4.9b) 对每个 \((u,T)\) 唯一给出
\((L,\epsilon_{u,T})\)。因此本区域不再需要逐五进数字 Hensel 提升。

定义

\[
\boxed{
g_u=
\frac{Mu^2-1-\Theta_u}{\Omega}\in\mathbb Z_{\ge0}.
}
\tag{4.10}
\]

事实上本区域有更强端点事实。由 \(u\ge2\) 与 (1.15)，

\[
Mu^2-1\ge4M-1>4\Omega,
\]

所以

\[
\boxed{g_u\ge4.}
\tag{4.11}
\]

因此题设要求审计的 \(g_u=0\) 在第一深带严格不可能；这一删除来自
\(\Omega<M\)，不是有限样本。

---

## 5. 原层二循环、奇偶门与精确状态计数

原 involution 在块坐标中为

\[
\boxed{(u,T)\longmapsto(C-u,L).}
\tag{5.1}
\]

若它是原模 \(\Lambda\) 固定点，则低块必须满足

\[
u=C-u.
\]

即 \(2u=C\)。但 \(C\) 为奇数且 \(u\in\mathbb Z\)，不可能发生。
等价地，模 \(C\) 的固定点条件是 \(2u\equiv0\pmod C\)，它只允许
\(u=0\)，而根门已给 \(u\equiv2,3\pmod5\)。所以即使商反射出现
\(T=L\)，也不是原 involution 固定点。准确结论是

\[
\boxed{
\text{全部允许状态组成交换低块的非平凡二循环；原层没有固定点。}
}
\tag{5.2}
\]

### 5.1 二循环中的奇偶判别

因 \(C\) 为奇数，

\[
\tau\equiv u+T\pmod2,
\qquad
\lambda_\tau\equiv1-u+L\pmod2.
\]

由 (4.8) 且 \(\Omega\) 为奇数，

\[
\boxed{
\tau+\lambda_\tau
\equiv1+\Theta_u+\epsilon_{u,T}\pmod2.
}
\tag{5.3}
\]

于是：

* 若 \(\Theta_u+\epsilon_{u,T}\) 为偶数，则
  \(\tau+\lambda_\tau\) 为奇数，二循环两端奇偶相反，固定 \(J\)
  的门 \(J+\tau\equiv1\pmod2\) 恰保留一个端点；
* 若 \(\Theta_u+\epsilon_{u,T}\) 为奇数，则两端奇偶相同，奇偶门同时
  保留两个端点或同时删除两个端点。

因此不能声称每个二循环自动留下一个端点。

### 5.2 不遍历 \(\Lambda\) 个 \(\tau\) 的计数公式

定义

\[
\mathcal U=
\{u:1\le u<C,\ u\equiv2,3\pmod5\},
\tag{5.4}
\]

\[
\mathcal U_2=
\{u:1\le u<C,\ u\equiv2\pmod5\}.
\tag{5.5}
\]

则

\[
\boxed{|\mathcal U|=\frac{2C}{5},\qquad
|\mathcal U_2|=\frac C5.}
\tag{5.6}
\]

每个低块对 \(\{u,C-u\}\) 在 \(\mathcal U_2\) 中有唯一代表，所以低块对
恰有

\[
\boxed{\frac C5}
\tag{5.7}
\]

个；根门后的原二循环总数为

\[
\boxed{\frac{C\Omega}{5}=\frac\Lambda5.}
\tag{5.8}
\]

为计数奇偶门，定义

\[
\Pi_p(X)=
\#\{t:0\le t\le X,\ t\equiv p\pmod2\},
\qquad p\in\{0,1\},
\tag{5.9}
\]

即

\[
\Pi_p(X)=
\begin{cases}
0,&X<p,\\[1mm]
\left\lfloor\dfrac{X-p}{2}\right\rfloor+1,&X\ge p.
\end{cases}
\tag{5.10}
\]

对固定 \((u,J)\)，置

\[
p_{u,J}=\langle1-J-u\rangle_2.
\tag{5.11}
\]

两个商进位室中通过终端奇偶门的有向状态数分别为

\[
\boxed{
\mathcal N_{J,0}
=\sum_{u\in\mathcal U}
\Pi_{p_{u,J}}(\Theta_u),
}
\tag{5.12}
\]

\[
\boxed{
\mathcal N_{J,1}
=\sum_{u\in\mathcal U}
\left\{
\Pi_{p_{u,J}}(\Omega-1)
-\Pi_{p_{u,J}}(\Theta_u)
\right\}.
}
\tag{5.13}
\]

在 \(\mathcal U\) 中偶、奇 \(u\) 各有 \(C/5\) 个；而长度为奇数的
区间 \([0,\Omega-1]\) 中偶数有 \((\Omega+1)/2\) 个、奇数有
\((\Omega-1)/2\) 个。因此

\[
\boxed{
\mathcal N_{J,0}+\mathcal N_{J,1}=\frac{C\Omega}{5}=\frac\Lambda5.
}
\tag{5.14}
\]

这给出固定 \(J\) 的精确有向状态总数；九个 \(J\) 共给
\(9\Lambda/5\) 个进入指数门之前的有向状态。

还可精确区分二循环保留零、一、二端。对 \(u\in\mathcal U_2\) 置

\[
\begin{aligned}
n_1(u)={}&
\mathbf1_{\Theta_u\equiv0\ (2)}(\Theta_u+1)\\
&+\mathbf1_{\Theta_u\equiv1\ (2)}(\Omega-1-\Theta_u),
\end{aligned}
\tag{5.15}
\]

这是恰保留一端的循环数。相同奇偶的循环中，恰保留两端的数为

\[
\begin{aligned}
n_2(u,J)={}&
\mathbf1_{\Theta_u\equiv1\ (2)}
\Pi_{p_{u,J}}(\Theta_u)\\
&+\mathbf1_{\Theta_u\equiv0\ (2)}
\left\{
\Pi_{p_{u,J}}(\Omega-1)-\Pi_{p_{u,J}}(\Theta_u)
\right\}.
\end{aligned}
\tag{5.16}
\]

故

\[
\boxed{
N_1(J)=\sum_{u\in\mathcal U_2}n_1(u),
\qquad
N_2(J)=\sum_{u\in\mathcal U_2}n_2(u,J),
}
\tag{5.17}
\]

\[
\boxed{
N_0(J)=\frac\Lambda5-N_1(J)-N_2(J).
}
\tag{5.18}
\]

这里 \(N_i(J)\) 是奇偶门保留 \(i\) 个端点的二循环数。由 (5.14)，

\[
N_1(J)+2N_2(J)=\frac\Lambda5=N_0(J)+N_1(J)+N_2(J),
\]

所以还自动有

\[
\boxed{N_0(J)=N_2(J).}
\tag{5.19}
\]

式 (5.12)–(5.19) 只对 \(2C/5\) 个低块作闭式区间计数，不遍历
\(C\Omega=\Lambda\) 个 \(\tau\)。它们没有把“参数化”误报成叶节点数绝对
有界。

---

## 6. 商层闭式与基础终端恒等式

定义

\[
\boxed{
S_u(T,L)=u+(C-u)T+uL+CTL.
}
\tag{6.1}
\]

由 (3.3) 与 (4.8)，

\[
\begin{aligned}
H_u(T,L)
={}&1+Mu(C-u)+T+L\\
&+MC\{(C-u)T+uL+CTL\}.
\end{aligned}
\]

又由

\[
Mu^2-1=\Theta_u+g_u\Omega
\]

以及 \(C=\Gamma\Omega\)，有

\[
1+Mu(C-u)+\Theta_u=MCu-g_u\Omega.
\]

因此

\[
\boxed{
H_u(T,L)
=\Omega\left\{
\epsilon_{u,T}-g_u+M\Gamma S_u(T,L)
\right\}.
}
\tag{6.2}
\]

GAL-2 的基础余数是 \(s_0=H_u/\Omega\)，故

\[
\boxed{
s_0=epsilon_{u,T}-g_u+M\Gamma S_u(T,L).
}
\tag{6.3}
\]

尽管 \(\epsilon_{u,T}-g_u<0\) 可以发生，原正整数表达式为

\[
s_0=
\frac{\tau+\lambda_\tau+B\tau\lambda_\tau}{\Lambda}.
\tag{6.4}
\]

这里 \(\tau>0\)、\(\lambda_\tau>0\)、\(B>0\)，且分子按 involution
图被 \(\Lambda\) 整除。因此

\[
\boxed{s_0>0.}
\tag{6.5}
\]

定义

\[
\boxed{
V=J\Lambda+\tau
=JC\Omega+u+CT,
}
\tag{6.6}
\]

\[
\boxed{r=1+BV,}
\tag{6.7}
\]

\[
\boxed{
q_0=1+B\lambda_\tau
=1+B(C-u+CL),
}
\tag{6.8}
\]

\[
\boxed{N_0=Jq_0+s_0.}
\tag{6.9}
\]

由 GAL-2 的双向终端公式，或直接展开 (6.7)–(6.9)，得到

\[
\boxed{q_0r=1+B\Lambda N_0.}
\tag{6.10}
\]

式 (6.9) 已给 \(N_0=Jq_0+s_0\)。还需独立核对上余数端点。
置 \(R_\tau=1+B\tau\)。由 (6.4)，

\[
q_0R_\tau=1+B\Lambda s_0.
\]

而 \(0<\tau<\Lambda\) 给

\[
0<R_\tau<B\Lambda.
\]

故 \(q_0R_\tau<q_0B\Lambda\)，从而

\[
\boxed{0<s_0<q_0.}
\tag{6.11}
\]

完整仿射恢复为

\[
\boxed{q=q_0+B\Lambda y,}
\tag{6.12}
\]

\[
\boxed{s=s_0+(1+B\tau)y,}
\tag{6.13}
\]

\[
\boxed{N=N_0+ry,}
\tag{6.14}
\]

其中

\[
\boxed{y\in\mathbb Z_{\ge0}.}
\tag{6.15}
\]

式 (6.10)、(6.12)–(6.14) 与

\[
qr=1+B\Lambda N,
\qquad
N=Jq+s
\]

严格双向。

---

## 7. 第一次二进下降与缺陷符号

真实指数写为

\[
\boxed{N=2^e10^\mu,\qquad \mu\ge0.}
\tag{7.1}
\]

由 \(e=2a+\delta\)，

\[
\boxed{M\mid N.}
\tag{7.2}
\]

式 (6.3) 给

\[
s_0\equiv\epsilon_{u,T}-g_u\pmod M.
\]

而 \(q_0\equiv r\equiv1\pmod M\)，所以

\[
\boxed{
N_0\equiv J+\epsilon_{u,T}-g_u\pmod M.
}
\tag{7.3}
\]

定义标准二进数字

\[
\boxed{
A_{u,T}:=a_{u,T}
=\left\langle J+\epsilon_{u,T}-g_u\right\rangle_M
\in\{0,\ldots,M-1\}.
}
\tag{7.4}
\]

由 \(N=N_0+ry\equiv0\pmod M\) 与 \(r\equiv1\pmod M\)，

\[
\boxed{y\equiv-A_{u,T}\pmod M.}
\tag{7.5}
\]

因此唯一写成

\[
\boxed{y=Mz-A_{u,T},}
\tag{7.6}
\]

其中

\[
\boxed{
z\in\mathbb Z_{\ge0},\qquad
z\ge z_{\min}^{(0)}:=
\begin{cases}
0,&A_{u,T}=0,\\
1,&A_{u,T}>0.
\end{cases}
}
\tag{7.7}
\]

这里没有先验删除 \(A_{u,T}=0\)、\(y=0\) 或 \(z=0\)。

定义整数

\[
\boxed{
b_{u,T}
=\frac{A_{u,T}-J-\epsilon_{u,T}+g_u}{M}
\in\mathbb Z.
}
\tag{7.8}
\]

再定义有符号缺陷

\[
\boxed{
\mathcal D_{u,T}
=\frac{A_{u,T}r-N_0}{M}.
}
\tag{7.9}
\]

把 (6.1)、(6.3)、(6.6)–(6.9) 代入，得到题设要求的显式整数闭式

\[
\boxed{
\begin{aligned}
\mathcal D_{u,T}
={}&b_{u,T}-\Gamma S_u(T,L)\\
&+C\Bigl[
A_{u,T}\{JC\Omega+u+CT\}
-J\{C-u+CL\}
\Bigr].
\end{aligned}
}
\tag{7.10}
\]

式 (7.10) 只含
\(u,T,L,\Theta_u,\epsilon_{u,T},g_u,J\) 及由外层参数确定的
\(M,C,\Omega,\Gamma\)。

### 7.1 缺陷的完整符号字典

由 (6.8) 与 \(0<\lambda_\tau<\Lambda\)，

\[
0<q_0<B\Lambda.
\]

结合 (6.10)，

\[
1+B\Lambda N_0=q_0r<B\Lambda r,
\]

故

\[
\boxed{0<N_0<r.}
\tag{7.11}
\]

于是 (7.9) 立即给出精确符号：

\[
\boxed{
\mathcal D_{u,T}<0
\Longleftrightarrow
A_{u,T}=0,
}
\tag{7.12}
\]

\[
\boxed{
\mathcal D_{u,T}>0
\Longleftrightarrow
A_{u,T}>0.
}
\tag{7.13}
\]

特别地

\[
\boxed{\mathcal D_{u,T}\ne0.}
\tag{7.14}
\]

这比仅由互素性推出非零更强。负缺陷不能统一删除；它恰对应必须保留的
\(A_{u,T}=0\) 端点。

将 (7.6) 代入 (6.14)：

\[
N=N_0+r(Mz-A_{u,T})
=M\{zr-\mathcal D_{u,T}\}.
\]

再用 \(N/M=2^\delta10^\mu\)，得到核心正规形

\[
\boxed{
2^\delta10^\mu
=zr-\mathcal D_{u,T}.
}
\tag{7.15}
\]

反向地，固定一个局部状态，任取满足 (7.7)、\(\mu\ge0\) 和 (7.15)
的整数 \((z,\mu)\)，以 (7.6) 定义 \(y\)。则 \(y\ge0\)，且

\[
N_0+ry=M2^\delta10^\mu=2^e10^\mu.
\]

再由 (6.12)–(6.14) 唯一恢复 \(q,s,N\)，全部终端恒等式和
\(0<s<q\) 自动成立。因此 (7.15) 与原仿射终端状态严格双向。

### 7.2 \(A_{u,T}=0\) 的精确计数入口

由

\[
g_u\Omega+\Theta_u=Mu^2-1,
\]

模 \(M\) 有

\[
g_u\equiv-(\Theta_u+1)\Omega^{-1}\pmod M.
\tag{7.16}
\]

故

\[
A_{u,T}=0
\Longleftrightarrow
J+\epsilon_{u,T}
+(\Theta_u+1)\Omega^{-1}
\equiv0\pmod M.
\tag{7.17}
\]

固定 \(J\) 后，通过根门和奇偶门的 \(A_{u,T}=0\) 有向端点数恰为

\[
\boxed{
\begin{aligned}
\mathcal Z_J
=\sum_{u\in\mathcal U}\Bigl[&
\mathbf1_{J-g_u\equiv0\ (M)}
\Pi_{p_{u,J}}(\Theta_u)\\
&+\mathbf1_{J+1-g_u\equiv0\ (M)}
\{\Pi_{p_{u,J}}(\Omega-1)-\Pi_{p_{u,J}}(\Theta_u)\}
\Bigr].
\end{aligned}
}
\tag{7.18}
\]

这也是负缺陷局部状态的精确数目。式 (7.18) 不遍历 \(\Lambda\) 个
\(\tau\)，且没有用小参数未观察到该端点来删除它。

由 (7.6)–(7.7)，还有

\[
\boxed{
y=0
\Longleftrightarrow
z=0
\Longleftrightarrow
A_{u,T}=0\text{ 且 }z=z_{\min}^{(0)}.
}
\tag{7.19}
\]

这些等价只描述仿射端点；它是否满足指数等式仍由第 8 节决定。

---

## 8. 缺陷互素性与唯一完整有限指数段

由 (7.9)，

\[
M\mathcal D_{u,T}=A_{u,T}r-N_0.
\tag{8.1}
\]

GAL-2 已证明

\[
\gcd(N_0,r)=1,
\qquad
\gcd(M,r)=1.
\]

若某素数同时整除 \(\mathcal D_{u,T}\) 与 \(r\)，则由 (8.1) 也整除
\(N_0\)，矛盾。因此

\[
\boxed{\gcd(\mathcal D_{u,T},r)=1.}
\tag{8.2}
\]

这里 gcd 对负缺陷取绝对值。式 (8.2) 再次独立证明
\(\mathcal D_{u,T}\ne0\)。

核心方程 (7.15) 模 \(r\) 给

\[
\boxed{
10^\mu
\equiv
-2^{-\delta}\mathcal D_{u,T}
\pmod r.
}
\tag{8.3}
\]

### 8.1 离散对数目标的统一塌缩

由 (6.10)，

\[
B\Lambda N_0\equiv-1\pmod r.
\]

而 (8.1) 给

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
\tag{8.4}
\]

因为

\[
M^2C^2\Omega
=2^{4a}5^{2\varphi+3\Delta}
=2^{4a}5^{2a+\Delta},
\]

(8.3) 等价于

\[
\boxed{
10^\mu
\equiv
-2^{-(4a+\delta)}5^{-(2a+\Delta)}
\pmod r,
}
\tag{8.5}
\]

或

\[
\boxed{
2^{2a+h}10^{\mu+2a+\Delta}
\equiv-1\pmod r.
}
\tag{8.6}
\]

除移动模数 \(r\) 外，离散对数目标不再显含 \(u,T,J\)。但
\(r\equiv1\pmod M\) 且 \(r\equiv1\pmod C\)，所以

\[
r\equiv1\pmod{40}.
\]

因而对正奇复合数的广义 Jacobi 符号，

\[
\left(\frac{-1}{r}\right)
=\left(\frac2r\right)
=\left(\frac5r\right)=1.
\]

式 (8.6) 在 Jacobi 层完全相容，没有形成统一矛盾。

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

该整个局部状态为空。若属于，则存在唯一

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
\frac{\mathcal D_{u,T}+2^\delta10^\mu}{r}.
}
\tag{8.9}
\]

### 8.3 同时处理正、负缺陷的严格下端

定义

\[
\boxed{
D_0=z_{\min}^{(0)}r-\mathcal D_{u,T}.
}
\tag{8.10}
\]

若 \(A_{u,T}=0\)，则 \(z_{\min}^{(0)}=0\) 且

\[
D_0=-\mathcal D_{u,T}=\frac{N_0}{M}>0.
\]

若 \(A_{u,T}>0\)，则 \(z_{\min}^{(0)}=1\)，并由 (7.9)

\[
D_0=r-\mathcal D_{u,T}
=\frac{(M-A_{u,T})r+N_0}{M}>0.
\]

因此统一有

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
=\min\{v\in\mathbb Z_{\ge0}:2^\delta10^v\ge D_0\}.
}
\tag{8.12}
\]

这同时正确处理 \(\mathcal D_{u,T}<0\)；没有把负缺陷错误地置为零下端。

### 8.4 严格大小门与上端

继承判别式大小门为

\[
20\cdot10^m<194029\,\mathfrak Z^2Y,
\tag{8.13}
\]

其中为避免与下降变量 \(z\) 混淆，记

\[
\mathfrak Z=\frac{B\Lambda}{2},
\qquad
Y=10^{3a},
\qquad
m=e+\mu.
\tag{8.14}
\]

置

\[
\mathscr X=194029\,\mathfrak Z^2Y,
\tag{8.15}
\]

\[
\boxed{
Q_\mu=
\left\lfloor
\frac{\mathscr X-1}{20\cdot10^e}
\right\rfloor.
}
\tag{8.16}
\]

若 \(Q_\mu<1\)，该状态整体为空。否则定义

\[
\boxed{
\mu_{\max}
=\max\{v\in\mathbb Z_{\ge0}:10^v\le Q_\mu\}.
}
\tag{8.17}
\]

则

\[
\boxed{
20\cdot10^{e+\mu_{\max}}
<\mathscr X
\le20\cdot10^{e+\mu_{\max}+1}.
}
\tag{8.18}
\]

式 (8.16) 使用 \(\mathscr X-1\)，完整保留严格不等式的相邻端点。

### 8.5 完整有限指数段

若离散对数存在，定义

\[
t_{\min}
=\max\left(
0,
\left\lceil\frac{\mu_{\min}-\mu_0}{P_r}\right\rceil
\right),
\tag{8.19}
\]

\[
t_{\max}
=\left\lfloor
\frac{\mu_{\max}-\mu_0}{P_r}
\right\rfloor.
\tag{8.20}
\]

若 \(t_{\min}>t_{\max}\)，该状态为空；否则全部指数恰为

\[
\boxed{
\mu=\mu_0+tP_r,
\qquad
t_{\min}\le t\le t_{\max}.
}
\tag{8.21}
\]

每个指数由 (8.9)、(7.6)、(6.12)–(6.14) 唯一恢复
\(z,y,q,s,N\)。这是完整有限同余段，不是有限采样 \(\mu\)。

准确的整数 \(z\) 上端为

\[
\boxed{
z\le
z_{\max}:=
\left\lfloor
\frac{\mathcal D_{u,T}+2^\delta10^{\mu_{\max}}}{r}
\right\rfloor.
}
\tag{8.22}
\]

若最大指数恰整除，等号可以发生；不能把 (8.22) 改成严格上界。

---

## 9. 原商、共轭和差与精确赋值

为避免与商层变量 \(L\) 混淆，记 GAL-2 的原商参数为

\[
\boxed{\mathscr L=\lambda_\tau+\Lambda y.}
\tag{9.1}
\]

代入 \(\lambda_\tau=C-u+CL\)、\(\Lambda=C\Omega\) 和
\(y=Mz-A_{u,T}\)，得到最短闭式

\[
\boxed{
\mathscr L
=C\{M\Omega z+1+L-\Omega A_{u,T}\}-u.
}
\tag{9.2}
\]

同时

\[
\boxed{V=u+C(T+J\Omega).}
\tag{9.3}
\]

于是

\[
\boxed{q=1+B\mathscr L,\qquad r=1+BV.}
\tag{9.4}
\]

定义

\[
\boxed{
W_+=1+\Theta_u
+\Omega\{Mz+J+\epsilon_{u,T}-A_{u,T}\},
}
\tag{9.5}
\]

\[
\boxed{
W_-=1+L-T
+\Omega\{Mz-A_{u,T}-J\}.
}
\tag{9.6}
\]

由 \(T+L=\Theta_u+\epsilon_{u,T}\Omega\)，逐项得到

\[
\boxed{\mathscr L+V=CW_+,}
\tag{9.7}
\]

\[
\boxed{\mathscr L-V=CW_--2u.}
\tag{9.8}
\]

因此

\[
\boxed{q+r=2+BCW_+,}
\tag{9.9}
\]

\[
\boxed{q-r=B(CW_--2u).}
\tag{9.10}
\]

### 9.1 \(q=r\) 与符号

若 \(q=r\)，则 \(\mathscr L=V\)。模 \(\Lambda\) 得
\(\lambda_\tau=\tau\)，这会使原 involution 出现固定点，与第 5 节
矛盾。因此

\[
\boxed{q=r\text{ 不可能}.}
\tag{9.11}
\]

更精确地，由

\[
\mathscr L-V=\lambda_\tau-\tau+\Lambda(y-J),
\]

有

\[
\boxed{
\begin{array}{c|c}
y\le J-1&q<r\\
y\ge J+1&q>r\\
y=J&\operatorname{sgn}(q-r)=\operatorname{sgn}(\lambda_\tau-\tau)
\end{array}}
\tag{9.12}
\]

若 \(z\ge z_{\min}^{(0)}+1\)，则：

* \(A_{u,T}=0\) 时 \(y=Mz\ge M>J\)；
* \(A_{u,T}>0\) 时 \(y=Mz-A_{u,T}\ge M+1>J\)。

所以

\[
\boxed{q<r\text{ 只可能发生在最小 }z=z_{\min}^{(0)}.}
\tag{9.13}
\]

当 \(A_{u,T}=0,z=0\) 时，\(y=0<J\)，故该端点若满足指数门，必有
\(q<r\)。它不能仅因符号为负而删除。

### 9.2 和差的精确二进、五进赋值

由 (9.9)，\(BCW_+\) 被 \(M\) 和 \(5\) 整除，故

\[
\boxed{v_2(q+r)=1,\qquad v_5(q+r)=0.}
\tag{9.14}
\]

对差，先有

\[
CW_--2u\equiv-2u\not\equiv0\pmod5,
\]

所以

\[
\boxed{v_5(q-r)=2\varphi.}
\tag{9.15}
\]

二进处需要保留终端奇偶门，不能只写下界。因为
\(C\equiv\Omega\equiv1\pmod4\)、\(M\equiv0\pmod4\)，由
\(A_{u,T}\equiv J+\epsilon_{u,T}-g_u\pmod4\) 得

\[
W_-
\equiv1+\Theta_u+g_u-2(T+J)\pmod4.
\]

而

\[
\Theta_u+g_u\Omega=Mu^2-1
\]

给 \(\Theta_u+g_u\equiv-1\pmod4\)。再用
\(J+u+T\equiv1\pmod2\)，得到

\[
CW_--2u\equiv2\pmod4.
\]

故

\[
\boxed{v_2(CW_--2u)=1,}
\tag{9.16}
\]

最终

\[
\boxed{v_2(q-r)=2a+1.}
\tag{9.17}
\]

式 (9.14)–(9.17) 是精确赋值，不是下界。

这些赋值与 \((q-r)^2=(q+r)^2-4qr\) 完全相容；把 (9.9)–(9.10)
代回只得到已有终端方程的恒等式。奇素数 gcd 仍可随
\(CW_--2u\) 移动。因此本轮没有出现类似浅正根或浅负根之外的新固定
因子门。

---

## 10. 一般正根块递归及其能力边界

第一深带的反射退化依赖

\[
\Omega\mid C
\iff
3\Delta\le4\varphi.
\]

当

\[
3\Delta>4\varphi
\]

时，第一商层模数 \(\Omega\) 不再整除 \(C\)，式 (4.1)–(4.5)
不能直接用于整个商层；第一商映射仍是 (3.9) 的非平凡 Möbius 变换。

不过正根图本身存在一个可严格归纳的一般块递归。以下定理只处理正根
involution，不把本文的缺陷符号、指数段或无解结论外推到更深带。

### 10.1 通用一步块引理

设某层图为

\[
G_j(X,Y)
=\eta_j+\alpha_jX+\beta_jY+\gamma_jXY
\equiv0\pmod{5^{n_j}},
\tag{10.1}
\]

并满足

\[
\boxed{
\alpha_j\beta_j-\gamma_j\eta_j=1,
\quad
\alpha_j\equiv\beta_j\equiv1\pmod C,
\quad
C\mid\gamma_j.
}
\tag{10.2}
\]

若 \(n_j>2\varphi\)，写

\[
X=v+CX',\qquad Y=w+CY',
\tag{10.3}
\]

其中

\[
\boxed{
w=\left\langle-\eta_j-v\right\rangle_C.
}
\tag{10.4}
\]

定义

\[
\boxed{
\eta_{j+1}
=\frac{\eta_j+\alpha_jv+\beta_jw+\gamma_jvw}{C},
}
\tag{10.5}
\]

\[
\boxed{
\alpha_{j+1}=\alpha_j+\gamma_jw,
\qquad
\beta_{j+1}=\beta_j+\gamma_jv,
\qquad
\gamma_{j+1}=C\gamma_j.
}
\tag{10.6}
\]

式 (10.4) 保证 (10.5) 为整数。直接展开得到

\[
\frac{G_j(v+CX',w+CY')}{C}
=\eta_{j+1}+\alpha_{j+1}X'
+\beta_{j+1}Y'+\gamma_{j+1}X'Y'.
\tag{10.7}
\]

而

\[
\begin{aligned}
&\alpha_{j+1}\beta_{j+1}
-\gamma_{j+1}\eta_{j+1}\\
={}&(\alpha_j+\gamma_jw)(\beta_j+\gamma_jv)\\
&-\gamma_j(\eta_j+\alpha_jv+\beta_jw+\gamma_jvw)\\
=&\alpha_j\beta_j-\gamma_j\eta_j=1.
\end{aligned}
\tag{10.8}
\]

并且 (10.6) 保持

\[
\alpha_{j+1}\equiv\beta_{j+1}\equiv1\pmod C,
\qquad C\mid\gamma_{j+1}.
\tag{10.9}
\]

因此每次剥去一个指数宽度 \(2\varphi\) 的 \(C\)-块，剩余深度恰减少
\(2\varphi\)，且行列式恒等式保持。

反向图把 \((\alpha_j,\beta_j)\) 交换，并把低块 \((v,w)\) 交换；
由 (10.5)–(10.6)，下一层仍只交换
\((\alpha_{j+1},\beta_{j+1})\)。对应矩阵

\[
\begin{pmatrix}
-\alpha_j&-\eta_j\\
\gamma_j&\beta_j
\end{pmatrix},
\qquad
\begin{pmatrix}
-\beta_j&-\eta_j\\
\gamma_j&\alpha_j
\end{pmatrix}
\]

的乘积为 \(I\)。故每层的正向、反向商矩阵严格互逆。

### 10.2 一般 \(q\)-块正规形

把总深度唯一写成

\[
\boxed{
3\Delta=q(2\varphi)+r_0,
\qquad
q\in\mathbb Z_{\ge0},
\qquad
0<r_0\le2\varphi.
}
\tag{10.10}
\]

若 \(2\varphi\mid3\Delta\)，这里取
\(q=3\Delta/(2\varphi)-1\)、\(r_0=2\varphi\)，从而保持
\(r_0>0\)。

初始图为

\[
(\eta_0,\alpha_0,\beta_0,\gamma_0)=(0,1,1,B).
\tag{10.11}
\]

连续应用 (10.3)–(10.9) 共 \(q\) 次：

* 第一低块满足 \(w_0=\langle-v_0\rangle_C\)，在合法非零块上即
  \(v_0\leftrightarrow C-v_0\)；
* 第 \(j\ge1\) 块满足
  \[
  w_j=\langle\Theta_j-v_j\rangle_C,
  \qquad
  \Theta_j=\langle-\eta_j\rangle_C;
  \]
* 每个输入块唯一决定输出块，没有逐位 Hensel 分支；
* 最后剩余模数 \(5^{r_0}\mid C\)，故末层再次退化为
  \[
  Y_q=\langle-\eta_q-X_q\rangle_{5^{r_0}}.
  \]

这给出任意深度正根 involution 的严格块递归正规形。

必须注意：只有第一块是朴素补数 \(u\leftrightarrow C-u\)。第二块起的
低块配对一般是带状态平移 \(\Theta_j\) 的仿射反射，而不是再次
\(v\leftrightarrow C-v\)。因此“每层都重复同一个补数映射”的更强说法
是错误的；本文没有作该外推。

本一般递归只消除了正根 involution 的 Hensel 输出树。它没有证明更深带的
终端缺陷具有本文同一符号字典，也没有关闭第一深带以外的任何区域。

---

## 11. 完整生成顺序与终端充分性边界

第一深带的全部终端候选必须、且在终端层面只须按以下顺序生成。

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
3. 构造 \(M,C,\Lambda,\Omega,\Gamma,B\)。
4. 取 \(J\in\{1,\ldots,9\}\) 及
   \[
   u\in\mathcal U,
   \qquad
   0\le T<\Omega,
   \qquad
   J+u+T\equiv1\pmod2.
   \]
5. 唯一计算
   \[
   \Theta_u=\langle Mu^2-1\rangle_\Omega,
   \quad
   L=\langle\Theta_u-T\rangle_\Omega,
   \quad
   \epsilon_{u,T}=(T+L-\Theta_u)/\Omega,
   \quad
   g_u=(Mu^2-1-\Theta_u)/\Omega.
   \]
6. 构造第 6、7 节的 \(s_0,q_0,N_0,r,A_{u,T},\mathcal D_{u,T}\)。
7. 检查 (8.3) 或统一式 (8.6)。若离散对数不存在，删除整个状态；若
   存在，按 (8.21) 生成唯一完整有限指数段。
8. 对每个指数用 (8.9)、(7.6)、(9.2)、(6.12)–(6.14) 唯一恢复
   \(z,y,\mathscr L,q,s,N\)。
9. 最后进入继承的十三首块、\(a_2\) 窗口、判别式平方、两个恢复符号、
   精确 gcd 尺度、\(a_3\) 窗口、三个逐项既约条件和原题直接回代。

第 1–8 步在终端层严格双向；第 9 步仍是原题完整候选不可省略的恢复门。
本文没有把终端状态误报为合法六元组。

---

## 12. 主动端点审计

### 12.1 \(u=0\)

根门要求 \(u\equiv2,3\pmod5\)，故严格删除。

### 12.2 \(u=C-u\)

它要求 \(2u=C\)，与 \(C\) 为奇数矛盾。

### 12.3 \(T=0\)

完整保留。此时按 \(0\le T\le\Theta_u\) 位于零进位室，
\(L=\Theta_u\)。

### 12.4 \(T=\Theta_u\) 与 \(L=0\)

两者严格等价，属于零进位室闭端点。原低块仍为 \(C-u>0\)，所以
\(\lambda_\tau=C-u>0\)；不能把商层 \(L=0\) 误作原层
\(\lambda_\tau=0\)。

### 12.5 商反射固定点

\(T=L\) 等价于 \(2T\equiv\Theta_u\pmod\Omega\)，因 \(\Omega\) 为奇数
恰有一个商层解。但原层低块从 \(u\) 变为 \(C-u\)，故它仍属于非平凡
二循环，不是原 involution 固定点。

### 12.6 \(\epsilon_{u,T}=0,1\)

两个室分别由 (4.9a)、(4.9b) 双向穷尽；状态计数为
(5.12)–(5.13)。

### 12.7 \(g_u=0\)

由 (4.11) 严格不可能。事实上 \(g_u\ge4\)。

### 12.8 \(s_0=0\)

由原正整数式 (6.4) 严格不可能；准确结论是 \(0<s_0<q_0\)。

### 12.9 \(A_{u,T}=0\)

不能先验删除。它由 (7.17) 精确判定，由 (7.18) 精确计数，并且恰对应
\(\mathcal D_{u,T}<0\)。

### 12.10 \(y=0\) 与 \(z=0\)

两者同时发生，当且仅当 \(A_{u,T}=0,z=0\)。该端点是否真实存在由
完整指数段决定，本文不预删。

### 12.11 \(\mathcal D_{u,T}<0\)

恰为 \(A_{u,T}=0\)。下端使用
\(D_0=-\mathcal D_{u,T}=N_0/M>0\)，没有错误套用正缺陷公式。

### 12.12 \(q=r\)

严格不可能，因为它会给原 involution 固定点。

### 12.13 \(q-r<0\)

不能先验删除。它只可能发生在最小 \(z\)；尤其
\(A_{u,T}=0,z=0\) 时必有 \(q<r\)。

### 12.14 \(\chi=2\varphi\) 与 \(3\Delta=4\varphi\)

两者等价，给无界射线 (1.9)。此时 \(\Omega=C\)、\(\Gamma=1\)，
全文公式仍成立，没有除以零或空室。

### 12.15 \(\mu=0\)

完整包含在 (8.8)、(8.12)、(8.17) 与 (8.21) 中。若它恰为同余类和
大小下端，必须保留。

### 12.16 大小门严格端点

使用 (8.16) 的 \(\mathscr X-1\) 处理严格不等式；(8.18) 同时核对
接受端和相邻拒绝端。以 \(\mu_{\max}\) 写出的 \(z\) 上端使用
\(\le\)，不误写为严格小于。

### 12.17 商反射退化的作用域

式 (4.5) 只直接适用于 \(3\Delta\le4\varphi\)。更深区域必须使用
第 10 节的多块递归；不能把第一商层反射误报为整个真正深区已经关闭。

---

## 13. 为什么不能升级为关闭或绝对有限化

本轮没有得到 GALD1((+))-1，原因是：

1. 统一离散对数目标 (8.6) 在 Jacobi 层自动相容；
2. 正、负缺陷都被严格允许，负缺陷恰对应未被删除的二进零数字端点；
3. \(q-r\) 的 \((2,5)\)-赋值虽被完全固定，但其符号和奇素数部分仍移动；
4. 和差平方路线只是终端乘积的恒等回代，没有新平方判别；
5. 严格大小门只逐状态截断 \(\mu\)，不约束移动模数 \(r\) 的全体；
6. 边界 \((a,\Delta,\varphi)=(7t,4t,3t)\) 是无界射线，现有关系与之
   相容。

本轮没有得到 GALD1((+))-2，因为 \(a,\Delta,u,r\) 仍未绝对有界。

本轮没有得到 GALD1((+))-4，因为两个商进位室、边界射线与严格第一深带
均未统一关闭任何一块。

但本轮严格达到 GALD1((+))-3：

* 原 Möbius involution 完成低块—商双向分解；
* 商层完全仿射反射化，逐位 Hensel 树消失；
* 每个固定 \((a,\Delta,h,J,u,T)\) 至多只剩一条完整有限指数同余段；
* 每个指数唯一恢复全部终端整数；
* 状态计数、二循环奇偶、缺陷符号、\(y=z=0\)、和差符号与精确赋值均已
  显式封闭。

由于残余仍随 \(a,\Delta,u,T,r\) 无界，本文不生成伪造的绝对有限证书，
也不以任何有限参数前缀外推。

---

## 14. 最终分类与停止点

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
\lambda_\tau=C-u+CL,\\
H_u(T,L)=\eta_u+\alpha_uT+\beta_uL+\mathcal BTL,\\
\alpha_u\beta_u-\mathcal B\eta_u=1,
\qquad
\mathcal M_{C-u}\mathcal M_u=I,\\
\Theta_u=\langle Mu^2-1\rangle_\Omega,
\qquad
L=\langle\Theta_u-T\rangle_\Omega,\\
T+L=\Theta_u+\epsilon_{u,T}\Omega,\\
s_0=\epsilon_{u,T}-g_u+M\Gamma S_u(T,L),\\
q_0r=1+B\Lambda N_0,
\qquad
N_0=Jq_0+s_0,
\qquad
0<s_0<q_0,\\
y=Mz-A_{u,T},\\
\mathcal D_{u,T}=(A_{u,T}r-N_0)/M,\\
\mathcal D_{u,T}<0\iff A_{u,T}=0,
\qquad
\mathcal D_{u,T}>0\iff A_{u,T}>0,\\
2^\delta10^\mu=zr-\mathcal D_{u,T},\\
\gcd(\mathcal D_{u,T},r)=1,\\
2^{2a+h}10^{\mu+2a+\Delta}\equiv-1\pmod r,\\
\mu=\mu_0+t\operatorname{ord}_r(10),
\qquad
t_{\min}\le t\le t_{\max},\\
z=\dfrac{\mathcal D_{u,T}+2^\delta10^\mu}{r},\\
\mathscr L=C\{M\Omega z+1+L-\Omega A_{u,T}\}-u,\\
q-r=B(CW_--2u)\ne0,
\qquad
q+r=2+BCW_+,\\
v_2(q-r)=2a+1,
\quad v_5(q-r)=2\varphi,
\quad v_2(q+r)=1,
\quad v_5(q+r)=0.
\end{gathered}
}
\tag{14.1}
\]

全部允许状态由 \(2C/5\) 个低块和每低块两个闭式商区间生成；固定
\(J\) 的终端奇偶门恰保留 \(\Lambda/5\) 个有向状态。每个状态的指数由
一条完整有限同余段穷尽，不存在逐位 Hensel 输出树或多分支指数树。

但移动模数 \(r\)、阶 \(\operatorname{ord}_r(10)\)、低块 \(u\) 和外层
\((a,\Delta)\) 仍无界；两个商进位室与边界射线均未关闭。因此最终分类为

\[
\boxed{\mathrm{GALD1}((+))\text{-}3.}
\]

本文到此停止，不研究第一深带负根、\(3\Delta>4\varphi\) 的更深终端系统、
浅正负根、高 \(\varphi\) 的 \(\mathcal F_{P-}\)、B、C、\(\gamma>1\)、
非本原 C2/C5、Q 或严格层。
