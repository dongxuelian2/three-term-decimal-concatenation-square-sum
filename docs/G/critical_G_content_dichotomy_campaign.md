# 三项十进制拼接平方和问题：临界 \(G\) 模板非本原内容二分报告

## 1. GP3 后的剩余系统

本文只研究临界层

\[
(\delta _2,\delta _3)=(-1,1),\qquad N_L=1
\]

中的偶边模板

\[
\mathrm G:\qquad 2\mid g
\]

的正余数、非本原内容层

\[
\boxed{h>1}.
\]

按本轮约定，暂时接受 T1–T18、K5、CG、E4、GT4、VA1、GD1
和 GP3，不作整个项目的统一独立审计。特别地：

- VA1 已关闭 \(J=10\)；
- GD1 已关闭零余数 \(T-Jb_2=0\)；
- GP3 已关闭 \(5\mid q\)。

因此起始系统恰为

\[
\boxed{
\begin{gathered}
J\in\{1,\ldots ,9\},\qquad
T=\tau N,\qquad b_2=\tau qh,\\
N=Jqh+s,\qquad
1\le s<qh,\qquad
\gcd(s,qh)=1,\\
q\rho-Fs=g,\qquad
0<\rho<hF,\\
\gcd(q,F)=1,\qquad
\gcd(q,10)=1,\qquad
\gcd(q,g)=1.
\end{gathered}}
\tag{1.1}
\]

这里

\[
T=10^m,\qquad Y=10^n,\qquad m\ge2,\quad n\ge1,
\tag{1.2}
\]

\[
g=2^a5^\varphi g_0,\qquad
a\ge1,\qquad \gcd(g_0,10)=1,
\tag{1.3}
\]

\[
u=2^c5^e,\qquad
v\in\{1,2\},\qquad
v\mid b_1,\qquad
\gcd(u,v)=1,
\tag{1.4}
\]

\[
b_2=\frac{b_1qu}{v},\qquad
b_3=b_1gu,
\tag{1.5}
\]

\[
\frac T{10}\le b_2<T,\qquad
\frac Y{10}\le b_3<Y.
\tag{1.6}
\]

K5 支撑条件

\[
\operatorname{rad}(u)\mid qg
\tag{1.7}
\]

和 E4 的全部 A、B、C、D 室、高阶消去参数及逐项既约条件始终保留。

记

\[
\sigma=v_2(b_1)\in\{0,1\},\qquad
d=v_2(v)\in\{0,1\},
\tag{1.8}
\]

\[
x=\sigma+c-d,\qquad
\alpha=\min(m,x),\qquad
\beta=\min(m,e).
\tag{1.9}
\]

由 GP3，

\[
\boxed{N=2^{m-\alpha}5^{m-\beta}},
\tag{1.10}
\]

\[
\boxed{h=2^{x-\alpha}5^{e-\beta}},
\tag{1.11}
\]

\[
\boxed{
F=2^{\alpha+n-c}5^{\beta+n-e}.
}
\tag{1.12}
\]

全文仍严格分为三个阶段，每阶段至多三个核心新引理：

- 阶段 I：CD-I.1–CD-I.3，互素性、纯内容三分法和 E4 映射；
- 阶段 II：CD-II.1–CD-II.3，唯一本原基底、内容提升和 \(q=1\)；
- 阶段 III：CD-III.1–CD-III.3，C2、C5 主方程及判别式攻击。

本轮最终分类为

\[
\boxed{\mathrm{CD6}.}
\tag{1.13}
\]

其准确含义不是“接近关闭”，而是：

1. \(h>1\) 被严格分成纯二进内容 C2 和纯五进内容 C5；
2. 每个 \((q,F,g)\) 的本原基底唯一；
3. 互素门单独恰放行 \(\varphi(h)\) 个提升，但加入互补纯幂与
   \(J\le9\) 后，实际候选统一降为至多九个提升；
4. \(q=1\) 得到完整指数带和新的判别式符号门，关闭一批低 \(J\)
   单元，但没有整体关闭；
5. C5 得到
   \[
   H\le n-1,
   \]
   但没有得到 \(H\) 的绝对上界；
6. C2 的 D1、D2 均存在通过全部分母、循环和 E4 前置门的无界辅助族，
   因而没有达到 CD1–CD5。

---

## 2. \(\gcd(N,h)=1\)

### 2.1 核心引理 CD-I.1：互补最小指数

由

\[
\alpha=\min(m,x)
\]

可得

\[
\min(m-\alpha,x-\alpha)=0.
\tag{2.1}
\]

因此素数 \(2\) 不可能同时整除 \(N\) 与 \(h\)。同理，

\[
\beta=\min(m,e)
\]

给出

\[
\min(m-\beta,e-\beta)=0,
\tag{2.2}
\]

所以素数 \(5\) 也不可能同时整除 \(N\) 与 \(h\)。

由于 \(N,h\) 都是 \((2,5)\)-平滑数，

\[
\boxed{\gcd(N,h)=1.}
\tag{2.3}
\]

