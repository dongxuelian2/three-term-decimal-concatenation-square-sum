# 三项十进制拼接平方和问题：临界 G 模板 A2 高 \(\varphi\) 单提升报告

日期：2026-08-01（Asia/Tokyo）

研究范围严格限定为

\[
\boxed{
G_{\mathrm{prim}},\qquad
\gamma=1,\qquad
\mathrm{A2},\qquad
a\ge3,\qquad
\varphi\ge a.
}
\]

本文接受 GA2-6 及其所列继承链，不研究 \(\varphi<a\)、B、C、
\(\gamma>1\)、非本原 C2/C5、Q 或严格层。最终分类为

\[
\boxed{\mathrm{GA2H\text{-}2}.}
\]

准确含义是：本分支未被统一证明为空，但已经双向压入三个显式递推族；
对每个 \(a\) 的全部局部终端状态和全部有限指数均有规范整数公式。特别地，
\(\varphi\ge a\) 区域不再含自由五进提升深度。本文没有找到合法原题解，
也没有发现 GA2-6 或继承系统错误。

为避免与继承系统中的分母尺度 \(u=5^e\) 混淆，下文把题设
\(r=\sigma+5^\zeta u\) 中的新提升坐标改记为 \(U\)。

---

## 1. 继承系统与整数参数范围

保留

\[
a\ge3,\qquad n=3a,qquad
d=2^a5^\varphi,qquad
Z=2^{2a-1}5^{3a-\varphi},
\tag{1.1}
\]

\[
e=3a+h-\varphi,\qquad
h\in\mathcal H(a),
\tag{1.2}
\]

\[
qr=1+2^{2a+m}5^{m-h},\qquad
2JZ<r<2(J+1)Z,qquad J\in\{1,\ldots,9\},
\tag{1.3}
\]

\[
k=r+Z,\qquad v_5(k^2-1)=2\varphi.
\tag{1.4}
\]

置

\[
t=\varphi-a\ge0,qquad
\zeta=3a-\varphi=2a-t,qquad
M=2^{2a}.
\tag{1.5}
\]

GA2-6 的严格上界

\[
3\varphi<3a+C_a,qquad
C_a=(2a-1)\log_5 2+\log_5 22
\]

等价于完全整数化的范围

\[
\boxed{125^t<22\cdot2^{2a-1}.}
\tag{1.6}
\]

因此对每个固定 \(a\)，允许的 \(t\) 是从 \(0\) 开始的一个完整有限初段，
而不是由浮点对数决定的近似区间。

尾窗的完整整数集合仍为

\[
\boxed{
\mathcal H(a)=
\left\{h\ge0:
2^{2a-2}\le5^{h+1},\quad5^h<2^{2a-1}
\right\}.
}
\tag{1.7}
\]

它含一个或两个相邻整数。

---

## 2. \(C_a<3a/2\) 与 \(d\mid Z\)

### 引理 2.1

对全部 \(a\ge3\)，

\[
\boxed{C_a<\frac{3a}{2}.}
\tag{2.1}
\]

**证明。** 当 \(a=3\) 时，(2.1) 等价于

\[
\log_5(22\cdot2^5)<\frac92.
\]

平方并改写为整数幂比较，即

\[
704^2=495616<1953125=5^9.
\]

另一方面，

\[
C_{a+1}-C_a=2\log_5 2=\log_5 4<\frac32,
\]

其中最后一步等价于 \(4^2<5^3\)。归纳即得 (2.1)。\(\square\)

由 \(\varphi<a+C_a/3\) 与 (2.1)，

\[
\varphi<\frac{3a}{2},\qquad 2\varphi<3a.
\tag{2.2}
\]

故

\[
v_2(Z)=2a-1\ge a,qquad
v_5(Z)=3a-\varphi>\varphi,
\]

从而

\[
\boxed{d=2^a5^\varphi\mid Z.}
\tag{R1}
\]

在 \(t\) 记号中，(2.2) 还给出

\[
\boxed{t<\frac a2,\qquad \zeta=2a-t>a+t=\varphi.}
\tag{2.3}
\]

后式将保证三个终端因子在模 \(5^\varphi\) 下具有同一个符号根。

---

## 3. 共同平方根锁定

由 \(r=k-Z\)、(R1) 和 \(d\mid k^2-1\)，

\[
r\equiv k\pmod d,qquad r^2\equiv1\pmod d.
\tag{3.1}
\]

