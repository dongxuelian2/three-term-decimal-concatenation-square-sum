# 三项十进制拼接平方和问题：临界 \(G\) 模板本原核心报告

## 1. CD6 后的 \(G\) 状态

本文只研究临界层

\[
(\delta _2,\delta _3)=(-1,1),\qquad N_L=1
\]

中的 \(G\) 模板本原正余数层

\[
\boxed{h=1}.
\]

按本轮约定，暂时接受 T1–T18、K5、CG、E4、GT4、VA1、GD1、
GP3 和 CD6，不作整个项目的统一独立审计。特别地：

\[
J\in\{1,\ldots ,9\},
\qquad
T=\tau N,
\qquad
b_2=\tau q,
\tag{1.1}
\]

\[
N=Jq+s,\qquad
1\le s<q,\qquad
\gcd(s,q)=1,
\tag{1.2}
\]

\[
q\rho-Es=g,\qquad
0<\rho<E,
\tag{1.3}
\]

\[
\tau=\frac{b_1u}{v},\qquad
E=\frac{b_1Y}{v},
\tag{1.4}
\]

\[
\gcd(q,E)=\gcd(q,g)=\gcd(q,10)=1.
\tag{1.5}
\]

沿用

\[
T=10^m,\qquad Y=10^n,\qquad
m\ge2,\quad n\ge1,
\tag{1.6}
\]

\[
u=2^c5^e,\qquad
g=2^a5^\varphi g_\ast,\qquad
a\ge1,\quad \gcd(g_\ast,10)=1.
\tag{1.7}
\]

这里特意把原来记作 \(g_0\) 的、与 \(10\) 互素的奇核心改记为
\(g_\ast\)。原因是约去 \(\gcd(g,E)\) 后出现的行列式商一般不等于
\(g_\ast\)；第 3 节将证明这是本轮必须修正的关键点。

全文仍只分三个阶段，每阶段恰有三个核心新引理：

- 阶段 I：本原行列式、正确约化、A/B/C 指数表；
- 阶段 II：终端因子分解、单位行列式、非单位行列式；
- 阶段 III：约化判别式、尺度恢复刚性、两条无界射线攻击。

本轮最终分类为

\[
\boxed{\mathrm{PR6}}.
\tag{1.8}
\]

得到的是新的既约结构和逐约化状态唯一尺度恢复；没有关闭全部本原层、
单位或非单位行列式完整分支，也没有把 A、B、C 中任一开放室整体关闭。

---

## 2. 本原层正规形

### 2.1 阶段 I 核心引理 PR-I.1：\(q\ge3\) 与四个互素门

由 \(1\le s<q\)，先有 \(q\ge2\)。再由 \(\gcd(q,10)=1\)，

\[
\boxed{q\ge3.}
\tag{2.1}
\]

其次，

\[
N=Jq+s
\]

立即给出

\[
\boxed{
\gcd(N,q)=\gcd(s,q)=1.
}
\tag{2.2}
\]

这一步不需要使用 \(N\) 的 \((2,5)\)-平滑性；它直接来自同一个
欧几里得余数 \(s\)。特别地，

\[
N>q\ge3.
\tag{2.3}
\]

因此本原层的基础互素系统为

\[
\boxed{
\gcd(s,q)=
\gcd(N,q)=
\gcd(q,E)=
\gcd(q,g)=1.
}
\tag{2.4}
\]

这完成题设要求的 \(\gcd(N,q)=1\) 证明。

---

## 3. 奇核心约化

### 3.1 阶段 I 核心引理 PR-I.2：正确的既约行列式

定义

\[
\boxed{d=\gcd(g,E).}
\tag{3.1}
\]

因为

\[
E=\frac{b_1Y}{v}
=2^{\,n+\sigma-\delta}5^n,
\qquad
\sigma=v_2(b_1),\quad
\delta=v_2(v),
\tag{3.2}
\]

而 \(g_\ast\) 与 \(10\) 互素，所以

\[
\boxed{
d=
2^{\min(a,n+\sigma-\delta)}
5^{\min(\varphi,n)}.
}
\tag{3.3}
\]

又由 \(\gcd(q,E)=1\)，

\[
\begin{aligned}
\gcd(\rho,E)
&=\gcd(q\rho,E)\\
&=\gcd(Es+g,E)\\
&=\gcd(g,E)=d.
\end{aligned}
\]

