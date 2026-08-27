# 三项十进制拼接平方和问题：临界 (G) 模板 A1 单位行列式战役

日期：2026-08-01（Asia/Tokyo）

最终分类：

\[
\boxed{
\mathrm{GA1\text{-}3}
}
\]

并附带一个严格强于“只得到相对窗口”的终端结果：本文给出全部剩余对象的
双向终端因子正规形、完整归一化曲线索引和低层 (E\le4) 的独立有限证书。
高层仍含无界偶参数 (E=e+\delta\)，故不能把结果误报为 GA1-2 的有限
种子表，也不能启动一个只覆盖有限 (E) 的周期证书并外推到全体。

本文只处理

\[
\boxed{
G_{\mathrm{prim}},\qquad h=1,\qquad \gamma=1,\qquad \mathrm{A1}.
}
\]

不研究 (\gamma>1)、A2、B、C、非本原 C2/C5、(Q) 或严格层。

---

## 1. SD6 后的 (G) 状态

按任务约定，暂时接受 T1–T18、K5、CG、E4、GT4、VA1、GD1、GP3、
CD6、PR6 和 SD6，不作全项目统一独立审计。A 室满足

\[
b_1=v=2,\qquad c=0,\qquad u=5^e,
\]

\[
T=10^m,\qquad Y=10^n,\qquad m\ge2,
\]

\[
N=2^m5^{m-e},\qquad e\le m,
\]

\[
b_2=q5^e,\qquad b_3=2g5^e.
\]

本原正余数正规形为

\[
N=Jq+s,\qquad 1\le s<q,\qquad J\in\{1,\ldots,9\},
\]

\[
q\rho_0-E_0s=\gamma,
\qquad
qM_0-E_0N=\gamma.
\]

本轮严格取

\[
\gamma=1,\qquad g=d=\gcd(g,Y),
\qquad g=2^a5^\varphi.
\]

这不是把“原奇核心 (g_*=1)”误当成充分条件；这里直接保留 PR6 的
约化行列式定义并显式要求 (g=d)。A1 给出

\[
a\ge2,\qquad \lambda=v_2(kq-1)=1,\qquad n=a+2,
\]

以及

\[
\theta_A=
\begin{cases}
3,&a=2,\\
2,&a\ge3.
\end{cases}
\]

仍须保留 K5 支撑

\[
\operatorname{rad}(u)\mid qg,
\]

分母窗口、十三首块、真实中分子窗口、第三块窗口和三个逐项既约条件。

---

## 2. A1 单位行列式系统

由 PR6，

\[
E_0=2Z,\qquad M_0=k-Z,
\qquad Z=\frac{Y}{2d}.
\]

代入

\[
qM_0-E_0N=1
\]

得到

\[
q(k-Z)=2ZN+1.
\tag{2.1}
\]

定义

\[
r=k-Z.
\]

则

\[
\boxed{qr=2ZN+1.}
\tag{2.2}
\]

另一方面

\[
M_0=2JZ+\rho_0,\qquad 0<\rho_0<2Z,
\]

所以

\[
\boxed{2JZ<r<2(J+1)Z.}
\tag{2.3}
\]

由于 (2ZN+1\) 与 (10) 互素，任一因子对自动满足

\[
\boxed{\gcd(q,10)=\gcd(r,10)=1.}
\tag{2.4}
\]

式 (2.1)–(2.3) 的正向推导无误；第 5 节给出完整恢复方向。

---

## 3. A1 尾窗二值化

由

\[
b_3=2^{a+1}5^{\varphi+e},\qquad n=a+2,
\]

有

\[
\frac{b_3}{Y}
=2^{a+1-n}5^{\varphi+e-n}
=\frac12\,5^{\varphi+e-n}.
\]

分母尾窗

\[
\frac{Y}{10}\le b_3<Y
\]

等价于

\[
\frac15\le5^{\varphi+e-n}<2.
\]

整数指数只能为 (-1) 或 (0)，故

\[
\boxed{\varphi+e\in\{n-1,n\}.}
\tag{3.1}
\]

定义

\[
\delta=n-(\varphi+e)\in\{0,1\},
\qquad
E=e+\delta,
\qquad
A=5^E,
\qquad
B=5^\delta.
\tag{3.2}
\]

