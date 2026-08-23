# 三项十进制拼接平方和问题：临界 G 模板 A2 高 \(\varphi\) 主二进室负符号族双走廊报告

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

接受 `critical_G_A2_high_phi_Fprimary_minus_campaign.md` 的 GFPm-3
三层下降、`critical_G_A2_high_phi_single_lift_campaign.md` 的 GA2H-2
双向正规形、`critical_G_A2_unit_determinant_campaign.md` 的 GA2-6
局部门与大小门，以及 PR6、SD6 和 v3 总账中与本分支相容的结论。

本轮没有证明整个 \(\mathcal F_{P-}\) 为空。得到的严格推进是：

1. 唯一 CRT 余数被改写成不含移动模数 \(r\) 的精确双商—进位坐标；
2. 所有低二进室的正商被删除；
3. 所有 \(\epsilon=1\) 室的正商被删除；
4. \(j=2,\epsilon=0\) 的正商先被纯符号论证强迫到绝对有限边界，
   再由独立证书完整删除；
5. 全部剩余状态双向压成八条明确进位递推族：六条零商族与
   \(j=0,1\) 的两条正商族。

因此最终分类为

\[
\boxed{\mathrm{GFPmR\text{-}3}.}
\]

这里的剩余对象不再是“计算随 \(r\) 移动的一个模余数”：每个终端候选先由
固定的 \(2,5\) 幂进位生成一个明确整数 \(E^*\)，再作至多三步的确定性
反向整除进位，并检查是否恢复继承初值 \(E_0\)。两条正商族中的进位大小仍可
随 \(a\) 无界，故本文没有得到固定有限状态自动机，也不能分类为 GFPmR-1
或 GFPmR-2。

---

## 1. Bezout 双坐标

置

\[
M=2^{2a},\qquad C=5^{c_0},\qquad c_0=2a-t,
\tag{1.1}
\]

\[
x=\left\langle2C^{-1}\right\rangle_M,
\qquad
Cx=2+Mc,
\tag{1.2}
\]

\[
U=JM+x,
\qquad
\boxed{D=CJ+c}.
\tag{1.3}
\]

由 (1.2) 直接得到

\[
CU=CJM+Cx=M(CJ+c)+2=MD+2,
\]

所以

\[
\boxed{CU-MD=2.}
\tag{1.4}
\]

负符号主室中

\[
r=-1+CU,
\]

故 (1.4) 同时给出

\[
\boxed{r=-1+CU=1+MD.}
\tag{1.5}
\]

两式缺一不可：第一式给五进商，第二式给二进商。

沿用 GFPm-3 的非平凡根坐标

\[
\rho=Cx-1=1+Mc,
\qquad
\eta=cx,
\qquad
E_0=\eta+\rho J.
\tag{1.6}
\]

除继承恒等式 \(\rho r=1+MCE_0\) 外，本轮还记录两个精确乘积式：

\[
\boxed{UD=E_0+Jr,}
\qquad
\boxed{xD=E_0+J.}
\tag{1.7}
\]

例如第一式由

\[
UD=(JM+x)(CJ+c)=Jr+\eta+\rho J
\]

逐项展开得到。它们为后文反向进位提供独立复核门。

GFPm-3 已经证明，每个三层状态在至多一次额外下降后唯一成为

\[
\boxed{2^A5^F=E+\ell r,}
\tag{1.8}
\]

\[
0<E<r,
\qquad
0\le F<c_0,
\qquad
0\le\ell<5^F.
\tag{1.9}
\]

后文始终保留 \(F=0,\ell=0\) 边界。

---

## 2. 五进商与低二进商

### 2.1 五进商是精确等式

唯一 CRT 条件给

\[
\ell\equiv E\pmod{5^F}.
\]

定义

\[
\boxed{u=\frac{E-\ell}{5^F}\in\mathbb Z_{\ge0}.}
\tag{2.1}
\]

把 \(r=-1+CU\) 代入 (1.8)：

\[
\begin{aligned}
2^A5^F
&=E+\ell(-1+CU)\\
&=(E-\ell)+\ell5^{c_0}U\\
&=5^F\left(u+\ell5^{c_0-F}U\right).
\end{aligned}
\]