由 \(qr=1+2ZN\) 及 \(d\mid Z\)，

\[
qr\equiv1\pmod d.
\tag{3.2}
\]

将 (3.2) 乘以 \(r\)，再用 \(r^2\equiv1\pmod d\)，得到

\[
q\equiv r\equiv k\pmod d.
\]

因此

\[
\boxed{q\equiv r\equiv k\pmod d,}
\tag{R2}
\]

\[
\boxed{q^2\equiv r^2\equiv k^2\equiv1\pmod d.}
\tag{R3}
\]

这还可精确到两个局部分量。

1. 在 \(\mathrm P_2\) 中 \(r\equiv1\pmod M\)；在
   \(\mathrm E_2\) 中 \(r\equiv1+M/2\pmod M\)。两式约到
   \(2^a\) 都给 \(r\equiv1\pmod{2^a}\)。又因 \(2^a\mid Z\)，
   (R2) 给
   \[
   \boxed{q\equiv r\equiv k\equiv1\pmod{2^a}.}
   \tag{3.3}
   \]
2. 模奇素数幂 \(5^\varphi\) 的平方根只有 \(\pm1\)。由
   \(5^\varphi\mid Z\) 和 (R2)，存在唯一
   \(\sigma\in\{\pm1\}\) 使
   \[
   \boxed{q\equiv r\equiv k\equiv\sigma\pmod{5^\varphi}.}
   \tag{3.4}
   \]

所以 \((q,r,k)\) 只落在两个模 \(d\) 的共同根类，而不是任意单位类。

---

## 4. 单提升定理与精确五进阶

因为

\[
v_5(k^2-1)=2\varphi
\]

且 \(\gcd(k-1,k+1)\mid2\)，存在唯一符号
\(\sigma\in\{\pm1\}\) 使

\[
\boxed{v_5(k-\sigma)=2\varphi.}
\tag{4.1}
\]

### 4.1 \(t>0\)

此时 \(\zeta<2\varphi\)。写

\[
k-\sigma=5^{2\varphi}w_5,\qquad5\nmid w_5.
\]

由于 \(Z=5^\zeta M/2\)，

\[
r-\sigma
=5^\zeta\left(5^{2\varphi-\zeta}w_5-\frac M2\right)
=5^\zeta\left(5^{3t}w_5-\frac M2\right).
\]

括号模 \(5\) 非零，故

\[
\boxed{v_5(r-\sigma)=\zeta.}
\tag{S1}
\]

并且唯一写成

\[
\boxed{r=\sigma+5^\zeta U,\qquad5\nmid U.}
\tag{S2}
\]

### 4.2 \(t=0\)

此时 \(\zeta=2\varphi=2a\)，仍唯一写成

\[
r=\sigma+5^\zeta U,
\]

但不能预设 \(5\nmid U\)。由

\[
k=\sigma+5^\zeta\left(U+\frac M2\right)
\]

和 (4.1)，必须且只须

\[
v_5\left(U+\frac M2\right)=0.
\]

### 4.3 统一公式

两种情形合并为

\[
\boxed{
v_5\left(U+\frac M2\right)
=2\varphi-\zeta
=3(\varphi-a)=3t.
}
\tag{V1}
\]

令

\[
W=\frac{U+M/2}{5^{3t}}.
\tag{4.2}
\]

则 \(5\nmid W\)，且

\[
\boxed{k=\sigma+5^{2\varphi}W.}
\tag{4.3}
\]

因此

\[
\boxed{
\frac{k^2-1}{5^{2\varphi}}\equiv2\sigma W\pmod5.
}
\tag{4.4}
\]

GA2-6 的判别式剩余门正好变成

\[
2\sigma W\equiv1\text{ 或 }4\pmod5.
\tag{4.5}
\]

式 (V1) 证明：

\[
\boxed{\varphi\ge a\text{ 区域不存在自由五进提升深度}.}
\tag{4.6}
\]

---

## 5. 窗口恰含一个二进周期

二进两室记为

\[
c_2=
\begin{cases}
1,&\mathrm P_2,\\
1+M/2,&\mathrm E_2.
\end{cases}
\]

由 \(r=\sigma+5^\zeta U\) 得

\[
\boxed{
U\equiv(c_2-\sigma)5^{-\zeta}\pmod M.
}
\tag{U1}
\]