故

\[
\boxed{\gcd(\rho,E)=d.}
\tag{3.4}
\]

写

\[
\rho=d\rho_0,\qquad
E=dE_0,\qquad
\boxed{\gamma=\frac gd}.
\tag{3.5}
\]

则真正的既约行列式是

\[
\boxed{
q\rho_0-E_0s=\gamma,
}
\tag{3.6}
\]

并且

\[
\boxed{
\gcd(q,E_0)=
\gcd(\rho_0,E_0)=
\gcd(s,q)=
\gcd(N,q)=1,
}
\tag{3.7}
\]

\[
\boxed{
\gcd(\gamma,E_0)=
\gcd(\gamma,q)=1.
}
\tag{3.8}
\]

因此

\[
\boxed{
\frac{\rho_0}{E_0}-\frac{s}{q}
=\frac{\gamma}{qE_0}>0.
}
\tag{3.9}
\]

这里

\[
\boxed{
\gamma=
2^{a-\min(a,n+\sigma-\delta)}
5^{\varphi-\min(\varphi,n)}
g_\ast.
}
\tag{3.10}
\]

所以题设拟写的

\[
q\rho_0-E_0s=g_0
\]

只有在

\[
a\le n+\sigma-\delta,\qquad
\varphi\le n
\tag{3.11}
\]

时，才可把右端认作原奇核心 \(g_\ast\)。一般情形必须使用
\(\gamma=g/d\)。

尤其：

- \(g_\ast>1\) 必然推出 \(\gamma>1\)；
- \(g_\ast=1\) 却不推出 \(\gamma=1\)，因为未被 \(E\) 吸收的
  \(2\)-进或 \(5\)-进溢出仍留在 \(\gamma\) 中。

因此阶段 II 的 Farey 分支必须按

\[
\boxed{\gamma=1\quad\text{与}\quad\gamma>1}
\tag{3.12}
\]

划分，而不能按原奇核心 \(g_\ast=1\) 与 \(g_\ast>1\) 划分。

---

## 4. A、B、C 映射

### 4.1 阶段 I 核心引理 PR-I.3：本原层的完整指数表

GP3 给出

\[
x=\sigma+c-\delta,\qquad
h=2^{x-\min(m,x)}5^{e-\min(m,e)}.
\tag{4.1}
\]

所以

\[
\boxed{
h=1
\iff
x\le m,\quad e\le m.
}
\tag{4.2}
\]

在本原层中

\[
\boxed{
N=2^{m-x}5^{m-e},
\qquad
E=2^{n+\sigma-\delta}5^n.
}
\tag{4.3}
\]

逐行代入 E4 的 A、B、C、D 位置，得到下表。表中

\[
r_2=\min(a,v_2(E)),\qquad
r_5=\min(\varphi,n).
\tag{4.4}
\]

| E4 位置 | \((b_1,v,c)\) | \(N\) | \(E\) | \(d\) | \(E_0\) |
|---|---:|---:|---:|---:|---:|
| A | \((2,2,0)\) | \(2^m5^{m-e}\) | \(2^n5^n\) | \(2^{\min(a,n)}5^{r_5}\) | \(2^{n-\min(a,n)}5^{n-r_5}\) |
| B，\(b_1=1\) | \((1,1,c),\ 0\le c<m\) | \(2^{m-c}5^{m-e}\) | \(2^n5^n\) | \(2^{\min(a,n)}5^{r_5}\) | \(2^{n-\min(a,n)}5^{n-r_5}\) |
| B，\(b_1=2\) | \((2,1,c),\ 0\le c\le m-1\) | \(2^{m-c-1}5^{m-e}\) | \(2^{n+1}5^n\) | \(2^{\min(a,n+1)}5^{r_5}\) | \(2^{n+1-\min(a,n+1)}5^{n-r_5}\) |
| C 边界 | \((1,1,m)\) | \(5^{m-e}\) | \(2^n5^n\) | \(2^{\min(a,n)}5^{r_5}\) | \(2^{n-\min(a,n)}5^{n-r_5}\) |

这里所有行还必须满足 \(e\le m\)。结论如下。

1. A 全部进入本原层；
2. B 全部进入，包括
   \[
   b_1=2,\quad c=m-1,\quad x=m
   \]
   的二进饱和边界；