故严格得到整数等式

\[
\boxed{2^A=u+\ell5^{c_0-F}U.}
\tag{2.2}
\]

这不是同余。

### 2.2 低二进室统一只有零商

若 \(A<2a\)，二进 CRT 条件为

\[
\ell\equiv-E\pmod{2^A}.
\]

定义

\[
v=\frac{E+\ell}{2^A}\in\mathbb Z_{\ge0}.
\tag{2.3}
\]

把 \(r=1+MD\) 代入 (1.8)：

\[
\begin{aligned}
2^A5^F
&=E+\ell(1+MD)\\
&=(E+\ell)+\ell2^{2a}D\\
&=2^A\left(v+\ell2^{2a-A}D\right).
\end{aligned}
\]

所以

\[
\boxed{5^F=v+\ell2^{2a-A}D.}
\tag{2.4}
\]

若 \(\ell\ge1\)，则因 \(2a-A\ge1\)、\(D>C=5^{c_0}>5^F\)，

\[
\ell2^{2a-A}D\ge2D>5^F,
\]

与 (2.4) 矛盾。因此

\[
\boxed{
A<2a\Longrightarrow \ell=0,\qquad E=2^A5^F.
}
\tag{2.5}
\]

这只把低二进室送入零商递推；并未把零商自动判空。

---

## 3. 高二进双商走廊

现在设 \(A\ge2a\)，定义

\[
\boxed{v=\frac{E+\ell}{M}\in\mathbb Z_{\ge0}.}
\tag{3.1}
\]

由 \(r=1+MD\) 得

\[
\boxed{2^{A-2a}5^F=v+\ell D.}
\tag{3.2}
\]

由 (2.1)、(3.1) 直接相减：

\[
\boxed{Mv-5^Fu=2\ell.}
\tag{3.3}
\]

由于 \(M\) 和 \(2\ell\) 都是偶数、\(5^F\) 为奇数，

\[
\boxed{2\mid u.}
\tag{3.4}
\]

写 \(u=2u_1\)，(3.3) 进一步成为固定 \((2,5)\)-进位式

\[
\boxed{\ell=2^{2a-1}v-5^Fu_1.}
\tag{3.5}
\]

因 \(0\le\ell<5^F\)，有

\[
\boxed{
\ell=\left\langle2^{2a-1}v\right\rangle_{5^F},
\qquad
u_1=\left\lfloor\frac{2^{2a-1}v}{5^F}\right\rfloor.
}
\tag{3.6}
\]

这一步已经把 \(\ell\) 从“模移动的 \(r\)”改写为模纯五次幂的普通进位。

若 \(\ell>0\)，从 (2.2) 及 \(U>JM\) 得

\[
2^A>\ell5^{c_0-F}JM,
\]

从 (3.2) 及 \(D>CJ\) 得同一上界

\[
\boxed{
1\le\ell<
\frac{2^{A-2a}}{J5^{c_0-F}}.
}
\tag{3.7}
\]

特别地

\[
\boxed{2^{A-2a}>J5^{c_0-F}.}
\tag{3.8}
\]

---

## 4. 六个 \((j,\epsilon)\) 室的整数幂展开

写原三层指数为

\[
\nu=2aj+v_0,
\qquad
j\in\{0,1,2\},
\qquad
0\le v_0<2a.
\tag{4.1}
\]

下降前

\[
A_j=2a-t+h+v_0,
\qquad
F_j=v_0+tj.
\tag{4.2}
\]

### 4.1 \(\epsilon=0\)

条件和最终指数为

\[
v_0+(j+1)t<2a,
\tag{4.3}
\]

\[
A=2a-t+h+v_0,
\qquad
F=v_0+tj.
\tag{4.4}
\]

所以

\[
A-2a=h+v_0-t,
\qquad
c_0-F=2a-v_0-(j+1)t.
\]

正商溢出条件严格化为

\[
\boxed{
2^{h+v_0-t}>
J5^{,2a-v_0-(j+1)t}.
}
\tag{4.5}
\]

### 4.2 \(\epsilon=1\)

条件和最终指数为

\[
v_0+(j+1)t\ge2a,
\tag{4.6}
\]