这不是从 \(\gcd(s,qh)=1\) 间接猜出的条件，而是 (1.10)–(1.11)
在两个素数上的精确互补。

### 2.2 核心引理 CD-I.2：严格大小关系

由

\[
N=Jqh+s,
\qquad
J,q,h\ge1,\quad s\ge1,
\]

立即得到

\[
N\ge h+s>h.
\]

故

\[
\boxed{N>h.}
\tag{2.4}
\]

特别地，在本轮 \(h>1\) 中，

\[
N>1.
\tag{2.5}
\]

这一步必须保留；若只使用互素性而不使用 \(N>h\)，会错误允许
\(N=1\) 的伪分支。

---

## 3. 纯内容三分法

### 3.1 核心引理 CD-I.3：唯一纯内容分类

由 (2.3)，\(N\) 与 \(h\) 的素数支撑不交。由 (2.4)，当 \(h>1\)
时二者又都大于 \(1\)。因此 \(h\) 不可能同时含 \(2\) 和 \(5\)：
若 \(2\mid h\) 且 \(5\mid h\)，则互素性会迫使 \(N=1\)，与
\(N>h\) 矛盾。

故所有候选唯一落入以下三类。

### P：本原层

\[
\boxed{h=1.}
\tag{3.1}
\]

本轮不研究。

### C2：纯二进内容

\[
\boxed{
h=2^H,\qquad N=5^R,\qquad H,R\ge1.
}
\tag{3.2}
\]

由 (1.10)–(1.11)，这等价于

\[
\boxed{x>m,\qquad e<m,}
\tag{3.3}
\]

且

\[
\boxed{H=x-m,\qquad R=m-e.}
\tag{3.4}
\]

注意必须是 \(e<m\)，不能把边界 \(e=m\) 放进 C2；在 \(e=m\) 时
\(N\) 的五进指数为零，从而 \(N=1\)，与 \(N>h\) 矛盾。

### C5：纯五进内容

\[
\boxed{
h=5^H,\qquad N=2^R,\qquad H,R\ge1.
}
\tag{3.5}
\]

这等价于

\[
\boxed{e>m,\qquad x<m,}
\tag{3.6}
\]

且

\[
\boxed{H=e-m,\qquad R=m-x.}
\tag{3.7}
\]

同理，边界 \(x=m\) 不能放进 C5。

所以所有交叉状态

\[
x>m,\qquad e>m
\tag{3.8}
\]

全部删除。它们不是第四种“混合内容”，而是与
\(\gcd(N,h)=1\)、\(N>h\) 同时矛盾。

### 3.2 C2 映射回 E4

在 E4 中，\(x>m\) 只可能发生于：

\[
\boxed{
\begin{array}{c|c|c|c}
\text{位置}&(b_1,v,c)&H&F\\ \hline
\mathrm C&(2,1,m)&1&2^n5^n=Y\\
\mathrm D&(1,1,m+j)&j&2^{n-j}5^n\\
\mathrm D&(2,1,m+j)&j+1&2^{n-j}5^n
\end{array}}
\tag{3.9}
\]

其中 \(j>0\)。因此：

- C 中只能有 \(b_1=2\)；
- D 中允许 \(b_1=1,2\)；
- C 的 \(b_1=1,x=m\) 边界不属于 C2；
- 不允许五进溢出，因为 \(e<m\)。

统一地，

\[
\boxed{
F=2^{m+n-c}5^n.
}
\tag{3.10}
\]

### 3.3 C5 映射回 E4

条件 \(x<m\) 只允许：

\[
\boxed{
\begin{array}{c|c|c}
\text{位置}&(b_1,v,c)&R\\ \hline
\mathrm A&(2,2,0)&m\\
\mathrm B&(1,1,c<m)&m-c\\
\mathrm B&(2,1,0\le c\le m-2)&m-c-1
\end{array}}
\tag{3.11}
\]

所以 C5 只能进入 A 和 B 的非二进饱和状态。它不能进入：

- C 的 \(b_1=2\) 行；
- C 的 \(b_1=1,x=m\) 边界；
- B 的 \(b_1=2,c=m-1,x=m\) 饱和边界；
- 任意 D 室。

在 C5 中

\[
\boxed{
F=2^{n+\sigma-d}5^{n-H}.
}
\tag{3.12}
\]

由 \(F\in\mathbb Z\) 已有 \(H\le n\)；阶段 III 将把它严格加强为
\(H\le n-1\)。

---

## 4. 唯一本原基底

### 4.1 核心引理 CD-II.1：严格尾窗与唯一基底

由

\[
b_3=b_1gu<Y=\frac{uF}{\tau}
\]

并约去 \(u>0\)，得到

\[
\boxed{b_1g\tau<F.}
\tag{4.1}
\]

因为 \(b_1\tau\ge1\)，

\[
\boxed{0<g<F.}
\tag{4.2}
\]

对 \(s\) 作关于 \(q\) 的唯一欧几里得除法：

\[
\boxed{
s=s_0+\ell q,\qquad0\le s_0<q.
}
\tag{4.3}
\]

定义

\[
\rho_0=\rho-\ell F.
\tag{4.4}
\]