严格终端窗除以 \(5^\zeta\)，逐端使用整数性，得到：

\[
\boxed{JM\le U\le(J+1)M-1\qquad(\sigma=1),}
\tag{U2+}
\]

\[
\boxed{JM+1\le U\le(J+1)M\qquad(\sigma=-1).}
\tag{U2-}
\]

令

\[
U_0=\left\langle(c_2-\sigma)5^{-\zeta}\right\rangle_M
\in\{0,\ldots,M-1\},
\tag{5.1}
\]

其中 \(\langle\cdot\rangle_M\) 表示最小非负剩余。唯一提升坐标的规范公式为

\[
\boxed{
U=
\begin{cases}
JM+U_0,&\sigma=1,\\
JM+1+\langle U_0-1\rangle_M,&\sigma=-1.
\end{cases}
}
\tag{5.2}
\]

因此每个

\[
(a,h,t,J,\mathrm P_2/\mathrm E_2,\sigma)
\]

至多产生一个 \(U\)、一个 \(r\) 和一个 \(k\)。

---

## 6. 三个显式递推族

定义

\[
p_{a,t}=\left\langle5^{-(2a-t)}\right\rangle_{4^a}.
\tag{6.1}
\]

对固定 \(a\)，

\[
\boxed{p_{a,t}=\langle5^t p_{a,0}\rangle_{4^a}.}
\tag{6.2}
\]

所以不必对每个 \(t\) 独立求逆。置

\[
x_{a,t}=\langle2p_{a,t}\rangle_M,qquad
y_{a,t}=\left\langle2p_{a,t}+\frac M2\right\rangle_M.
\tag{6.3}
\]

则四个原始室—符号公式退化为

\[
\begin{array}{c|c}
(\mathrm P_2,+)&U=JM\\
(\mathrm E_2,+)&U=JM+M/2\\
(\mathrm P_2,-)&U=JM+x_{a,t}\\
(\mathrm E_2,-)&U=JM+y_{a,t}.
\end{array}
\tag{6.4}
\]

### 6.1 正符号的两次统一删除

在 \((\mathrm P_2,+)\) 中，(V1) 化为

\[
v_5(2J+1)=3t.
\tag{6.5}
\]

由于 \(3\le2J+1\le19\)，左边至多为 \(1\)。所以 \(t>0\) 全部删除。
当 \(t=0\) 时，联合 (4.5) 和主室模 \(8\) 门

\[
\frac{k^2-1}{2^{2a}}\equiv3\text{ 或 }7\pmod8
\]

作 \(J=1,\ldots,9\) 的固定剩余表，恰只留下

\[
\boxed{J\in\{5,9\}.}
\tag{6.6}
\]

此族有特别简单的闭式

\[
\boxed{
r=1+J100^a,qquad
k=1+\frac{2J+1}{2}100^a,qquad J\in\{5,9\}.
}
\tag{F+}
\]

在 \((\mathrm E_2,+)\) 中，(V1) 为

\[
v_5(J+1)=3t.
\]

更强地，

\[
v_2(k^2-1)=2a+v_2(J+1)+1\le2a+4<4a+2
\]

对全部 \(a\ge3\) 成立，与异常室的最低要求

\[
v_2(k^2-1)\ge4a+2v_2(H_1)\ge4a+2
\]

矛盾。因此

\[
\boxed{(\mathrm E_2,+)\text{ 整体为空}.}
\tag{6.7}
\]

### 6.2 最终三个族

本分支全部候选被完备压入下列三个递推族：

\[
\boxed{
\begin{array}{ll}
\mathcal F_+:&t=0,\ \mathrm P_2,\ \sigma=+1,\ J\in\{5,9\};\\
\mathcal F_{P-}:&t\ge0,\ \mathrm P_2,\ \sigma=-1,\ U=JM+x_{a,t};\\
\mathcal F_{E-}:&t\ge0,\ \mathrm E_2,\ \sigma=-1,\ U=JM+y_{a,t}.
\end{array}}
\tag{6.8}
\]

每一行还须检查 (V1)、(4.5)，主室还检查 GA2-6 的模 \(8\) 门；异常室
令 \(\alpha=v_2(k^2-1)\)，先要求

\[
\alpha\ge4a+2,
\]

并在后续分子恢复中只允许

\[
\boxed{1\le v_2(H_1)\le
\left\lfloor\frac{\alpha-4a}{2}\right\rfloor.}
\tag{6.9}
\]