\[
A=h+v_0-t,
\qquad
F=v_0+(j+1)t-2a.
\tag{4.7}
\]

若还位于高二进室，则

\[
A-2a=h+v_0-t-2a,
\qquad
c_0-F=4a-v_0-(j+2)t,
\]

因而正商条件为

\[
\boxed{
2^{h+v_0-t-2a}>
J5^{,4a-v_0-(j+2)t}.
}
\tag{4.8}
\]

全部端点都由整数幂比较定义，没有使用实数对数。

---

## 5. 所有 \(\epsilon=1\) 正商室为空

先假设 \(A\ge2a\)，否则第 2.2 节已经给出 \(\ell=0\)。

### 5.1 \(j=0\)

由 \(v_0\le2a-1\)、\(h\le a-1\)，(4.8) 左边至多为

\[
2^{h-t-1}\le2^{a-2}.
\]

另一方面

\[
4a-v_0-2t\ge2a+1-2t>a+1,
\]

故右边至少为 \(5^{a+2}\)，不可能小于左边。

### 5.2 \(j=1\)

左边仍至多为 \(2^{a-2}\)。而

\[
4a-v_0-3t\ge2a+1-3t>\frac a2+1.
\]

因 \(5^{a/2}>2^a\) 等价于 \(5^a>4^a\)，右边再次严格大于左边。

### 5.3 \(j=2\)

若 \(t=0\)，(4.6) 要求 \(v_0\ge2a\)，与 \(v_0<2a\) 矛盾。
若 \(t\ge1\)，第三层精确上界为

\[
v_0\le a+t+2-h.
\]

而高二进条件 \(A\ge2a\) 要求

\[
v_0\ge2a+t-h.
\]

两式联合给 \(a\le2\)，与 \(a\ge3\) 矛盾。

因此

\[
\boxed{
\epsilon=1\Longrightarrow\ell=0.
}
\tag{5.1}
\]

---

## 6. 去除移动模数的进位参数化

本节给出本轮核心双向定理。

设 \(A\ge2a\)，置

\[
\boxed{
p=2^{A-2a},
\qquad
q_*=c_0-F\ge1.
}
\tag{6.1}
\]

对任意可能的 \(\ell\)，定义主进位

\[
\boxed{w=p-J\ell5^{q_*}.}
\tag{6.2}
\]

### 定理 6.1：静态双商进位

高二进 CRT 走廊与下列整数系统双向等价：

\[
0\le\ell<5^F,
\qquad
w=p-J\ell5^{q_*}>0,
\tag{6.3}
\]

\[
\boxed{
u=Mw-\ell5^{q_*}x,
\qquad
v=5^Fw-\ell c,
}
\tag{6.4}
\]

\[
\boxed{
E^*=M5^Fw-\ell\rho,
\qquad
0<E^*<r,
}
\tag{6.5}
\]

再加上 \(E^*=E_d\)，其中 \(d=j+\epsilon\) 是继承下降深度。

**正向证明。** 由 (2.2) 写

\[
2^A=u+\ell5^{q_*}(JM+x).
\]

除去 \(M\) 并使用 \(p=2^{A-2a}\)，得到

\[
u=M(p-J\ell5^{q_*})-\ell5^{q_*}x=Mw-\ell5^{q_*}x.
\]

同理由 (3.2) 与 \(D=CJ+c=J5^{F+q_*}+c\) 得

\[
v=5^F(p-J\ell5^{q_*})-\ell c=5^Fw-\ell c.
\]

最后

\[
\ell+5^Fu=M5^Fw-\ell(Cx-1)=M5^Fw-\ell\rho,
\]

\[
Mv-\ell=M5^Fw-\ell(1+Mc)=M5^Fw-\ell\rho.
\]

故两条商表达给出同一个 \(E^*\)。

**反向证明。** 由 (6.2)、(6.5) 与 \(r=\rho+MCJ\)，

\[
\begin{aligned}
E^*+\ell r
&=M5^Fw-\ell\rho+\ell(\rho+MCJ)\\
&=M5^F(w+J\ell5^{q_*})\\
&=M5^Fp=2^A5^F.
\end{aligned}
\]