则

\[
\varphi=n-E,
\qquad
d=g=2^{n-2}5^{n-E},
\tag{3.3}
\]

并且

\[
\boxed{Z=2A=2\cdot5^{e+\delta}.}
\tag{3.4}
\]

又因

\[
N=2^m5^{m-e}=\frac{B10^m}{A},
\]

所以

\[
\boxed{2ZN=4B10^m.}
\tag{3.5}
\]

终端因子严格二值化为

\[
\boxed{qr=1+4B10^m,\qquad B\in\{1,5\}.}
\tag{3.6}
\]

即

\[
qr=4\cdot10^m+1
\]

或

\[
qr=20\cdot10^m+1.
\]

尾分母还简化为

\[
b_3=2d5^e=
\begin{cases}
Y/2,&\delta=0,\\
Y/10,&\delta=1.
\end{cases}
\tag{3.7}
\]

所以完整候选必有

\[
\gcd(a_3,10)=1.
\tag{3.8}
\]

---

## 4. 终端因子分解与严格窗口

第二分母窗口给出

\[
\frac{N}{10}\le q<N.
\tag{4.1}
\]

由 (2.3)、(3.4)，

\[
\boxed{4JA<r<4(J+1)A.}
\tag{4.2}
\]

因此每个终端状态先由

\[
(\delta,J,e,r,m)
\]

给出，其中

\[
r\mid1+4B10^m,
\qquad
4JA<r<4(J+1)A.
\]

对固定 ((\delta,J,e,r))，因 (gcd(r,10)=1)，指数整数性为

\[
\boxed{
10^m\equiv-(4B)^{-1}\pmod r.
}
\tag{4.3}
\]

若 (4.3) 有解，令

\[
M_r=\operatorname{ord}_r(10).
\]

乘法子群内离散对数唯一，所以全部解至多是一类

\[
\boxed{m\equiv m_0\pmod{M_r}.}
\tag{4.4}
\]

这里没有把“固定 (r) 的唯一指数类”错误提升为“全体 (r) 已有限化”。

实际初端门也可精确写出。由

\[
q=\frac{1+4B10^m}{r},\qquad
N=\frac{B10^m}{A},
\]

条件 (s=N-Jq>0) 等价于

\[
\boxed{
B10^m(r-4JA)>JA.
}
\tag{4.5}
\]

而 (q\ge3) 等价于

\[
\boxed{1+4B10^m\ge3r.}
\tag{4.6}
\]

一旦 (4.2)、(4.5) 成立，(s<q) 自动成立；(4.1) 的下端也由

\[
r<4(J+1)A\le40A
\]

自动满足。因此固定 ((\delta,J,e,r)) 后，全部实际指数恰为

\[
\boxed{m=m_*+\ell M_r,\qquad \ell\ge0,}
\tag{4.7}
\]

其中 (m_*) 是同余类中第一个同时满足

\[
m\ge\max(2,e),\qquad (4.5),\qquad (4.6)
\]

的指数。

---

## 5. 双向恢复

固定一个满足 (3.6)、(4.2) 和实际初端门的五元组

\[
(\delta,J,e,r,m).
\]

定义

\[
\boxed{
q=\frac{1+4B10^m}{r},
\qquad
k=r+2A,
}
\tag{5.1}
\]

\[
\boxed{
s=N-Jq,
\qquad
\rho_0=r-4JA.
}
\tag{5.2}
\]

严格窗口给出

\[
0<\rho_0<4A=2Z.
\]

又由 (3.6)，

\[
\begin{aligned}
q\rho_0-4As
&=q(r-4JA)-4A(N-Jq)\\
&=qr-4AN\\
&=1.
\end{aligned}
\tag{5.3}
\]

所以

\[
q\rho_0-2Zs=1.
\]

同时 (N=Jq+s)，且实际初端门保证 (1\le s<q)。因此

\[
\boxed{
(\delta,J,e,r,m)
\longleftrightarrow
(q,r,s,\rho_0,J,k)
}
\]

在上述门内是双向且唯一的；没有额外的 (s,\rho_0,J,k) 分支。