3. C 只允许
   \[
   \boxed{b_1=1,\quad x=m;}
   \]
4. C 的 \(b_1=2\) 行有 \(x=m+1\)，不在本原层；
5. D 中 \(x>m\)，全部不在本原层；
6. \(e>m\) 的五进溢出全部不在本原层。

C 的 \(b_1=1,x=m\) 边界没有遗漏。但在该边界若 \(e=m\)，则

\[
N=1,
\]

与 \(N>q\ge3\) 矛盾。因此真正存活的 C 本原状态还满足

\[
\boxed{b_1=1,\quad c=m,\quad e<m.}
\tag{4.5}
\]

本原层中的 D 为空是 GP3 内容表的精确后果，不是本轮借判别式新关闭的
E4 室；第 9 节因此不把它重复计为 PR3。

---

## 5. \(\gamma=1\)：单位行列式

### 5.1 阶段 II 核心引理 PR-II.1：终端因子分解

先对任意 \(\gamma\ge1\) 建立共同正规形。GT4 有

\[
\chi=gk-\frac Yv=JE+\rho.
\tag{5.1}
\]

由 \(d\mid E,\rho,g\)，式 (5.1) 说明

\[
\boxed{d\mid\frac Yv.}
\tag{5.2}
\]

定义

\[
\boxed{
Z=\frac{Y}{vd}\in\mathbb Z_{>0},
\qquad
M_0=JE_0+\rho_0.
}
\tag{5.3}
\]

则

\[
\boxed{
E_0=b_1Z,\qquad
M_0=\gamma k-Z.
}
\tag{5.4}
\]

把 \(N=Jq+s\) 代入 (3.6)，得到移位行列式

\[
\boxed{
qM_0-E_0N=\gamma.
}
\tag{5.5}
\]

再代入 (5.4)，恰得

\[
\boxed{
\gamma(qk-1)=Z(q+b_1N).
}
\tag{5.6}
\]

由于 \(\gcd(\gamma,Z)=1\)，

\[
\boxed{
\gamma\mid q+b_1N,\qquad
Z\mid qk-1.
}
\tag{5.7}
\]

令

\[
C=\frac{q+b_1N}{\gamma}\in\mathbb Z_{>0},
\]

则

\[
\boxed{qk-1=ZC.}
\tag{5.8}
\]

又因

\[
Jq<N<(J+1)q,\qquad J\le9,\qquad b_1\le2,
\]

有严格大小关系

\[
\boxed{
\gamma\le q+b_1N<(1+10b_1)q\le21q.
}
\tag{5.9}
\]

这就是非单位行列式所要求的终端分母窗口大小关系。它把
\(\gamma\) 压入一个真实终端因子，但 \(q,N\) 仍可移动，所以不是绝对上界。

### 5.2 阶段 II 核心引理 PR-II.2：Farey 结论及其准确能力

现在假设

\[
\boxed{\gamma=1.}
\tag{5.10}
\]

由 (3.7)，

\[
\frac{s}{q},\qquad\frac{\rho_0}{E_0}
\]

均为既约分数，并满足

\[
q\rho_0-E_0s=1.
\]

因此它们在任意满足

\[
\max(q,E_0)\le Q<q+E_0
\]

的 Farey 序列 \(F_Q\) 中相邻。等价地，任意严格位于二者之间的
既约分数 \(x/y\) 都满足

\[
\boxed{y\ge q+E_0.}
\tag{5.11}
\]

移位后的两个分数

\[
\frac Nq=J+\frac sq,\qquad
\frac{M_0}{E_0}=J+\frac{\rho_0}{E_0}
\]

也满足

\[
\boxed{
\frac{M_0}{E_0}-\frac Nq=\frac1{qE_0},
\qquad
qM_0-E_0N=1.
}
\tag{5.12}
\]

结合 (5.6)，单位行列式进一步等价于

\[
\boxed{
qk-1=Z(q+b_1N),\qquad E_0=b_1Z.
}
\tag{5.13}
\]

在 A、B 中 \(q+b_1N\) 为奇数，故 (5.13) 的二进赋值正好恢复
E4 的 A、B 循环关系；在 C 中

\[
\eta=v_2(q+N),
\]

式 (5.13) 正好恢复