### 6.3 关于 \(a\) 的规范递推

上述公式不只是“每个 \(a\) 有限”。它们由有限条整数递推生成。

令

\[
H_a=\max\{h:5^h<2^{2a-1}\}.
\]

则 \(H_3=2\)，且

\[
H_{a+1}=
\begin{cases}
H_a+1,&5^{H_a+1}<2^{2a+1},\\
H_a,&\text{否则}.
\end{cases}
\tag{6.10}
\]

随后

\[
\mathcal H(a)=
\{H_a\}\cup
\{H_a-1:5^{H_a}\ge2^{2a-2}\}.
\tag{6.11}
\]

令

\[
T_a=\max\{t:125^t<22\cdot2^{2a-1}\}.
\]

则 \(T_3=1\)，且因每步右端只乘 \(4<125\)，

\[
T_{a+1}\in\{T_a,T_a+1\},
\tag{6.12}
\]

由下一幂是否满足严格不等式唯一决定。

最后令 \(P_a=p_{a,0}\)，所以

\[
25^aP_a=1+Q_a4^a.
\]

先取唯一 \(\delta_a\in\{0,1,2,3\}\) 使

\[
Q_a+\delta_a25^a\equiv0\pmod4,
\]

并置 \(\widehat P_a=P_a+\delta_a4^a\)。则

\[
\boxed{
P_{a+1}=\left\langle25^{-1}\widehat P_a\right\rangle_{4^{a+1}},
\qquad P_3=57.
}
\tag{6.13}
\]

式 (6.2)、(6.10)–(6.13) 联合 (6.8)，就是覆盖全部无界 \(a\) 的
有限递推系统。

---

## 7. 终端因子与完整有限指数段

对通过全部局部门的唯一 \(r\)，有 \(\gcd(r,10)=1\)。置

\[
\ell=m-h,qquad C_{a,h}=2^{2a+h}.
\]

终端因子条件严格等价于

\[
\boxed{10^\ell\equiv-C_{a,h}^{-1}\pmod r.}
\tag{7.1}
\]

令

\[
M_r=\operatorname{ord}_r(10).
\]

若右端不属于 \(\langle10\rangle\subset(\mathbb Z/r\mathbb Z)^\times\)，
该终端状态整体删除；否则存在唯一

\[
\ell_0\in[0,M_r)
\]

使 (7.1) 成立，全部指数为

\[
\ell\equiv\ell_0\pmod{M_r}.
\tag{7.2}
\]

本分支中

\[
e=\zeta+h\ge5,
\]

所以 \(m\ge\max(2,e)\) 简化为

\[
\ell\ge\zeta.
\tag{7.3}
\]

上端不用浮点数定义。令 \(m_{\max}\) 是满足

\[
\boxed{
20\cdot10^m<194029Z^2Y
}
\tag{7.4}
\]

的最大整数；若不存在则该状态为空。全部终端指数恰为

\[
\boxed{
m=h+\ell,qquad
\zeta\le\ell\le m_{\max}-h,qquad
\ell\equiv\ell_0\pmod{M_r}.
}
\tag{7.5}
\]

这是完整有限同余段，不是对无界指数类取若干样本。

对 (7.5) 中每个 \(m\)，定义

\[
N=2^m5^{m-e},\qquad
q=\frac{1+2ZN}{r},\qquad
\rho_0=r-2JZ,qquad
s=N-Jq.
\tag{7.6}
\]

由于 \(N\ge2^e>9\) 且 \(\rho_0\ge1\)，初端门

\[
N\rho_0>J
\]

在本分支自动成立。因此 \(0<s<q\)，并恢复完整终端状态；没有遗漏一个
额外的无界初端搜索。

---

## 8. 每个 \(a\) 的完整有限恢复公式

固定 (7.5) 中的状态。重申 \(T=10^m\)，并置

\[
b_1=2,qquad b_2=q5^e,qquad b_3=2d5^e,qquad Y=10^{3a}.
\tag{8.1}
\]

依次枚举完整有限集合

\[
a_1\in\{5,7,9,11,13\},qquad
10^{m-2}\le a_2<10^{m-1},qquad
\gcd(a_2,b_2)=1.
\tag{8.2}
\]

定义

\[
H_1=a_1T+10a_2,qquad
R=(5^ea_1)^2+(2a_2)^2,qquad
K=k^2-1,qquad A=2ZH_1.
\tag{8.3}
\]