---

## 6. A1 高阶参数的终端化

E4 中

\[
\theta_A=v_2\!\left(
99q^2 5^{e+n}-q5^{\varphi+e}
-2^{m+1}5^{\varphi+m}
-2^{m+2}q5^{m+n}
\right).
\]

由

\[
\varphi+e=n-\delta,
\qquad
qr=1+4B10^m,
\]

提出奇因子 (5^{n-\delta}) 后，括号严格化为

\[
\boxed{
\Theta=q^2(99A-r)-2N.
}
\tag{6.1}
\]

因此

\[
\theta_A=v_2(\Theta).
\]

对 (m\ge3)，有 (v_2(2N)=m+1\ge4)，而 (q) 为奇数。所以 A1
所需的低赋值完全终端化为

\[
\boxed{
\theta_A=2\iff v_2(99A-r)=2,
}
\tag{6.2}
\]

\[
\boxed{
\theta_A=3\iff v_2(99A-r)=3.
}
\tag{6.3}
\]

唯一需要直接计算的低层例外是 (m=2)。此时 (v_2(2N)=3)：

- 若 (v_2(99A-r)=2)，则 (	heta_A=2)；
- 若 (v_2(99A-r)>3)，则 (	heta_A=3)；
- 若两项同为赋值 (3)，必须保留真实消去，不能取最小值。

这给出固定终端种子的完整 A1 指数门，而不是小模筛选率。

---

## 7. 五进尺度锁定

这是本轮越过 SD6 停止点的主要新引理。

### 引理 7.1

设 (e>0)，并假设一个终端状态能通过完整判别式平方与 SD6 尺度恢复。
令

\[
K=k^2-1,
\qquad
\beta=v_5(K).
\]

则

\[
\boxed{
\beta\ge2\text{ 且为偶数},
\qquad
\varphi=\frac\beta2,
\qquad
n=E+\frac\beta2.
}
\tag{7.1}
\]

#### 证明

归一化判别式为

\[
w_0^2=(4AH_1)^2-K\bigl((5^ea_1)^2+(2a_2)^2\bigr),
\tag{7.2}
\]

其中

\[
H_1=a_1T+10a_2.
\]

因为 (e>0)，第二分母 (b_2=q5^e) 被 (5) 整除。逐项既约给出

\[
5\nmid a_2.
\]

又因 (m\ge2)，

\[
v_5(H_1)=1.
\]

三项的五进赋值分别为

\[
2E+2,
\]

\[
\beta+2e+2v_5(a_1)>\beta,
\]

\[
\beta.
\]

由 (r<40A) 和 (k=r+2A)，

\[
k<42A.
\]

若 (5^\beta\mid K)，则 (5^\beta\mid k-1) 或 (k+1)，故

\[
5^\beta\le k+1<43\cdot5^E<5^{E+3}.
\]

于是

\[
\beta\le E+2<2E+2.
\]

所以 (7.2) 中第三项具有唯一最低五进赋值，

\[
v_5(w_0^2)=\beta.
\]

因此 (eta) 为偶数，且

\[
v_5(w_0)=\frac\beta2.
\]

定义

\[
L_\pm=4AH_1\pm kw_0.
\]

因为

\[
v_5(4AH_1)=E+1>\frac\beta2,
\]

两个符号都满足

\[
v_5(L_\pm)=\frac\beta2.
\]

SD6 的精确尺度恢复为

\[
d=\frac{K}{\gcd(K,L_\varepsilon)}.
\]

所以

\[
v_5(d)=\beta-\min\!\left(\beta,\frac\beta2\right)=\frac\beta2.
\]

而 (3.3) 给出

\[
v_5(d)=n-E=\varphi.
\]

故

\[
\varphi=\frac\beta2,
\qquad
n=E+\frac\beta2.
\]

最后，K5 在 (e>0) 时要求 (5\mid g)，所以 (arphi\ge1)，即

\[
\beta\ge2.
\]

证毕。

### 推论 7.2

对 (e>0)，(n,\varphi,d) 已不再是移动自由度，而由终端整数 (k)
唯一确定：

\[
\boxed{
n=E+\frac{v_5(k^2-1)}2,
}
\]