又因 \(\rho\equiv-1\pmod{5^F}\)、\(\rho\equiv1\pmod M\)，

\[
E^*\equiv\ell\pmod{5^F},
\qquad
E^*\equiv-\ell\pmod M.
\]

结合范围即恢复唯一 CRT 余数。故 (6.3)–(6.5) 不只是必要筛。
\(\square\)

特别地，正商候选不再通过 \(E_d\bmod r\) 生成；它的有限区间直接是

\[
\boxed{
1\le\ell\le
L:=\min\left(
5^F-1,
\left\lfloor\frac{p-1}{J5^{q_*}}\right\rfloor
\right).
}
\tag{6.6}
\]

### 6.2 至多三步的确定性反向进位

还需检查静态生成的 \(E^*\) 是否正好是继承下降余项 \(E_d\)。这可不用
移动模逆元完成。

置

\[
R_d=E^*.
\]

对 \(i=d-1,d-2,\ldots,0\) 依次定义

\[
\boxed{
\kappa_i=\left\lfloor\frac{BR_{i+1}}r\right\rfloor,
\qquad
R_i=BR_{i+1}-\kappa_i r.
}
\tag{6.7}
\]

若某一步 \(R_i=0\)，立即拒绝；否则自动有 \(0<R_i<r\) 及
\(0\le\kappa_i<B\)。候选成立当且仅当

\[
\boxed{R_0=E_0.}
\tag{6.8}
\]

若 (6.8) 成立，从 \(L_d=\ell\) 开始反向定义

\[
\boxed{L_i=\kappa_i+BL_{i+1}.}
\tag{6.9}
\]

则逐步有

\[
\frac N{B^i}=R_i+L_ir,
\]

最终恢复

\[
N=E_0+L_0r,
\qquad
q=\rho+BL_0,
\qquad
s=\eta+\rho L_0.
\tag{6.10}
\]

继承证明给出 \(0<s<q\)。所以 (6.1)–(6.10) 是完整双向恢复，而不是只
检查若干必要同余。

---

## 7. 双商的赋值与近邻约束

由 \(x\equiv2C^{-1}\pmod M\) 且 \(C^{-1}\) 为奇数，

\[
\boxed{v_2(x)=v_2(U)=1.}
\tag{7.1}
\]

主室局部门还给 \(D\) 为奇数。事实上

\[
k=1+\frac M2(2D+C),
\]

而 \(a\ge3\) 时

\[
\frac{k^2-1}{M}\equiv2D+C\pmod8.
\]

该数模 \(8\) 为 \(3\) 或 \(7\)，模 \(4\) 化简并用 \(C\equiv1\pmod4\)，
得到

\[
\boxed{2\nmid D.}
\tag{7.2}
\]

又因 \(q_*\ge1\)，(2.2) 模 \(5\) 给

\[
\boxed{5\nmid u.}
\tag{7.3}
\]

对 \(\ell>0\)，写 \(e_5=v_5(\ell)<F\)。由 (3.2) 及
\(5\nmid D\)，

\[
\boxed{v_5(v)=v_5(\ell).}
\tag{7.4}
\]

若 \(v_2(\ell)+1<A\)，由 (2.2)、(7.1) 还得到

\[
\boxed{v_2(u)=v_2(\ell)+1.}
\tag{7.5}
\]

若 \(v_2(\ell)<A-2a\)，由 (3.2)、(7.2) 得

\[
\boxed{v_2(v)=v_2(\ell).}
\tag{7.6}
\]

这些关系和 (3.5)–(3.6) 构成固定 \((2,5)\) 字母上的局部进位门；
它们不再调用完整移动模数 \(r\)。但 \(w,u,v\) 本身仍可无界，故本文不把
它们误报为有限状态自动机。

---

## 8. \(j=2,\epsilon=0,\ell>0\) 的绝对有限化

本室有

\[
F=v_0+2t,
\qquad
q_*=2a-v_0-3t,
\qquad
p=2^{h+v_0-t}.
\tag{8.1}
\]

正商必要条件为

\[
J5^{q_*}<p.
\]

乘以 \(2^{q_*}\) 得

\[
\boxed{J10^{q_*}<2^{2a+h-4t}.}
\tag{8.2}
\]