异常室先核对 (6.9)。随后要求

\[
w_0^2=A^2-KR,qquad w_0\in\mathbb Z_{\ge0}.
\tag{8.4}
\]

对两个符号分别置

\[
L_\varepsilon=A+\varepsilon kw_0.
\]

只保留 \(L_\varepsilon>0\) 且

\[
\boxed{
d=\frac K{\gcd(K,L_\varepsilon)},\qquad
a_3=\frac{L_\varepsilon}{\gcd(K,L_\varepsilon)}\in[Y,10Y).
}
\tag{8.5}
\]

再核对

\[
a_3\mid(k^2R-A^2),\qquad
K^{(10)}\mid L_\varepsilon,qquad
\gcd(a_3,b_3)=1,
\tag{8.6}
\]

球面、拼接恢复和原题直接回代。因 (8.2) 是严格有限区间，这给出每个
\(a\) 的完整有限状态公式。这里没有把判别式平方、局部尺度或任一恢复符号
误写成充分条件。

---

## 9. 独立生成器与验证器

附件实现两个分离路径。

1. 生成器按三个递推族生成局部状态；以精确试除分解 \(r\) 和
   \(\varphi(r)\)，约去阶的素因子求真实 \(M_r\)，再以 BSGS 求完整离散
   对数类，并与有限指数段逐项直算比较。可用 `--full-recovery` 启动
   第 8 节的完整有限分子恢复。
2. 验证器从原始四个室—符号组合重新生成唯一 \(U\)，不信任三族列表；它用
   直接乘法轨道重建 \(M_r\) 和离散对数，再逐个整数 \(m\) 回放终端因子，
   并附带破坏性测试。

规范回归证书取 \(a=3\)。这是实现核对，不承担对无界 \(a\) 的外推；无界
完备性由第 2–8 节的符号证明和递推定理承担。输出为

```text
a=3 local_states=6 terminal_exponents=0 original_solutions=0
independently verified recursive certificate: a=3 local_states=6 terminal_exponents=0 original_solutions=0
```

规范文件 SHA-256：

```text
critical_G_A2_high_phi_single_lift_generator.py
80faa8db1b726a77c9d3d5c673817944d58d50326bdfd5422c110f7ee7cd6302

critical_G_A2_high_phi_single_lift_verifier.py
5359dd605a9005a4f787ef0299f595fdabdf481b6c81d4173a90d9d8d879c78b

critical_G_A2_high_phi_single_lift_certificate.json
69ff7845903a0e45461b5306af93391dbaa441d6d3a2e5538773ca3fffbb1164

critical_G_A2_high_phi_single_lift_certificate_bundle.tar.gz
b6462be41583473e59980c389ae9389d3193f94b0e9a7fd07709dff8881e764b
```

验证命令：

```bash
python3 critical_G_A2_high_phi_single_lift_verifier.py \
  critical_G_A2_high_phi_single_lift_certificate.json --destruction-tests
```

---

## 10. 主动审计

### 10.1 是否在 \(\varphi=a\) 预设 \(5\nmid U\)

没有。边界只由 (V1) 要求 \(5\nmid(U+M/2)\)；\(U\) 自身可以被 \(5\)
整除。

### 10.2 是否把模 \(2^a\) 的平方根误写成一般只有 \(\pm1\)

没有。二进正根来自 GA2-6 已证明的更强室剩余模 \(2^{2a}\)，不是来自
“模 \(2^a\) 的平方根只有 \(\pm1\)”这一错误命题。

### 10.3 是否遗漏异常室

没有。只统一删除了 \((\mathrm E_2,+)\)；\((\mathrm E_2,-)\) 作为第三个
递推族完整保留，并携带实际 \(\alpha\) 和允许的 \(v_2(H_1)\) 上界。

### 10.4 是否把每个 \(a\) 有限误报为 \(a\) 有界

没有。\(a\) 仍无绝对上界；第 6.3 节给出的是覆盖所有 \(a\) 的整数递推，
而不是有限检查 \(a\)。

### 10.5 是否有限采样无界指数

没有。先以真实 \(M_r\) 和完整离散对数类得到 (7.2)，再用已证明的判别式
上界截成 (7.5) 的完整有限同余段。

### 10.6 是否用浮点数决定整数边界