\[
\boxed{
d=2^{E+v_5(k^2-1)/2-2}
5^{v_5(k^2-1)/2}.
}
\tag{7.3}
\]

仍须检查

\[
v_2(K)\ge n-2.
\tag{7.4}
\]

---

## 8. 高层偶参数定理与低层有限证书

### 8.1 高层偶参数定理

设 (e>0) 且 (E\ge5)。由引理 7.1，

\[
n\ge E+1.
\]

又由 (d\mid K)，

\[
v_2(K)\ge n-2\ge E-1.
\]

对奇数 (k)，(k-1,k+1) 中一个的二进赋值恰为 (1)。因此存在
唯一 (sigma\in\{\pm1\}) 使

\[
k\equiv\sigma\pmod{2^{E-2}}.
\tag{8.1}
\]

此时 (m\ge e=E-\delta\ge4)，故 A1 要求

\[
v_2(99A-r)=2.
\]

利用 (r=k-2A)，左边为

\[
v_2(101A-k).
\]

若 (sigma=-1)，则模 (8)

\[
101A-k\equiv101\cdot5^E+1\equiv2\text{ 或 }6\pmod8,
\]

赋值只能为 (1)，矛盾。故 (sigma=1)。此时

\[
101A-k\equiv101\cdot5^E-1\pmod8.
\]

当 (E) 为偶数时右边为 (4\pmod8)；当 (E) 为奇数时右边为
(0\pmod8)。所以

\[
\boxed{
E\ge5
\Longrightarrow
E\text{ 为偶数},
\qquad
k\equiv1\pmod{2^{E-2}}.
}
\tag{8.2}
\]

特别地，高层只可能有

\[
\boxed{E=6,8,10,\ldots.}
\tag{8.3}
\]

再由 (k<42A)，

\[
\boxed{
2\le\beta=v_5(K)\le E+2,
\qquad \beta\equiv0\pmod2.
}
\tag{8.4}
\]

### 8.2 (E\le4) 的完整有限证书

对 (E\le4)，严格窗口中的 (r) 属于有限集合。独立生成器枚举：

1. (delta\in\{0,1\})、(e\ge0)、(E=e+\delta\le4)；
2. (J\in\{1,\ldots,9\})；
3. 全部整数 (4JA<r<4(J+1)A) 且 (gcd(r,10)=1)；
4. 完整乘法子群门 (4.3)；
5. A1 的真实 (m=2) 例外及 (m\ge3) 尾门；
6. K5、引理 7.1 和 (d\mid K) 的必要尺度门；
7. 实际单调初端 (4.5)–(4.6)。

独立验证器不用生成器的乘法循环函数，而由 (arphi(r)) 分解计算
(\operatorname{ord}_r(10))，重新枚举离散对数并比较完整规范集合。

结果只有两条低层终端指数级数：

| (delta) | (e) | (E) | (J) | (r) | (k) | (v_2(K)) | (v_5(K)) | (n) | 指数级数 |
|---:|---:|---:|---:|---:|---:|---:|---:|---:|---|
| 0 | 3 | 3 | 4 | 2251 | 2501 | 3 | 4 | 5 | (m=2229+2250\ell) |
| 1 | 2 | 3 | 4 | 2251 | 2501 | 3 | 4 | 5 | (m=551+2250\ell) |

两条都满足

\[
d=2^3 5^2=200.
\]

规范 CSV 的 SHA-256 为

```text
afb06541c03dd8a7015487cb16fd85ccd74cf406f230a135a9e5f6b4ff38cf5a
```

生成器与验证器的 SHA-256 分别为

```text
ebfa696336751071e8bf13353f3d8be8f81d6b5b58cead16d976107e2a4f7f0b
a48bb1dbb99c4f7cb3c6235f79f7c35e1f1ad2a49102dc9e273916b6581628e9
```

验证输出为

```text
verified complete low-E certificate: 2 rows
```

这两条是“通过终端、A1、K5 和必要尺度门”的曲线种子，不是原题解，
也没有被提升为判别式平方存在声明。

---

## 9. 归一化判别式与完整剩余曲线

本节给出题设第 4 项意义下的完整符号曲线表。