\[
a+\lambda=n+\eta.
\]

所以单位行列式与 \(N,\chi\) 的联合并没有额外制造一个位于
\(s/q\) 与 \(\rho_0/E_0\) 之间、且分母小于 \(q+E_0\) 的既约分数。
特别地，不能仅凭两个端点处于同一单位区间或同一终端商 \(J\)
推出矛盾。

### 5.3 一个通过全部前置门的无界单位射线

对任意

\[
n\ge5,
\]

取

\[
\begin{gathered}
m=2,\quad b_1=v=2,\quad u=25,\quad
T=100,\quad Y=10^n,\\
q=3,\quad N=4,\quad J=1,\quad s=1,\\
d=g=\frac{Y}{500}
=2^{n-2}5^{n-3},\\
E_0=500,\quad \rho_0=167,\quad
Z=250,\quad k=917.
\end{gathered}
\tag{5.14}
\]

则

\[
3\cdot167-500=1,
\]

故 \(\gamma=1\)。同时

\[
b_2=75,\qquad b_3=\frac Y{10},
\tag{5.15}
\]

命中真实分母窗口，并且

\[
qk-1=2750=250(3+2\cdot4).
\tag{5.16}
\]

这里

\[
a=n-2,\qquad \varphi=n-3,\qquad
\lambda=v_2(2750)=1,\qquad n=a+2,
\]

所以它位于 A1。E4 的真实高阶括号等于

\[
5^{n-3}\cdot2634100,
\]

而

\[
2634100\equiv4\pmod8,
\]

故

\[
\boxed{\theta_A=2,}
\tag{5.17}
\]

正好满足 A1 在 \(a\ge3\) 时的高阶门。

十三首块和分子前置门也非空：例如可取

\[
a_1=5,\qquad a_2=1,\qquad a_3=Y+1.
\]

它们满足真实分子窗口及三个逐项既约条件。该族不是原题解；第 7 节将
用完整判别式统一排除它。它在此处的作用是严格证明：

\[
\boxed{
\gamma=1+\text{Farey 相邻}+N,\chi+\text{全部分母/K5/E4 前置门}
}
\]

仍允许 \(n,a,\varphi,d\) 无界，因而不能仅凭阶段 II 关闭单位行列式分支。

---

## 6. \(\gamma>1\)：非单位行列式

### 6.1 阶段 II 核心引理 PR-II.3：耦合单元而非独立 Farey 间隔

设

\[
\gamma>1.
\]

若既约分数 \(x/y\) 严格位于

\[
\frac sq<\frac xy<\frac{\rho_0}{E_0},
\]

则两个整数

\[
qx-sy>0,\qquad
\rho_0y-E_0x>0.
\]

恒等式

\[
E_0(qx-sy)+q(\rho_0y-E_0x)=\gamma y
\]

给出

\[
\boxed{
y\ge\left\lceil\frac{q+E_0}{\gamma}\right\rceil.
}
\tag{6.1}
\]

当 \(\gamma=1\) 时这退化为标准 Farey 下界。对
\(\gamma>1\)，端点之间可以作正规扇形的单位行列式细分，但中间向量由
同一个欧几里得递推耦合；它们不是 \(\gamma\) 个可独立选择的 Farey
间隔。现有主系统也没有指定某个必须出现且违反 (6.1) 的中间分数。

另一方面，(5.7) 给出真正可用的算术约束

\[
\boxed{
\gamma\mid q+b_1N,\qquad
\gamma<21q.
}
\tag{6.2}
\]

这说明 \(\gamma\) 的全部素因子来自移动的终端因子
\(q+b_1N\)，而不是固定有限素数集。由于 \(q,N\) 仍无界，
(6.2) 没有把非单位分支化成有限多个固定行列式状态。

### 6.2 原奇核心 \(g_\ast=1\) 仍可有 \(\gamma>1\)

对任意

\[
n\ge2,
\]

取

\[
\begin{gathered}
m=2,\quad b_1=v=1,\quad u=4,\quad
T=100,\quad Y=10^n,\\
q=3,\quad N=25,\quad J=8,\quad s=1,\\
d=\frac Y{25}=2^n5^{n-2},\qquad
g=2d=2^{n+1}5^{n-2},\\
E_0=25,\quad \rho_0=9,\quad
\gamma=2,\quad Z=25,\quad k=117.
\end{gathered}
\tag{6.3}
\]