没有。\(t\)、\(h\) 和 \(m\) 的全部端点分别由 (1.6)、(1.7)、(7.4)
的整数幂比较决定。

### 10.7 是否发现继承错误

没有。题设以同一个字母 \(u\) 同时表示原分母尺度 \(5^e\) 和新提升坐标，
属于记号冲突；本文改记 \(U\)，不构成数学错误。R1–V1 与 GA2-6 相容。

### 10.8 \(a=3\) 的空终端证书是否被外推

没有。它只核对两个实现。本文没有据此宣称 \(a\ge4\) 为空；GA2H-2 的
无界结论来自递推压缩，而不是该有限样本。

---

## 11. 最终分类与停止点

本文严格证明：

1. 对全部 \(a\ge3\)，\(C_a<3a/2\)，故 \(d\mid Z\)；
2. \(q,r,k\) 只能位于两个共同模 \(d\) 根类；
3. \(\varphi\ge a\) 中每个室—符号—窗口元组至多有一个五进提升；
4. 精确五进阶统一为 (V1)，不存在自由提升深度；
5. \((\mathrm E_2,+)\) 整体为空，\((\mathrm P_2,+)\) 只剩
   \(t=0,J=5,9\)；
6. 全部剩余状态完备落入 (6.8) 的三个显式递推族；
7. 每个递推状态的全部指数由真实乘法阶、完整离散对数类和严格整数上界
   给出；
8. 每个 \(a\) 的后续判别式、两个恢复符号、尺度、逐项既约和原题回代均为
   明确有限公式。

这已经超过“只证明单提升但仍保留未组织的无界 \(a\)”的 GA2H-3 停止点。
然而本文没有得到三个递推族的统一空性证书，所以不能分类为 GA2H-1；也没有
找到合法原题六元组或继承错误。

故最终分类为

\[
\boxed{
\mathrm{GA2H\text{-}2}:
\quad
\varphi\ge a\text{ 的完整子分支被压成三个显式整数递推族，}
\text{每个 }a\text{ 的终端与恢复状态均严格有限。}
}
\]

开放对象只剩这三个递推族中通过第 7、8 节全部门的状态。本文到此停止，
不研究 \(\varphi<a\)、B、C、\(\gamma>1\)、C2/C5、Q 或严格层。

---

## 12. 后继状态说明：GE2-1 删除 \(\mathcal F_{E-}\)

日期：2026-08-06（Asia/Tokyo）

后继报告 `critical_G_A2_exceptional_binary_resolution.md` 已在完整
判别式—尺度恢复层严格证明

\[
\boxed{
\mathrm E_2\Longrightarrow\text{无完整候选}.
}
\tag{12.1}
\]

该结论不依赖 \(\varphi\ge a\) 或五进根类 \(\sigma\)。因此本报告第 6.2 节
构造的异常负符号递推族满足

\[
\boxed{
\mathcal F_{E-}\Longrightarrow\text{无候选}.
}
\tag{12.2}
\]

第 5、6 节对 \(\mathcal F_{E-}\) 的唯一提升公式和局部参数化本身没有
错误；它们给出了一个必要递推族。GE2-1 新增的共轭乘积赋值表明，该族没有
任何状态能够通过完整尺度恢复，所以不再进入第 7、8 节的终端与分子枚举。

再联合已经冻结的

\[
\mathcal F_+\Longrightarrow\text{无候选},
\]

高 \(\varphi\) 区的最新完备状态为

\[
\boxed{
G_{\mathrm{prim}},\quad
\gamma=1,\quad
\mathrm{A2},\quad
a\ge3,\quad
\varphi\ge a
\Longrightarrow
\text{只剩 }\mathcal F_{P-}.
}
\tag{12.3}
\]

其中 \(\mathcal F_{P-}\) 尚未统一关闭：六条零商族仍为移动高位 Bezout
正规形；\(\mathscr P_0\)、\(\mathscr P_1\) 的每个递推状态至多一个
显式候选，但同样受移动高位二进 Bezout 数字控制。不得把 (12.3) 误报为
整个高 \(\varphi\) 区为空。

同时，A2 的完整二进尺度关系已由 GE2-1 升级为

\[
\boxed{v_2(k^2-1)=2a.}
\tag{12.4}
\]

本后继说明不研究 \(\mathcal F_{P-}\)、\(\varphi<a\)、B、C、
\(\gamma>1\)、C2/C5、Q 或严格层。