### 9.1 终端种子索引

定义低层索引集 (mathscr S_{\mathrm{lo}}) 为第 8.2 节的两行。

定义高层索引集 (mathscr S_{\mathrm{hi}}) 为全部

\[
\mathfrak s=(\delta,e,E,J,r,k,\beta,n,m_*,M_r)
\]

满足：

\[
\delta\in\{0,1\},
\qquad
E=e+\delta\in\{6,8,10,\ldots\},
\tag{9.1}
\]

\[
4J5^E<r<4(J+1)5^E,
\qquad
J\in\{1,\ldots,9\},
\qquad
\gcd(r,10)=1,
\tag{9.2}
\]

\[
k=r+2\cdot5^E,
\qquad
k\equiv1\pmod{2^{E-2}},
\tag{9.3}
\]

\[
\beta=v_5(k^2-1)\in2\mathbb Z,
\qquad
2\le\beta\le E+2,
\tag{9.4}
\]

\[
n=E+\frac\beta2,
\qquad
v_2(k^2-1)\ge n-2,
\tag{9.5}
\]

以及 (4.3) 有解，并以 (4.5)–(4.6) 取唯一实际尾类

\[
m=m_*+\ell M_r,qquad \ell\ge0.
\tag{9.6}
\]

令

\[
\mathscr S=\mathscr S_{\mathrm{lo}}\cup\mathscr S_{\mathrm{hi}}.
\]

### 9.2 固定 Pell–几何级数曲线

固定 (mathfrak s\in\mathscr S)、

\[
a_1\in\{5,7,9,11,13\},
\]

并写

\[
X_\ell=10^{m_*+\ell M_r},
\qquad
U=5^e,
\qquad
A=5^E,
\]

\[
q_\ell=\frac{1+4B X_\ell}{r},
\qquad
K=k^2-1.
\]

中分子变量 (y=a_2) 满足

\[
\frac{X_\ell}{100}\le y<\frac{X_\ell}{10},
\qquad
\gcd(y,q_\ell U)=1.
\tag{9.7}
\]

归一化判别式严格为

\[
\boxed{
w^2
=16A^2(a_1X_\ell+10y)^2
-K\bigl(U^2a_1^2+4y^2\bigr).
}
\tag{9.8}
\]

展开后为固定系数二次曲线

\[
\begin{aligned}
w^2={}&16A^2a_1^2X_\ell^2
+320A^2a_1X_\ell y\\
&+(1600A^2-4K)y^2
-KU^2a_1^2.
\end{aligned}
\tag{9.9}
\]

对固定 ((\mathfrak s,a_1))，系数 (A,U,K) 固定，而

\[
X_\ell=X_0(10^{M_r})^\ell.
\]

所以 (9.8)–(9.9) 是一条固定 Pell–几何级数曲线，不是随 (ell)
重新生成系数的方程。

### 9.3 两个恢复符号与尺度

对 (9.8) 的整数平方根 (w\ge0)，分别定义

\[
L_\varepsilon=4A(a_1X_\ell+10y)+\varepsilon kw,
\qquad
\varepsilon\in\{\pm1\}.
\tag{9.10}
\]

只保留 (L_\varepsilon>0)。由终端索引恢复

\[
d=2^{n-2}5^{n-E},
\qquad
Y=10^n=4Ad.
\tag{9.11}
\]

完整 SD6 尺度门为

\[
\boxed{
\gcd(K,L_\varepsilon)=\frac Kd.
}
\tag{9.12}
\]

然后唯一恢复

\[
\boxed{
a_3=\frac{dL_\varepsilon}{K}
=\frac{L_\varepsilon}{\gcd(K,L_\varepsilon)}.
}
\tag{9.13}
\]

第三块窗口因 (Y=4Ad) 精确化为与 (n,d) 无关的固定系数门

\[
\boxed{
4AK\le L_\varepsilon<40AK.
}
\tag{9.14}
\]

还必须满足

\[
\boxed{\gcd(a_3,10)=1.}
\tag{9.15}
\]

由 SD6 共轭乘积，(9.12)、(9.15) 还推出