### 8.1 \(t=0\)

第三层上界 \(v_0\le a+3-h\) 给

\[
q_*=2a-v_0\ge a+h-3.
\]

由 (8.2)、\(J\ge1\)，

\[
10^{a+h-3}<2^{2a+h}.
\]

又 \(h\ge1\)，故必要地

\[
5^{a+1}<1000\cdot2^a.
\tag{8.3}
\]

它在 \(a=6\) 时已经失败：

\[
5^7=78125>64000=1000\cdot2^6,
\]

以后两边之比每步再乘 \(5/2>1\)。因此

\[
\boxed{t=0\Longrightarrow a\le5.}
\tag{8.4}
\]

### 8.2 \(t\ge1\)

第三层上界 \(v_0\le a+t+2-h\) 给

\[
q_*\ge a+h-4t-2.
\]

由 (8.2) 得

\[
5^{a+h-4t}<100\cdot2^a.
\tag{8.5}
\]

尾窗左端

\[
2^{2a-2}\le5^{h+1}
\]

代入 (8.5)，推出必要条件

\[
2^{a-2}5^a<500\cdot5^{4t}.
\tag{8.6}
\]

将 (8.6) 立方，并把严格提升上界

\[
5^{3t}=125^t<22\cdot2^{2a-1}=11\cdot4^a
\]

取四次方代入，得到

\[
\boxed{
125^a<2^{5a+6}\,500^3\,11^4.
}
\tag{8.7}
\]

在 \(a=24\) 时，左、右分别为

\[
211758236813575084767080625169910490512847900390625,
\]

\[
155689816690295626361477113356516199497728000000000,
\]

故 (8.7) 已失败。以后左、右比值每步再乘 \(125/32>1\)。所以

\[
\boxed{t\ge1\Longrightarrow a\le23.}
\tag{8.8}
\]

这是绝对有限化的符号来源；后面的机器证书不承担任意 \(a\) 前缀外推。

---

## 9. 第二层正商有限证书

在 (8.4)、(8.8) 的严格有限范围内，生成器按下列顺序重建：

1. 完整 \(t\) 初段和尾窗 \(\mathcal H(a)\)；
2. \(x,c,U,D,r,k\) 的整数公式；
3. 五进阶、五进平方类、二进主室和精确大小门；
4. 第三层 \(v_0\) 上界、\(\epsilon=0\) 条件及 (6.6) 的全部 \(\ell\)；
5. 静态进位 \((w,u,v,E^*)\)；
6. 两步继承下降余项 \(E_2\) 与精确匹配。

只剩一个参数室：

\[
\boxed{
(a,t,h,J,v_0,\epsilon,A,F,q_*)
=(3,0,1,4,5,0,12,5,1).
}
\tag{9.1}
\]

其数据为

\[
r=4781249,
\qquad
E_2=2233076,
\qquad
p=64,
\qquad
1\le\ell\le3.
\]

完整三行如下。

| \(\ell\) | \(w\) | \(u\) | \(v\) | \(E^*\) | 删除原因 |
|---:|---:|---:|---:|---:|---|
| 1 | 44 | 2566 | 125293 | 8018751 | \(E^*>r\) |
| 2 | 24 | 1036 | 50586 | 3237502 | \(0<E^*<r\)，但 \(E^*\ne E_2\) |
| 3 | 4 | -494 | -24121 | -1543747 | 双商非负性和 \(E^*>0\) 失败 |

因此

\[
\boxed{
j=2,\quad\epsilon=0,\quad\ell>0
\Longrightarrow\text{无候选}.
}
\tag{9.2}
\]

独立验证器不导入生成器；它重新计算尾窗、提升初段、局部门、大小门、
三层上界、全部静态进位和下降余项，并检查阈值相邻、删除候选、篡改进位、
错误 \(\epsilon\) 与错误 CRT 余数破坏测试。规范输出为

```text
independently verified dual-corridor finite boundary: rooms=1 candidates=3 survivors=0
certificate_sha256=6ee20a53efdf09347c15b86da9dbd23e83050ad81af8a44c811a0ce27f7cc8f8
destruction tests: passed
```