则

\[
3\cdot9-25=2,
\tag{6.4}
\]

\[
2(3\cdot117-1)=25(3+25),
\tag{6.5}
\]

\[
b_2=12,\qquad
b_3=\frac{8Y}{25}.
\tag{6.6}
\]

该族满足真实分母窗口、K5 支撑和 \(h=1\)。又有

\[
a=n+1,\qquad
\varphi=n-2,\qquad
g_\ast=1,
\]

\[
\lambda=v_2(3\cdot117-1)=1,\qquad
\eta=v_2(3+25)=2.
\]

因此

\[
a+\lambda=n+\eta,\qquad
\lambda<2\eta+1,\qquad
2a>n,
\]

恰位于 E4 的 C1 室。取

\[
a_1=a_2=1,\qquad a_3=Y+1
\]

还可通过十三首块、真实分子窗口和逐项既约前置门。

这个无界族严格证明

\[
\boxed{
g_\ast=1\centernot\Longrightarrow\gamma=1.
}
\tag{6.7}
\]

在该例中，两个端点为

\[
\frac13<\frac9{25},
\]

它们的行列式为 \(2\)；唯一最简单的单位细分是

\[
\frac13<\frac5{14}<\frac9{25},
\]

两个小行列式均为 \(1\)，而中间分母

\[
14=\frac{3+25}{2}
\]

恰命中 (6.1)。这个中间项由两个端点共同决定，不能作为两个独立
Farey 间隔的自由变量使用。

---

## 7. 完整判别式

### 7.1 阶段 III 核心引理 PR-III.1：约化判别式

令

\[
R=(ua_1)^2+(va_2)^2,\qquad
H_1=a_1T+10a_2.
\tag{7.1}
\]

完整判别式为

\[
\mathcal D
=Y^2H_1^2-(k^2-1)g^2R.
\tag{7.2}
\]

由

\[
Y=vdZ,\qquad g=d\gamma,
\]

精确提出平方因子：

\[
\boxed{
\mathcal D=d^2\Delta,
}
\tag{7.3}
\]

其中

\[
\boxed{
\Delta=
v^2Z^2H_1^2
-(k^2-1)\gamma^2
\bigl((ua_1)^2+(va_2)^2\bigr).
}
\tag{7.4}
\]

若 \(\mathcal D=w^2\)，则逐素数比较 \(d^2\mid w^2\) 得

\[
\boxed{w=dw_0,\qquad \Delta=w_0^2}
\tag{7.5}
\]

其中 \(w_0\in\mathbb Z_{\ge0}\)。因而大公共尺度 \(d\) 不应继续
留在平方判别中；真正的平方问题是 (7.4)。

此外，GT4 的 \(\chi>E\) 与尾窗给出 \(k>1\)，故

\[
K:=k^2-1>0.
\tag{7.6}
\]

### 7.2 阶段 III 核心引理 PR-III.2：恢复—既约迫使唯一尺度

假设 (7.5) 成立。对两个符号分别定义

\[
L_\pm=vZH_1\pm kw_0,
\tag{7.7}
\]

\[
c_\pm=\gcd(K,L_\pm),\qquad
K_\pm'=\frac K{c_\pm}.
\tag{7.8}
\]

这里只保留使 \(L_\pm>0\) 的符号，并把 \(\gcd(K,L_\pm)\) 理解为
正最大公因数。

第三块恢复式变为

\[
a_3=\frac{dL_\pm}{K}.
\tag{7.9}
\]

写

\[
K=c_\pm K_\pm',\qquad
L_\pm=c_\pm L_\pm',\qquad
\gcd(K_\pm',L_\pm')=1.
\]