\[
a_3\mid Q,
\qquad
K^{(10)}\mid L_\varepsilon,
\]

但实现和审计时仍应直接核对，不把它们单独当作充分条件。

### 9.4 完整双向曲线清单

全部仍未关闭的终端曲线恰为

\[
\boxed{
\left\{
\mathcal C_{\mathfrak s,a_1,\varepsilon}:
\mathfrak s\in\mathscr S,
\ a_1\in\{5,7,9,11,13\},
\ \varepsilon\in\{\pm1\}
\right\},
}
\tag{9.16}
\]

其中曲线方程为 (9.8)，点和恢复门为 (9.7)、(9.10)–(9.15)。

正向方向：任一原题 A1、(gamma=1) 候选，依次由第 3–8 节唯一落入
(mathscr S)，再由 PR6 判别式给出 (9.8)，由 SD6 给出一个合法恢复符号。

反向方向：若 (9.16) 中某点通过全部门，置

\[
(b_1,b_2,b_3)=(2,q_\ell U,2dU),
\]

\[
(a_1,a_2,a_3)=(a_1,y,a_3).
\]

再定义

\[
t=\frac{Y(a_1X_\ell+10y)+a_3}{k}.
\]

SD6 回代给出

\[
(dUa_1)^2+(2dy)^2+a_3^2=t^2,
\]

以及

\[
Y(a_1X_\ell+10y)+a_3=kt.
\]

最后直接核对三个逐项既约、全部数字块窗口、K5、终端商和原拼接等式，
即可恢复合法原题六元组。故 (9.16) 没有遗漏恢复符号，也没有把判别式
平方误写成原题解。

---

## 10. 周期证书的准确停止点

对固定 ((\delta,J,e,r))，指数确实只有一条算术级数；对固定
((\mathfrak s,a_1))，(9.8) 也确实是固定系数曲线。因此每个固定终端
种子都可以进一步建立 ((\ell,y)) 二维周期系统。

但全体终端种子尚未有限化。高层仍有

\[
E=6,8,10,\ldots,
\]

并且每个 (E) 的 (r) 移动于

\[
4J5^E<r<4(J+1)5^E.
\]

条件

\[
r\mid1+4B10^m
\]

等价于一个随模数 (r) 自身移动的离散对数问题。现有链条没有给出
(E) 的绝对上界，也没有把所有允许 (r) 压成有限个固定模数或有限个
五进提升状态。各 (M_r=\operatorname{ord}_r(10)) 也随 (r) 变化，
没有一个已证明覆盖所有 (E) 的有限公共周期表。

因此：

1. 不能因固定 (r) 有唯一指数类，就宣称全体 (r) 有限；
2. 不能对有限 (E) 或有限 (m) 作筛后外推；
3. 不能把第 8.2 节的两条低层种子当作全体剩余；
4. 只有先关闭或有限化 (mathscr S_{\mathrm{hi}})，才有资格启动全分支
   的有限二维周期证书。

本轮没有生成伪造的“全周期空证书”。

---

## 11. 显式辅助射线回归与主动反例攻击

### 11.1 PR6 无界 A1 辅助射线

继承射线为

\[
m=2,quad q=3,quad N=4,quad Z=250,quad k=917,
\]

及全部 (n\ge5) 提升。这里

\[
\delta=1,qquad e=2,qquad E=3,qquad A=125,
\]

\[
r=k-Z=667.
\]

终端因子确有

\[
3\cdot667=1+20\cdot10^2.
\]

所以新正规形不会在前置层误删该射线。

但

\[
K=917^2-1\equiv3\pmod5,
\]

而 (e>0) 的完整候选由引理 7.1 必须满足

\[
v_5(K)=2\varphi\ge2.
\]

因此该射线在 SD6 精确尺度恢复处整体删除。独立地，PR6 已给出判别式
模 (5) 非平方证书；两条删除机制相容。该射线既未在前置层被误删，也
没有被保留为原题反例。

### 11.2 是否遗漏 (e=0)

没有。引理 7.1 明确只用于 (e>0)；(e=0) 时 K5 不要求 (5\mid g)，
低层生成器改为直接枚举全部

\[
d=2^{n-2}5^{n-E}\mid K,
\qquad n\ge4,
\]