SHA-256：

```text
critical_G_A2_high_phi_Fprimary_minus_dual_corridor_finite_generator.py
1d11bda188f6879366fd2055197484b2717fd20278dd01e6a48512f50902b509

critical_G_A2_high_phi_Fprimary_minus_dual_corridor_finite_verifier.py
8f6fb65d1ccd9058d84d0e688be47bd0fa2de3b5bebaead3fc8ef142bcd0da6d

critical_G_A2_high_phi_Fprimary_minus_dual_corridor_finite_certificate.json
6ee20a53efdf09347c15b86da9dbd23e83050ad81af8a44c811a0ce27f7cc8f8

critical_G_A2_high_phi_Fprimary_minus_dual_corridor_finite_certificate_bundle.tar.gz
fd3969506b0bbdf27631efeb590b6f5fae41e912daf2ec00f0dcd2b3cd903105
```

验证命令：

```bash
python3 critical_G_A2_high_phi_Fprimary_minus_dual_corridor_finite_verifier.py \
  critical_G_A2_high_phi_Fprimary_minus_dual_corridor_finite_certificate.json \
  --destruction-tests
```

---

## 10. 剩余八条进位递推族

第 2、5、9 节已经删除：

\[
A<2a,\ \ell>0;
\qquad
\epsilon=1,\ \ell>0;
\qquad
j=2,\epsilon=0,\ \ell>0.
\]

所以全部未决状态恰分为以下八族。

### 10.1 六条零商族

对每个可达

\[
(j,\epsilon)\in\{0,1,2\}\times\{0,1\},
\]

定义

\[
\boxed{\mathscr Z_{j,\epsilon}:\quad\ell=0.}
\tag{10.1}
\]

此时

\[
E^*=2^A5^F.
\tag{10.2}
\]

以 \(d=j+\epsilon\) 在 (6.7) 中作至多三步反向进位，并且只保留

\[
R_0=E_0.
\tag{10.3}
\]

这与继承的

\[
E_d=\left\langle B^{-d}E_0\right\rangle_r^+,
\qquad
E_d\equiv(-1)^dE_0^{d+1}\pmod r
\]

完全相容，但 (10.1)–(10.3) 是从已知终端 \(S\)-单位向初值回放的
显式整除进位，不再把“求一个移动模正余数”作为停止点。

### 10.2 两条无界正商族

只剩

\[
\boxed{
\mathscr P_0:\ (j,\epsilon)=(0,0),\ \ell>0,
}
\tag{10.4}
\]

\[
\boxed{
\mathscr P_1:\ (j,\epsilon)=(1,0),\ \ell>0.
}
\tag{10.5}
\]

两族分别代入

\[
A=2a-t+h+v_0,
\qquad
F=v_0+tj,
\qquad
q_*=2a-v_0-(j+1)t,
\]

然后用 (6.6) 生成完整有限 \(\ell\) 区间，以 (6.2)–(6.5) 生成
\((w,u,v,E^*)\)，最后用 (6.7)–(6.10) 双向恢复。

对每个固定 \((a,t,h,J,v_0,j)\)，\(\ell\) 区间严格有限且没有自由
CRT 选择；但其长度

\[
L=\min\left(5^F-1,
\left\lfloor\frac{2^{h+v_0-t}-1}
{J5^{2a-v_0-(j+1)t}}\right\rfloor\right)
\]

没有被本文统一有界。因此这两族仍覆盖无界 \(a\)，且尚未化成固定有限状态表。

六条 \(\mathscr Z\) 与两条 \(\mathscr P\) 互斥，并由 \(\ell=0/\ell>0\)、
\((j,\epsilon)\) 分室及前述删除定理穷尽全部 \(\mathcal F_{P-}\) 候选。

---

## 11. 回归反例的精确拒绝位置

继承反例状态为

\[
(a,t,h,J,v_0)=(3,0,1,4,5).
\]

它属于

\[
\boxed{(j,\epsilon,A,F,d)=(2,0,12,5,2).}
\tag{11.1}
\]

继承下降给

\[
E_2=2233076,
\qquad
5^F=3125,
\qquad
M=64.
\]

五进规范余数是