代入 \(q\rho-Fs=g\)，得

\[
\boxed{q\rho_0-Fs_0=g.}
\tag{4.5}
\]

由右端为正，

\[
\rho_0>0.
\]

又因 \(s_0\le q-1\) 且 \(g<F\)，

\[
q\rho_0=Fs_0+g
<F(q-1)+F=qF,
\]

故

\[
\boxed{0<\rho_0<F.}
\tag{4.6}
\]

如果 \((s_0,\rho_0)\) 与 \((s_0',\rho_0')\) 都满足
(4.5)–(4.6)，则

\[
q(\rho_0-\rho_0')=F(s_0-s_0').
\]

由 \(\gcd(q,F)=1\)，\(q\mid s_0-s_0'\)。结合
\(|s_0-s_0'|<q\)，得到 \(s_0=s_0'\)，继而
\(\rho_0=\rho_0'\)。

因此：

\[
\boxed{
(s_0,\rho_0)\text{ 若存在，则由 }(q,F,g)\text{ 唯一确定}.
}
\tag{4.7}
\]

显式地，

\[
s_0\equiv-gF^{-1}\pmod q,\qquad0\le s_0<q,
\tag{4.8}
\]

\[
\rho_0=\frac{Fs_0+g}{q}.
\tag{4.9}
\]

这里 \(s_0=0\) 没有被删除；它将在 \(q=1\) 中必然出现。

---

## 5. 内容提升

### 5.1 核心引理 CD-II.2：提升指标、互素计数与统一九提升界

由 \(s>0\) 和 \(s<qh\)，(4.3) 中的商满足

\[
\boxed{0\le\ell<h.}
\tag{5.1}
\]

同时

\[
\boxed{
s=s_0+\ell q,\qquad
\rho=\rho_0+\ell F.
}
\tag{5.2}
\]

于是

\[
\boxed{
N=q(Jh+\ell)+s_0.
}
\tag{5.3}
\]

这说明内容提升只有一个共同指标 \(\ell\)；\(s\) 和 \(\rho\)
不是两个彼此独立的提升。

先处理互素门。若 \(d\mid s_0,q\)，由

\[
q\rho_0-Fs_0=g
\]

可得 \(d\mid g\)。结合 \(\gcd(q,g)=1\)，

\[
\gcd(s_0,q)=1.
\tag{5.4}
\]

又因为 \(h\) 是 \(2\)-幂或 \(5\)-幂而 \(\gcd(q,10)=1\)，

\[
\gcd(q,h)=1.
\tag{5.5}
\]

故

\[
\boxed{
\gcd(s,qh)=1
\Longleftrightarrow
\gcd(s_0+\ell q,h)=1.
}
\tag{5.6}
\]

当 \(\ell\) 遍历 \(0,\ldots,h-1\) 时，
\(s_0+\ell q\) 因 (5.5) 遍历模 \(h\) 的全部剩余类。因此互素门
单独恰好放行

\[
\boxed{\varphi(h)}
\tag{5.7}
\]

个提升。具体地：

\[
\boxed{
\begin{array}{c|c}
h&\text{通过互素门的 }\ell\text{ 数}\\ \hline
2^H&2^{H-1}\\
5^H&4\cdot5^{H-1}
\end{array}}
\tag{5.8}
\]

所以只用互素门，不能把“至多 \(h\) 个提升”降成统一常数。

但是加入 \(N\) 为互补纯幂后会发生第二次压缩。由 (5.3) 和
\(0\le\ell<h,\ 0\le s_0<q\)，

\[
\boxed{
Jqh<N<(J+1)qh.
}
\tag{5.9}
\]

固定 \((q,h,J)\)：

- C2 中两个不同的 \(5\)-幂之比至少为 \(5\)，而区间端点之比
  \((J+1)/J\le2\)，故至多有一个 \(5^R\)；
- C5 中两个不同的 \(2\)-幂之比至少为 \(2\)。当 \(J\ge2\) 时
  \((J+1)/J<2\)；当 \(J=1\) 时区间为严格开区间
  \((qh,2qh)\)，也不可能同时容纳 \(M\) 与 \(2M\)。

因此每个 \(J\) 至多产生一个纯幂 \(N\)，而一旦 \(N\) 固定，

\[
\ell=\frac{N-s_0}{q}-Jh
\tag{5.10}
\]

也唯一。由于 \(J\in\{1,\ldots,9\}\)，

\[
\boxed{
\text{固定 }(q,F,g,h)\text{ 后，全部纯内容候选至多有九个提升}.
}
\tag{5.11}
\]

这是一个真正与 \(h\) 无关的统一常数界。它不是参数有限性：
\(q,F,g,h\) 本身仍可无界。

---

## 6. \(q=1\) 分支

### 6.1 核心引理 CD-II.3：指数带与判别式符号门

若 \(q=1\)，则 (4.3)–(4.9) 给出

\[
\boxed{s_0=0,\qquad \rho_0=g.}
\tag{6.1}
\]

由于 \(s>0\)，

\[
1\le\ell<h.
\tag{6.2}
\]

而

\[
N=Jh+\ell.
\tag{6.3}
\]

故 C2 中

\[
\boxed{
J2^H<5^R<(J+1)2^H,\qquad
\ell=5^R-J2^H,
}
\tag{6.4}
\]

C5 中

\[
\boxed{
J5^H<2^R<(J+1)5^H,\qquad
\ell=2^R-J5^H.
}
\tag{6.5}
\]

两个指数带本身都含无限多点：

- 对每个 \(R\ge1\)，取
  \[
  H=\lfloor R\log_2 5\rfloor,
  \]
  即有
  \[
  2^H<5^R<2^{H+1},
  \]
  给出 (6.4) 的 \(J=1\) 点；
- 对每个 \(H\ge1\)，取
  \[
  R=\lceil H\log_2 5\rceil,
  \]
  即有
  \[
  5^H<2^R<2\cdot5^H,
  \]
  给出 (6.5) 的 \(J=1\) 点。

这里 \(\log_2 5\) 为无理数，所以端点等号不会发生。因此不能仅凭
(6.4)–(6.5) 调用线性形式或连分数宣称指数有界；这些条带确实有
无穷多整数点。若要使用线性形式，必须先从 E4、循环或完整球面中
得到另一个非零指数关系。

现在加入完整判别式。\(q=1\) 时循环方程为

\[
\boxed{
g(k-1)=\frac{TY}{u}+\frac Yv
=Y\left(\frac Tu+\frac1v\right).
}
\tag{6.6}
\]

记

\[
C=g(k-1)>0.
\]

则

\[
(k^2-1)g^2=C(C+2g)>C^2.
\tag{6.7}
\]

完整判别式为

\[
\mathcal D
=Y^2(a_1T+10a_2)^2
-(k^2-1)g^2\bigl((ua_1)^2+(va_2)^2\bigr).
\tag{6.8}
\]

若

\[
\frac uv\,a_1\ge10a_2,
\tag{6.9}
\]

则

\[
Cua_1
=Y\left(T+\frac uv\right)a_1
\ge Y(a_1T+10a_2),
\]

结合 (6.7) 可得 \(\mathcal D<0\)。所以任何 \(q=1\) 候选必须满足

\[
\boxed{
\frac uv\,a_1<10a_2.
}
\tag{6.10}
\]

又因

\[
\frac uv=\frac{b_2}{b_1},
\qquad
a_2<\frac T{10},
\qquad
\frac T{b_2}=\frac Nh,
\]

推出

\[
\boxed{
\frac Nh>\frac{a_1}{b_1}.
}
\tag{6.11}
\]

这给出下列统一终端单元删除：

\[
\boxed{
\begin{array}{c|c}
(a_1,b_1)&q=1\text{ 时仍可能的 }J\\ \hline
(1,1)&1,\ldots,9\\
(2,1)&2,\ldots,9\\
(3,1)&3,\ldots,9\\
\vdots&\vdots\\
(8,1)&8,9\\ \hline
(5,2)&2,\ldots,9\\
(7,2)&3,\ldots,9\\
(9,2)&4,\ldots,9\\
(11,2)&5,\ldots,9\\
(13,2)&6,\ldots,9
\end{array}}
\tag{6.12}
\]

例如 \(b_1=2\) 的 A 室中，全部 \(q=1,J=1\) 状态由判别式负性
统一关闭。

但是 (6.11) 对较大的 \(J\) 不产生矛盾，故本轮没有达到 CD3。

---

## 7. C2：纯二进内容

### 7.1 核心引理 CD-III.1：C2 的完整主方程

在 C2 中

\[
\boxed{
h=2^H,\qquad N=5^R,\qquad
e=m-R,\qquad
\tau=2^m5^{m-R}.
}
\tag{7.1}
\]

唯一本原基底和提升方程为

\[
\boxed{
q\rho_0-Fs_0=g,\qquad
0\le s_0<q,\quad0<\rho_0<F,
}
\tag{7.2}
\]

\[
\boxed{
5^R=q(J2^H+\ell)+s_0,\qquad
0\le\ell<2^H,
}
\tag{7.3}
\]

\[
\boxed{
\gcd(s_0+\ell q,2^H)=1.
}
\tag{7.4}
\]

#### C 行

\[
\boxed{
b_1=2,\quad v=1,\quad c=m,\quad H=1,\quad F=Y.
}
\tag{7.5}
\]

循环方程化为

\[
\boxed{
g(kq-1)=Y(5^R+q).
}
\tag{7.6}
\]

并且

\[
\eta=v_2(5^R+q),
\qquad
a+\lambda=n+\eta.
\tag{7.7}
\]

其余仍是 E4 的 C1、C2、C3：

\[
\begin{array}{c|l}
\mathrm{C1}&
\lambda<2\eta+1,\quad2a>n,\quad a+\lambda=n+\eta;\\
\mathrm{C2}&
a\ge\eta+2,\quad\lambda=2a-1,\quad n=3a-1-\eta;\\
\mathrm{C3}&
a=\eta+1,\quad\lambda=2a-1,\quad n=2a,\quad\kappa=1.
\end{array}
\tag{7.8}
\]

#### D 行

若 \(b_1=1\)，则 \(H=j\)；若 \(b_1=2\)，则 \(H=j+1\)。两行都有

\[
\boxed{
c=m+j,\qquad F=2^{n-j}5^n.
}
\tag{7.9}
\]

循环方程在两行中统一为

\[
\boxed{
g(kq-1)=F(5^R+q2^j).
}
\tag{7.10}
\]

E4 只剩

\[
\boxed{
\begin{array}{c|c|c}
\text{室}&\lambda&n\\ \hline
\mathrm{D1}&1&j+a+1\\
\mathrm{D2}&2a-1&j+3a-1
\end{array}
\qquad a\ge2.
}
\tag{7.11}
\]

令

\[
\mu=v_5(kq-1)\ge0.
\tag{7.12}
\]

因为 \(5^R+q\not\equiv0\pmod5\) 且
\(5^R+q2^j\not\equiv0\pmod5\)，(7.6)、(7.10) 都给出

\[
\boxed{\varphi+\mu=n.}
\tag{7.13}
\]

完整球面—拼接判别式在 C2 中为

\[
\boxed{
\begin{aligned}
w^2={}&
Y^2(a_1T+10a_2)^2\\
&-(k^2-1)g^2
\left(
\bigl(2^c5^{m-R}a_1\bigr)^2+a_2^2
\right),
\end{aligned}}
\tag{7.14}
\]

\[
\boxed{
a_3=\frac{Y(a_1T+10a_2)\pm kw}{k^2-1}
\in\mathbb Z_{>0}.
}
\tag{7.15}
\]

还必须保留

\[
Y\le a_3<10Y,\qquad
\gcd(a_1,b_1)=\gcd(a_2,b_2)=\gcd(a_3,b_3)=1.
\tag{7.16}
\]

#### D1、D2 前置门反例攻击

内容方程、窗口、K5 支撑和 E4 本身不能关闭 D1 或 D2。以下给出
两个无界辅助族；它们不是原题解，只证明关闭必须真正使用
(7.14)–(7.16)。

固定

\[
b_1=v=q=1,\qquad
j=R=H=1,\qquad
J=2,\qquad
s_0=0,\quad\ell=1.
\tag{7.17}
\]

于是

\[
5=2\cdot2+1.
\]

对 D1，任取 \(a\ge2\)，令

\[
n=a+2,\qquad
g=2^a5,\qquad
k=1+14\cdot5^{a+1}.
\tag{7.18}
\]

选择唯一整数 \(m\) 满足

\[
\frac1{10}\le
2^{m-1}5^{m-a-2}<1,
\tag{7.19}
\]

并令

\[
e=m-1,\qquad
c=m+1,\qquad
u=2^{m+1}5^{m-1}.
\tag{7.20}
\]

(7.19) 的区间在取对数后长度恰为 \(1\)，故该 \(m\) 唯一；
且 \(a\ge2\) 时 \(m\ge3\)。直接核对：

\[
\frac{b_2}{T}=\frac25,
\qquad
\frac{b_3}{Y}=2^{m-1}5^{m-a-2}\in[1/10,1),
\tag{7.21}
\]

\[
g(k-1)=2^{a+1}5^{a+2}(2+5),
\qquad
v_2(k-1)=1.
\tag{7.22}
\]

所以这是无界的 D1 前置门辅助族。

对 D2，仍取 (7.17)，任取 \(a\ge2\)，令

\[
n=3a,\qquad
g=2^a5,\qquad
k=1+7\cdot2^{2a-1}5^{3a-1}.
\tag{7.23}
\]

选择唯一整数 \(m\) 满足

\[
\frac1{10}\le
2^{m+1-2a}5^{m-3a}<1,
\tag{7.24}
\]

并仍令 \(e=m-1,c=m+1\)。则

\[
\frac{b_2}{T}=\frac25,\qquad
\frac{b_3}{Y}\in[1/10,1),
\tag{7.25}
\]

\[
v_2(k-1)=2a-1.
\tag{7.26}
\]

这给出无界的 D2 前置门辅助族。

这两个族也不被第 6 节的粗判别式符号门自动删除：取合法首块
\(a_1=1\)，并令

\[
a_2=5\cdot10^{m-2}+1.
\tag{7.27}
\]

则 \(a_2\) 位于真实中分子窗口内，且因 \(b_2=u\) 是
\((2,5)\)-平滑数而有 \(\gcd(a_2,b_2)=1\)。同时

\[
10a_2>\frac25T=u=\frac uv\,a_1.
\tag{7.28}
\]

所以 (6.10) 也通过；真正未解决的是 (7.14) 的平方性、(7.15)
的整性及第三块恢复。

因此本轮没有关闭 D1 或 D2；也不能在 \(a,m\) 未控制时对
(7.14) 作有限搜索并升级为全局结论。

---

## 8. C5：纯五进内容

### 8.1 核心引理 CD-III.2：C5 的完整主方程与严格内容界

在 C5 中

\[
\boxed{
h=5^H,\qquad N=2^R,\qquad
e=m+H,\qquad
x=m-R.
}
\tag{8.1}
\]

本原基底与提升为

\[
\boxed{
q\rho_0-Fs_0=g,\qquad
0\le s_0<q,\quad0<\rho_0<F,
}
\tag{8.2}
\]

\[
\boxed{
2^R=q(J5^H+\ell)+s_0,\qquad
0\le\ell<5^H,
}
\tag{8.3}
\]

\[
\boxed{
\gcd(s_0+\ell q,5^H)=1.
}
\tag{8.4}
\]

三种位置为

\[
\boxed{
\begin{array}{c|c|c|c}
\text{位置}&(b_1,v,c)&R&F\\ \hline
\mathrm A&(2,2,0)&m&2^n5^{n-H}\\
\mathrm B&(1,1,c<m)&m-c&2^n5^{n-H}\\
\mathrm B&(2,1,c\le m-2)&m-c-1&2^{n+1}5^{n-H}
\end{array}}
\tag{8.5}
\]

统一的循环方程是

\[
\boxed{
g(kq-1)
=\frac F{b_1}\left(b_1\,2^R+q5^H\right).
}
\tag{8.6}
\]

括号满足

\[
b_1\,2^R+q5^H\not\equiv0\pmod5.
\tag{8.7}
\]

令

\[
\mu=v_5(kq-1)\ge0.
\]

比较 (8.6) 的五进赋值，得到

\[
\boxed{\varphi+\mu=n-H.}
\tag{8.8}
\]

由于 \(e=m+H>0\)，素数 \(5\) 整除 \(u\)。又因
\(\operatorname{rad}(u)\mid qg\) 且 \(5\nmid q\)，必有

\[
\varphi=v_5(g)\ge1.
\tag{8.9}
\]

所以

\[
\boxed{
H\le n-1.
}
\tag{8.10}
\]

这严格删除了此前只由 \(F\in\mathbb Z\) 允许的边界 \(H=n\)。
但 \(n\) 仍可无界，所以 (8.10) 不是 CD4 意义下的绝对内容上界。

E4 的关系原样保留：

\[
\boxed{
\begin{array}{c|l}
\mathrm{A1}&a\ge2,\ \lambda=1,\ n=a+2;\\
\mathrm{A2}&a\ge2,\ \lambda=2a-1,\ n=3a;\\
\mathrm B,\ 0<c<m&
a\ge2,\ \lambda=1\text{ 或 }2a-1;\\
\mathrm B,\ c=0,b_1=2&
\lambda=1\text{ 或 }2a;\\
\mathrm B,\ c=0,b_1=1&
\text{保留 }e_1,e_2,h_B,\varepsilon_B\text{ 的共振系统}.
\end{array}}
\tag{8.11}
\]

完整判别式为

\[
\boxed{
\begin{aligned}
w^2={}&
Y^2(a_1T+10a_2)^2\\
&-(k^2-1)g^2
\left(
\bigl(2^c5^{m+H}a_1\bigr)^2+(va_2)^2
\right),
\end{aligned}}
\tag{8.12}
\]

\[
\boxed{
a_3=\frac{Y(a_1T+10a_2)\pm kw}{k^2-1}
\in\mathbb Z_{>0},
}
\tag{8.13}
\]

再联合真实窗口和逐项既约。

本轮没有从 (8.8)、E4 的 \(n=a+\lambda\) 型关系及
\(H\le n-1\) 推出 \(H\) 的绝对上界。A、B 各室仍可随
\(a,\lambda,n\) 同步增长。

---

## 9. 完整判别式与反例攻击

### 9.1 核心引理 CD-III.3：判别式的能力边界

对 C2、C5，完整必要条件统一为

\[
\boxed{
\mathcal S
=g^2\bigl((ua_1)^2+(va_2)^2\bigr),
}
\tag{9.1}
\]

\[
\boxed{
H_1=a_1T+10a_2,
}
\tag{9.2}
\]

\[
\boxed{
\mathcal D=Y^2H_1^2-(k^2-1)\mathcal S=w^2,
}
\tag{9.3}
\]

\[
\boxed{
a_3=\frac{YH_1\pm kw}{k^2-1}
\in\mathbb Z_{>0}.
}
\tag{9.4}
\]

判别式平方不是充分条件；还必须核对 (9.4)、第三块窗口、球面恢复和
三个逐项既约条件。

### 9.2 C5 中一个无界 E4 辅助族及其统一排除

指数带与 E4 前置门确实可以同时存在无界族。固定

\[
q=1,\quad b_1=v=2,\quad
H=1,\quad m=3,\quad e=4,
\tag{9.5}
\]

\[
u=625,\quad N=8,\quad J=1,\quad\ell=3.
\tag{9.6}
\]

对任意奇数 \(a\ge5\)，令

\[
n=a+2,\qquad
g=3\cdot2^a5^{a-3},\qquad
k=8751.
\tag{9.7}
\]

则

\[
\frac{b_2}{T}=\frac58,\qquad
\frac{b_3}{Y}=\frac3{10},
\tag{9.8}
\]

\[
g(k-1)=\frac{TY}{u}+\frac Y2,
\qquad
v_2(k-1)=1.
\tag{9.9}
\]

而 A1 的高阶参数满足

\[
\theta_A=2.
\tag{9.10}
\]

证明 (9.10)：在 \(\theta_A\) 的括号中，后两项被 \(16\) 整除；
前两项约去奇数 \(5^4\) 后为

\[
99\cdot5^n-3.
\]

因 \(n=a+2\) 为奇数，

\[
99\cdot5^n-3\equiv4\pmod8.
\]

所以其二进赋值恰为 \(2\)，正好命中 E4 对 \(a\ge3\) 的 A1 门。

该族因此满足 C5、\(q=1\)、真实分母窗口、K5 支撑、循环和 E4
高阶门，但它不是原题解。事实上它有 \(J=1,b_1=2\)，而
(6.11) 要求

\[
\frac Nh>\frac{a_1}{b_1}\ge\frac52.
\]

这里 \(N/h=8/5<2\)，矛盾。因此完整判别式对整个族统一为负。

这个例子同时说明两点：

1. 指数带、窗口和 E4 兼容并不意味着原题候选存在；
2. 完整判别式确实能统一关闭某些无界辅助族，但当前符号门只关闭
   \(q=1\) 的一批低 \(J\) 单元，不能覆盖全部 C2、C5。

### 9.3 为什么没有达到 CD1–CD5

1. C2 的 D1、D2 辅助族 (7.17)–(7.26) 通过全部分母与 E4
   前置门；本轮没有证明其完整判别式对所有分子块统一非平方或为负。
2. C5 的 (8.8) 只给 \(H\le n-1\)，没有给绝对上界。
3. \(q=1\) 的低 \(J\) 单元被 (6.11) 删除，但较大 \(J\) 仍开放。
4. 判别式系数仍随 \(q,g,H,R,m,n,a\) 移动，尚未化为有限多个
   系数固定的曲线。
5. 因指数仍无界，没有使用有限搜索支持任何全局关闭。

### 9.4 主动审计

1. **是否真的有 \(\gcd(N,h)=1\)：**  
   有。第 2 节分别使用
   \[
   \alpha=\min(m,x),\qquad\beta=\min(m,e)
   \]
   证明 \(2\) 和 \(5\) 都不可能同时整除 \(N,h\)。

2. **是否使用 \(N>h\) 排除 \(N=1\)：**  
   是。式 (2.4) 来自 \(N=Jqh+s\) 与 \(s\ge1\)，并在三分法中
   排除了 \(N=1\)。

3. **是否错误允许 \(h\) 同时含 \(2,5\)：**  
   没有。若 \(2,5\mid h\)，互素性迫使 \(N=1\)，与 \(N>h\)
   矛盾。

4. **是否把 \(e=m\) 放入 C2：**  
   没有。C2 使用严格条件 \(e<m\)；边界 \(e=m\) 会给 \(N=1\)。

5. **是否把 \(x=m\) 放入 C5：**  
   没有。C5 使用严格条件 \(x<m\)；C 的 \(b_1=1\) 边界和 B 的
   二进饱和边界均已删除。

6. **是否遗漏 \(s_0=0,q=1\)：**  
   没有。第 6 节保留
   \[
   s_0=0,\qquad\rho_0=g,
   \]
   并由 \(s>0\) 推出 \(1\le\ell<h\)。

7. **是否由 \(g<F\) 正确推出 \(0<\rho_0<F\)：**  
   是。下界来自 \(q\rho_0=Fs_0+g>0\)；上界使用
   \(s_0\le q-1\) 与严格不等式 \(g<F\)。

8. **是否把内容提升误写成两个独立指标：**  
   没有。式 (5.2) 中 \(s,\rho\) 共用同一个 \(\ell\)，并由
   (5.3) 与纯幂窗口进一步压到统一至多九个。

9. **是否在指数尚未控制时使用有限搜索：**  
   没有。D1、D2 的无界辅助族只作符号核对；没有用任何有限枚举
   排除它们或升级全局结论。

10. **是否把判别式平方误写成完整候选：**  
    没有。全文同时保留 (9.4)、第三块窗口、球面恢复和逐项既约；
    (9.3) 始终只是必要条件。

---

## 10. 最终分类 CD1–CD6

本轮达到

\[
\boxed{
\mathrm{CD6}:
\quad
\text{得到严格纯内容结构及统一九提升界，但未关闭完整纯内容分支}.
}
\tag{10.1}
\]

决定性新链条为

\[
\boxed{
\begin{gathered}
\alpha=\min(m,x),\quad\beta=\min(m,e)\\
\Longrightarrow \gcd(N,h)=1;\\
N=Jqh+s>h\\
\Longrightarrow
h>1\text{ 时只可能为 C2 或 C5};\\
q\rho-Fs=g,\quad0<g<F\\
\Longrightarrow
(s_0,\rho_0)\text{ 唯一};\\
N\in(Jqh,(J+1)qh),\quad N\text{ 为互补纯幂}\\
\Longrightarrow
\text{每个 }J\text{ 至多一个提升，总计至多九个};\\
\mathrm{C5}+\operatorname{rad}(u)\mid qg\\
\Longrightarrow
v_5(g)+v_5(kq-1)=n-H,\quad H\le n-1.
\end{gathered}}
\tag{10.2}
\]

为什么不是 CD1：

- C2、C5 都仍有开放状态。

为什么不是 CD2：

- 没有关闭 C2 或 C5 中任何一个完整纯内容分支。

为什么不是 CD3：

- 只关闭了 (6.12) 所列的 \(q=1\) 低 \(J\) 单元；其余
  \(q=1\) 状态尚未统一排除。

为什么不是 CD4：

- \(H\le n-1\) 是相对界，不是绝对有效上界；
- \(m,n,a,e,j,\eta\) 仍可无界。

为什么不是 CD5：

- 九提升界固定的是每个移动基底上的提升数；
- \((q,F,g,h)\) 和判别式系数仍可无界变化，尚未得到有限多个固定曲线。

为什么只能列为 CD6：

- 三分法、唯一基底、精确提升计数和九提升界都是覆盖全部 \(h>1\)
  的严格结构；
- 但 D1、D2 的无界前置门辅助族证明，这些结构还没有跨越完整
  球面—拼接障碍。

没有找到合法原题解。

---

## 11. \(G\) 的最新剩余系统

结合 VA1、GD1、GP3 与本报告，临界 \(G\) 正余数层分为：

### 11.1 本原层

\[
\boxed{
h=1,\qquad
\tau=\frac{b_1u}{v}.
}
\tag{11.1}
\]

本轮未研究。

### 11.2 C2

\[
\boxed{
\begin{gathered}
h=2^H,\quad N=5^R,\quad H,R\ge1,\\
x>m,\quad e<m,\\
\text{仅位于 C 的 }(b_1=2)\text{ 行或 D 的 }(b_1=1,2)\text{ 行},\\
5^R=q(J2^H+\ell)+s_0,\\
q\rho_0-Fs_0=g,\quad
0\le s_0<q,\quad0<\rho_0<F,\\
0\le\ell<2^H,\quad
\gcd(s_0+\ell q,2^H)=1.
\end{gathered}}
\tag{11.2}
\]

还必须联合 (7.6) 或 (7.10)、E4 的 C1–C3 或 D1–D2，以及
完整判别式 (7.14)–(7.16)。

### 11.3 C5

\[
\boxed{
\begin{gathered}
h=5^H,\quad N=2^R,\quad H,R\ge1,\\
e=m+H,\quad x=m-R<m,\\
H\le n-1,\\
\text{仅位于 A 或 B 的非二进饱和行},\\
2^R=q(J5^H+\ell)+s_0,\\
q\rho_0-Fs_0=g,\quad
0\le s_0<q,\quad0<\rho_0<F,\\
0\le\ell<5^H,\quad
\gcd(s_0+\ell q,5^H)=1,\\
v_5(g)+v_5(kq-1)=n-H.
\end{gathered}}
\tag{11.3}
\]

还必须联合 E4 的 A1、A2、B 各室及共振参数，以及
(8.12)–(8.13)。

### 11.4 统一剩余门

所有 \(h>1\) 状态均满足：

\[
\boxed{
\begin{gathered}
J\in\{1,\ldots,9\},\qquad
\gcd(q,10)=\gcd(q,F)=\gcd(q,g)=1,\\
(s_0,\rho_0)\text{ 由 }(q,F,g)\text{ 唯一确定},\\
\text{固定 }(q,F,g,h)\text{ 后至多九个提升},\\
\text{十三种首块、真实分母与分子窗口、逐项既约},\\
\mathcal D=w^2,\qquad
a_3=\frac{YH_1\pm kw}{k^2-1}\in\mathbb Z_{>0}.
\end{gathered}}
\tag{11.4}
\]

对 \(q=1\) 还必须满足

\[
\boxed{
\frac Nh>\frac{a_1}{b_1},
}
\tag{11.5}
\]

故 (6.12) 的全部低 \(J\) 单元已删除。

当前仍未控制

\[
\boxed{
H,\ q,\ F,\ g_0,\ m,\ n,\ a,\ e,\ j,\eta,
\theta_A,\theta_B,\kappa
}
\tag{11.6}
\]

中的无界移动系数系统。准确停止点是：

\[
\boxed{
\begin{gathered}
\text{非本原内容已严格二分为 C2、C5；}\\
\text{本原基底唯一，实际提升数统一至多九个；}\\
\text{C5 有 }H\le n-1\text{，}q=1\text{ 有新的判别式低 }J\text{ 删除；}\\
\text{但 C2 的 D1、D2 及 C5 的较高 }J\text{ 状态仍开放；}\\
\text{故最终分类为 CD6，而不是 CD1–CD5。}
\end{gathered}}
\]

全文到此停止；不研究本原层 \(h=1\)、O 或 Q。