若 (7.9) 为整数，则 \(K_\pm'\mid d\)。令

\[
d=K_\pm' e_\pm.
\]

于是

\[
a_3=e_\pm L_\pm'.
\]

另一方面

\[
b_3=b_1gu=b_1d\gamma u
\]

也被 \(e_\pm\) 整除。逐项既约
\(\gcd(a_3,b_3)=1\) 因而强迫

\[
e_\pm=1.
\]

所以任何完整候选都必须满足

\[
\boxed{
d=
\frac{k^2-1}
{\gcd(k^2-1,\ vZH_1\pm kw_0)}.
}
\tag{7.10}
\]

相应地，

\[
\boxed{
d\mid k^2-1,\qquad
a_3=
\frac{vZH_1\pm kw_0}
{\gcd(k^2-1,\ vZH_1\pm kw_0)}.
}
\tag{7.11}
\]

这是完整判别式、\(a_3\) 恢复和第三块既约联合后的新刚性：

\[
\boxed{
\text{固定 }(q,N,\gamma,Z,k,u,v,a_1,a_2)
\text{ 后，每个符号至多允许一个 }d.
}
\tag{7.12}
\]

还得到高阶赋值门

\[
\boxed{
v_2(d)\le v_2(k^2-1),\qquad
v_5(d)\le v_5(k^2-1).
}
\tag{7.13}
\]

但 \(k\) 与全部约化状态仍可无界移动，所以 (7.10)–(7.13) 不是
对 \(d,a,\varphi\) 的绝对统一上界。

### 7.3 阶段 III 核心引理 PR-III.3：两条无界射线的完整判别式攻击

先处理第 5.3 节的单位射线。这里

\[
E_0=500,\quad
\gamma=1,\quad
u=25,\quad v=2,\quad k=917.
\]

十三首块和中分子窗口只有

\[
a_1\in\{5,7,9,11,13\},
\qquad
a_2\in\{1,2,4,7,8\}.
\tag{7.14}
\]

约化判别式为

\[
\Delta_A
=500^2(100a_1+10a_2)^2
-(917^2-1)\bigl((25a_1)^2+(2a_2)^2\bigr).
\tag{7.15}
\]

模 \(5\) 有

\[
\Delta_A\equiv3a_2^2\pmod5.
\]

由于 \(5\nmid a_2\)，右端只能为 \(2\) 或 \(3\)，均非平方剩余。
故

\[
\boxed{\text{第 5.3 节的全部无界单位射线由 }\mathcal D\text{ 非平方关闭}.}
\tag{7.16}
\]

再处理第 6.2 节的非单位 C1 射线。这里

\[
E_0=25,\quad
\gamma=2,\quad
u=4,\quad v=1,\quad k=117,
\]

\[
a_1\in\{1,\ldots,8\},\qquad
a_2\in\{1,5,7\}.
\tag{7.17}
\]

约化判别式为

\[
\Delta_C
=25^2(100a_1+10a_2)^2
-(117^2-1)\bigl((4a_1)^2+a_2^2\bigr).
\tag{7.18}
\]

下表在每个固定格中给出一个使 \(\Delta_C\) 为二次非剩余的素数。
列标是 \(a_2\)，行标是 \(a_1\)。

| \(a_1\backslash a_2\) | \(1\) | \(5\) | \(7\) |
|---:|---:|---:|---:|
| 1 | 7 | 3 | 19 |
| 2 | 3 | 5 | 3 |
| 3 | 3 | 3 | 3 |
| 4 | 7 | 3 | 17 |
| 5 | 3 | 7 | 3 |
| 6 | 3 | 3 | 3 |
| 7 | 17 | 3 | 19 |
| 8 | 3 | 5 | 3 |

因此

\[
\boxed{\text{第 6.2 节的全部无界非单位 C1 射线也由 }\mathcal D
\text{ 非平方关闭}.}
\tag{7.19}
\]

这里的有限表不枚举无界参数 \(n\)：\(n\) 已由 (7.3) 完整提出为
平方因子 \(d^2\)，表中检查的是全部真实首块和中分子块形成的
固定约化二次型。因此 (7.19) 是对整条无界射线的证明，不是有限搜索
外推。

两条射线的关闭说明约化判别式确实比 Farey 结构更强；但它们只是 A1
和 C1 中的两个固定约化状态。一般的

\[
(q,N,\gamma,Z,k,u,v)
\]

仍可移动，(7.4) 尚未成为有限多个固定二次型。

---

## 8. 反例攻击与主动审计

### 8.1 \(h=1\) 是否确实排除 D

是。D 中 \(c=m+j\)，且

\[
x=\sigma+c>m.
\]

故 \(v_2(h)=x-m>0\)，与 \(h=1\) 矛盾。

### 8.2 是否遗漏 C 的 \(b_1=1\)

没有。C 的 \(b_1=1,c=m,x=m\) 被完整列入表 (4.3)；只额外由
\(N>q\ge3\) 排除了其中 \(e=m,N=1\) 的空边界。

### 8.3 \(\gcd(N,q)=1\) 是否正确

是。它直接来自

\[
\gcd(N,q)=\gcd(Jq+s,q)=\gcd(s,q)=1.
\]

### 8.4 \(\gcd(\rho,E)=\gcd(g,E)\) 是否正确

是。关键是先用 \(\gcd(q,E)=1\) 把
\(\gcd(\rho,E)\) 换成 \(\gcd(q\rho,E)\)，再使用
\(q\rho=Es+g\)。

### 8.5 是否把原奇核心误当成约化行列式

没有。全文严格区分

\[
g_\ast\quad\text{与}\quad\gamma=g/d.
\]

第 6.2 节给出的无界 C1 族满足 \(g_\ast=1,\gamma=2\)，是对错误
识别的机制级反例。

### 8.6 是否把 \(\gamma=1\) 自动写成固定 Farey 阶数

没有。准确说法是：端点在

\[
\max(q,E_0)\le Q<q+E_0
\]

的 Farey 序列中相邻；\(q,E_0\) 自身仍可变化。

### 8.7 是否把 \(\gamma>1\) 拆成独立单位间隔

没有。只使用了严格分母下界 (6.1) 和终端因子分解 (6.2)。
任何正规细分中的中间向量仍由同一欧几里得递推耦合。

### 8.8 是否忘记十三首块、真实分子窗口和 \(a_3\) 恢复

没有。第 7.3 节的两条射线分别穷尽相应的五种或八种首块，以及
全部合法一位中分子块。一般系统仍保留 (7.10)–(7.11)、第三块窗口和
三个逐项既约条件。

### 8.9 是否只检查判别式平方

没有。PR-III.2 明确把平方根代回 \(a_3\)，并用
\(\gcd(a_3,b_3)=1\) 推出唯一尺度公式 (7.10)。判别式平方仍只是一道
必要门。

### 8.10 是否用有限搜索支持无界结论

没有。第 7.3 节先代数提出完整平方尺度 \(d^2\)，剩下的有限格正好是
固定 \(m=2\) 射线中的全部真实分子块；结论覆盖每个允许的 \(n\)。
没有用任何有界盒推断 A、B、C 的全局结论。

### 8.11 辅助族是否满足完整前置门

是。第 5.3、6.2 节逐项满足：

- \(h=1\)、\(J\in\{1,\ldots,9\}\)、\(q\ge3\)；
- 真实 \(T,b_2,Y,b_3\) 窗口；
- K5 的互素和支撑门；
- E4 的 A1 高阶门或 C1 共振门；
- 十三首块、真实分子窗口和逐项既约前置门。

它们随后被完整判别式统一排除，从未被表述为原题解。

---

## 9. 最终分类 PR1–PR6

本轮达到

\[
\boxed{
\mathrm{PR6}:
\quad
\text{得到正确的既约行列式、终端因子分解和唯一尺度恢复，}
\text{但未关闭完整开放分支或开放室}.
}
\tag{9.1}
\]

决定性新链条为

\[
\boxed{
\begin{gathered}
d=\gcd(g,E),\quad
\gamma=g/d\\
\Longrightarrow
q\rho_0-E_0s=\gamma,\quad
qM_0-E_0N=\gamma;\\
\chi=gk-Y/v=JE+\rho\\
\Longrightarrow
d\mid Y/v,\quad
\gamma(qk-1)=Z(q+b_1N);\\
\Longrightarrow
\gamma\mid q+b_1N,\quad\gamma<21q;\\
\mathcal D=d^2\Delta,\quad
\Delta=w_0^2,\quad
\gcd(a_3,b_3)=1\\
\Longrightarrow
d=\frac{k^2-1}
{\gcd(k^2-1,vZH_1\pm kw_0)}.
\end{gathered}
}
\tag{9.2}
\]

为什么不是 PR1：

- A、B、C 均仍有开放本原状态。

为什么不是 PR2：

- \(\gamma=1\) 和 \(\gamma>1\) 都存在通过全部分母、K5、E4
  前置门的无界射线；
- 本轮只用完整判别式关闭了其中两个固定约化射线，没有关闭任一完整
  行列式分支。

为什么不是 PR3：

- D 在 \(h=1\) 中为空是 GP3 内容映射的继承结论；
- 本轮没有用新的球面—拼接论证关闭 A、B、C 中任一完整开放室。

为什么不是 PR4：

- (7.10) 固定每个约化状态上的尺度 \(d\)，但
  \(q,N,\gamma,Z,k,u,v\) 仍可无界移动；
- \(d\le k^2-1\) 不是绝对参数上界。

为什么不是 PR5：

- 行列式商满足 \(\gamma\mid q+b_1N\)，但终端因子本身移动；
- 约化判别式的系数仍随
  \((q,N,\gamma,Z,k,u,v)\) 变化，尚未得到有限多个固定行列式状态。

为什么达到 PR6：

1. 修正了原奇核心与约化行列式商的非等价；
2. 建立了同时耦合 \(N,\chi\) 的移位行列式；
3. 把非单位行列式压入真实终端因子；
4. 提出判别式的完整公共平方尺度；
5. 联合 \(a_3\) 恢复和逐项既约，证明每个约化状态每个符号至多有一个
   原尺度；
6. 两个满足全部前置门的无界射线被完整判别式严格关闭。

没有找到合法原题解。

---

## 10. \(G\) 模板最新状态

结合 VA1、GD1、GP3、CD6 与本报告，本原正余数层必须满足

\[
\boxed{
\begin{gathered}
J\in\{1,\ldots,9\},\qquad q\ge3,\\
T=\frac{b_1u}{v}N,\qquad
b_2=\frac{b_1u}{v}q,\\
N=Jq+s,\qquad
1\le s<q,\qquad
\gcd(N,q)=\gcd(s,q)=1,\\
q\rho_0-E_0s=\gamma,\qquad
\gcd(q,E_0)=\gcd(\rho_0,E_0)=1,\\
d\mid Y/v,\qquad
E_0=b_1Z,\qquad
\gamma(qk-1)=Z(q+b_1N),\\
\gamma\mid q+b_1N,\qquad
\gamma<21q.
\end{gathered}
}
\tag{10.1}
\]

其 E4 支持恰为：

\[
\boxed{
\begin{array}{c|c}
\mathrm A&\text{全部，且 }e\le m\\
\mathrm B&\text{全部，且 }e\le m\\
\mathrm C&b_1=1,\ c=m,\ e<m\\
\mathrm D&\text{本原层中为空}
\end{array}
}
\tag{10.2}
\]

任何完整候选还必须满足

\[
\boxed{
\Delta=
v^2Z^2H_1^2
-(k^2-1)\gamma^2
\bigl((ua_1)^2+(va_2)^2\bigr)
=w_0^2,
}
\tag{10.3}
\]

以及某一符号下的

\[
\boxed{
d=
\frac{k^2-1}
{\gcd(k^2-1,vZH_1\pm kw_0)},
}
\tag{10.4}
\]

\[
\boxed{
a_3=
\frac{vZH_1\pm kw_0}
{\gcd(k^2-1,vZH_1\pm kw_0)}
\in[Y,10Y),
}
\tag{10.5}
\]

再联合十三首块、真实中分子窗口和三个逐项既约条件。

当前仍未统一控制

\[
\boxed{
q,\ N,\ \gamma,\ Z,\ k,\ m,\ n,\ a,\ e,\ \varphi,
\quad
\eta,\theta_A,\theta_B,\kappa
}
\tag{10.6}
\]

及 B 边界的 \(e_2,h_B,\varepsilon_B\) 等高阶参数。

本轮的准确停止点是：

\[
\boxed{
\begin{gathered}
\text{本原层 D 为空，C 的真实边界已完整保留；}\\
\text{原奇核心分支必须改为约化行列式分支 }\gamma=1,\gamma>1;\\
\text{单位 Farey 结构本身不关闭分支；}\\
\text{非单位商被压入 }q+b_1N\text{，但该因子仍移动；}\\
\text{完整球面—拼接使每个约化状态至多恢复两个符号尺度，}\\
\text{却尚未把约化状态本身有限化；}\\
\text{故最终分类为 PR6。}
\end{gathered}
}
\]

全文到此停止；不研究 C2、C5、O 或 Q，也不返回 \(J=10\)、
零余数或 \(5\mid q\)。