\[
\ell_*=E_2\bmod3125=1826.
\]

但

\[
E_2+\ell_*=2234902\equiv22\pmod{64}.
\]

因此

\[
v=\frac{E_2+\ell_*}{M}
\]

不是整数。该状态在精确走廊的 (3.1)，等价地在二进 CRT 门，立即失败。

从静态进位的另一方向看，(6.6) 只允许 \(\ell=1,2,3\)。其中唯一落在
\(0<E^*<r\) 的是 \(\ell=2\)，但

\[
E^*-E_2=3237502-2233076=1004426\ne0.
\]

这正好等于继承报告中的

\[
(P_2-E_2)-2r=1004426.
\]

所以新方法正确拒绝该状态，且完全没有使用已经被它否定的统一间隙

\[
0<P_2-E_2<r.
\]

---

## 12. 主动审计

### 12.1 是否把双商等式当作必要筛

没有。定理 6.1 从静态进位反向恢复

\[
2^A5^F=E^*+\ell r
\]

及两个规范 CRT 类；(6.7)–(6.10) 再恢复全部下降商和原终端变量。

### 12.2 是否遗漏 \(F=0,\ell=0\)

没有。\(F=0\) 时 \(5^F=1\)，(6.6) 没有正商；该状态完整进入相应
\(\mathscr Z_{j,\epsilon}\)。

### 12.3 是否把 \(\ell=0\) 自动判无解

没有。六条零商族仍开放，并保留 \(E^*=2^A5^F\) 的全部反向进位匹配。

### 12.4 是否用浮点数决定边界

没有。\(a\le5\) 和 \(a\le23\) 分别由 (8.3)、(8.7) 的整数幂比较及
相邻阈值推出。

### 12.5 有限证书是否承担无界 \(a\) 前缀

没有。第 8 节先符号证明第二层正商只有 \(a\le23\)；证书只重建该严格
有限集合。\(j=0,1\) 的无界族没有由有限样本外推。

### 12.6 是否得到固定有限状态自动机

没有。式 (3.6)、(7.4)–(7.6) 已把局部字母改成纯 \(2,5\) 进位，
但 \(w,u,v\) 和 (6.6) 的区间长度仍可随 \(a\) 增长。本文只声称有限条
递推族，不声称固定有限状态集合。

### 12.7 是否发现继承错误或合法原题解

均没有。GFPm-3 的反例被精确走廊正确拒绝；它仍只是否定旧的简单间隙路线。

---

## 13. 最终分类与停止点

本轮严格证明：

\[
\boxed{CU-MD=2,\qquad r=-1+CU=1+MD,}
\]

\[
\boxed{2^A=u+\ell5^{c_0-F}U,}
\]

\[
\boxed{2^{A-2a}5^F=v+\ell D,\qquad Mv-5^Fu=2\ell,}
\]

并将高二进走廊双向改写为

\[
\boxed{
w=2^{A-2a}-J\ell5^{c_0-F},
}
\]

\[
\boxed{
u=Mw-\ell5^{c_0-F}x,
\quad
v=5^Fw-\ell c,
\quad
E^*=M5^Fw-\ell\rho.
}
\]

此外：

\[
\boxed{A<2a\text{ 或 }\epsilon=1\Longrightarrow\ell=0,}
\]

\[
\boxed{j=2,\epsilon=0,\ell>0\Longrightarrow\text{无候选}.}
\]

全部未决状态恰为六条零商反向进位族和两条
\((j,\epsilon)=(0,0),(1,0)\) 正商静态进位族。它们覆盖全部无界 \(a\)，
但尚未被统一删除或压成绝对有限边界。

因此准确分类为

\[
\boxed{
\mathrm{GFPmR\text{-}3}:
\quad
\mathcal F_{P-}\text{ 被压成八条覆盖全部 }a\text{ 的明确进位递推族；}
\text{第二层正商已完整关闭，但零商及前两层正商仍开放。}
}
\]

没有找到合法原题解，也没有发现 GFPm-3 或其继承系统错误。本文到此停止，
不研究 \(\mathcal F_{E-}\)、\(\varphi<a\)、B、C、\(\gamma>1\)、
C2/C5、Q 或严格层。