直到 (d>K)。证书结果中没有 (e=0) 行。

### 11.3 是否把 (eta) 的偶性从平方条件错误提升到裸终端层

没有。第 7 节的假设明确包含 (7.2) 为整数平方和 SD6 精确尺度恢复。
裸终端因子可以有奇数 (eta)；只是这种状态不能成为完整候选。

### 11.4 是否遗漏 (m=2) 高阶消去

没有。第 6 节单独保留 (m=2) 的等赋值情形，生成器和验证器都直接
计算

\[
v_2\bigl(q^2(99A-r)-2N\bigr),
\]

没有用 (6.2)–(6.3) 机械替代。

### 11.5 是否把 (d\mid K) 错强为 (d^2\mid K)

没有。全过程只使用

\[
d=\frac K{\gcd(K,L_\varepsilon)},
\]

因而 (d\mid K)。低层证书也只检查 (d\mid K)。

### 11.6 是否只检查判别式平方

没有。完整曲线表同时要求两个符号、精确 gcd 尺度、第三块窗口、
(a_3\mid Q)、(K^{(10)}\mid L_\varepsilon)、逐项既约、主方程和原题
回代。

### 11.7 是否发现继承错误

没有。本文逐项审计后确认：

- (2.1)–(2.3) 从 PR6 恢复正确；
- W1–W4 的二值化端点正确，(delta=1) 正好对应 (b_3=Y/10)；
- SD6 的两个恢复符号、精确尺度和 (a_3\mid Q) 与本轮归一化相容；
- 原奇核心 (g_*=1) 未被用作 (gamma=1) 的替代定义。

所以本轮不是 GA1-5。

---

## 12. 最终分类与 (G) 模板最新状态

### 12.1 为什么不是 GA1-1

没有证明 (mathscr S_{\mathrm{hi}}) 为空，也没有证明 (9.16) 的全部曲线
无整数恢复点。

### 12.2 为什么不是 GA1-2

低层只有两条种子级数，但高层仍有无界偶参数

\[
E=6,8,10,\ldots.
\]

没有有限种子表覆盖全体。

### 12.3 为什么不是有限种子级二维周期系统

每个固定种子有二维周期系统，但种子索引 (mathscr S_{\mathrm{hi}}) 本身
尚未有限；有限多个固定种子的 CRT 不能覆盖无界 (E)。

### 12.4 达到的准确结果

本文严格完成：

1. 尾窗二值化与终端因子的双向恢复；
2. 每个固定 (r) 的唯一指数类和唯一单调起点；
3. A1 高阶参数的终端化；
4. (e>0) 时
   
   \[
   \varphi=\frac12v_5(k^2-1),
   \qquad
   n=E+\frac12v_5(k^2-1);
   \]

5. 高层
   
   \[
   E\text{ 为偶数},
   \qquad
   k\equiv1\pmod{2^{E-2}};
   \]

6. (E\le4) 的完整有限证书，只剩两条终端指数级数；
7. 全部分支剩余曲线的完整符号列表 (9.16)；
8. PR6 辅助射线在尺度恢复处的严格回归删除。

由于题设分类没有“低层有限证书 + 高层完整无限曲线表”的独立标签，按其
定义只能取

\[
\boxed{
\mathrm{GA1\text{-}3}.
}
\]

这不是 GA1-6：本轮已经消去了自由的 (n,\varphi)，关闭全部低层终端
状态到两条曲线级数，并给出全体剩余曲线的双向正规形。但它仍不能被包装成
完整分支关闭或有限种子化。

### 12.5 (G) 模板最新状态

截至本报告：

\[
\boxed{
O\text{ 已完整关闭};
\qquad
G_{\mathrm{prim}},\gamma=1,\mathrm{A1}
\text{ 已压成 (9.16) 的终端曲线系统};
}
\]

其中低层 (E\le4) 只有两条指数级数，高层仅允许偶 (E\ge6)，但尚未
有限化或关闭。

以下分支状态保持原样，未在本轮研究：

- (\gamma>1)；
- A2；
- B、C；
- 非本原 C2、C5；
- (Q)；
- 严格层。

全文到此停止。
