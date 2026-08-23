# 三项十进制拼接平方和问题：临界 G 模板 A2 高 \(\varphi\) 主二进室负符号族正商 \(j=0\) 报告

日期：2026-08-02（Asia/Tokyo）

本文严格限定于

\[
\boxed{
\mathscr P_0:
\quad j=0,\quad \epsilon=0,\quad d=0,\quad \ell>0.
}
\]

接受 GFPmR-3、GFPm-3、GFP-1、GA2H-2、GA2-6、PR6、SD6 与 v3
总账中和本分支相容的冻结结论。本文不研究 \(\mathscr P_1\)、六条零商族、
\(\mathcal F_{E-}\)、\(\varphi<a\)、B、C、\(\gamma>1\)、C2/C5、Q
或严格层。

本轮得到的主要推进是：

1. 题设的仿射坐标 \(H=J+\ell\) 确实把每个固定状态压成至多一个候选；
2. 正商条件本身进一步强迫
   \[
   \boxed{F\ge a+1,\qquad 5^F>10M;}
   \]
   因而题设要求讨论的 \(5^F<M\) 分室在 \(\mathscr P_0\) 中实际为空，
   \(h_5=0\) 分室也为空；
3. 规范 CRT 代表有一个不再含 \(\eta,\rho\) 的第二 Bezout 闭式：若
   \[
   I_{a,t,F}=\left\langle5^{-(c_0+F)}\right\rangle_{M^2/4}^{+},
   \]
   则
   \[
   \boxed{
   H_*=\frac{4I_{a,t,F}5^F-2x}{M}.
   }
   \]
4. 区间命中进一步强迫
   \[
   \boxed{I_{a,t,F}\le M/4-1.}
   \]
   这把全部残余精确定位为一个随 \(a\) 移动的高位二进 Bezout 数字；
5. 给出了覆盖全部 \(a\) 的有限数字递推。每个
   \((a,t,h,J,F)\) 只计算一个 \(I\)、一个 \(H_*\)、一个
   \(\ell\) 和一个 \(w_*\)，没有任何长度随 \(a\) 增长的自由
   \(\ell\) 枚举。

但是，现有继承链没有证明上述标准逆元始终大于 \(M/4\)，也没有把这一移动
高位数字化为固定有限状态或完整外部素数周期证书。因此本文不能诚实分类为
GFPmP0-1 或 GFPmP0-2。没有找到合法原题解，也没有发现 GFPmR-3、
GFPmZ-6 或其继承系统错误。最终分类为

\[
\boxed{\mathrm{GFPmP0\text{-}3}.}
\]

这里的无界残余已经是“每个递推状态至多一个显式整数候选”，而不是自由正商
区间。

---

## 1. 继承参数与直接终端等式

保留

\[
a\ge3,\qquad 0\le t<\frac a2,\qquad
h\in\mathcal H(a),\qquad J\in\{1,\ldots,9\},
\tag{1.1}
\]

\[
\mathcal H(a)=
\left\{h\ge0:
2^{2a-2}\le5^{h+1},\quad5^h<2^{2a-1}
\right\},
\tag{1.2}
\]

以及

\[
1\le h\le a-1,\qquad h\ge t,
\tag{1.3}
\]

\[
125^t<22\cdot2^{2a-1}.
\tag{1.4}
\]

置

\[
M=2^{2a},\qquad c_0=2a-t,\qquad C=5^{c_0},\qquad B=MC,
\tag{1.5}
\]

\[
x=\left\langle2C^{-1}\right\rangle_M,
\qquad Cx=2+Mc,
\tag{1.6}
\]

\[
\rho=Cx-1=1+Mc,\qquad \eta=cx,
\tag{1.7}
\]

\[
U=x+MJ,\qquad D=c+CJ.
\tag{1.8}
\]

于是

\[
\boxed{CU-MD=2,}
\tag{1.9}
\]

\[
\boxed{r=-1+CU=1+MD,}
\tag{1.10}
\]

并沿用

\[
k=-1+C\left(U+\frac M2\right)=r+\frac B2.
\tag{1.10a}
\]

\[
\boxed{E_0=\eta+\rho J=cU+J=xD-J.}
\tag{1.11}
\]

同时保留全部局部门

\[
v_5\!\left(U+\frac M2\right)=3t,
\tag{1.12}
\]

\[
W=\frac{U+M/2}{5^{3t}},\qquad
-2W\equiv1\ \text{或}\ 4\pmod5,
\tag{1.13}
\]

\[
v_2(k^2-1)=2a,\qquad
\frac{k^2-1}{2^{2a}}\equiv3\ \text{或}\ 7\pmod8.
\tag{1.14}
\]

本室中

\[
F=v_0,\qquad A=2a-t+h+F,
\qquad 0\le F<c_0,
\tag{1.15}
\]

\[
s=c_0-F\ge1,
\qquad p=2^{A-2a}=2^{h+F-t}.
\tag{1.16}
\]

正商区间为

\[
1\le\ell\le
L=
\min\left(
5^F-1,
\left\lfloor\frac{p-1}{J5^s}\right\rfloor
\right),
\tag{1.17}
\]

并定义

\[
w=p-J\ell5^s>0.
\tag{1.18}
\]

因 \(d=0\)，继承终端条件没有任何模余数回放，而是直接等式

\[
\boxed{
M5^Fw-\ell\rho=E_0.
}
\tag{1.19}
\]

这一定量事实是后文全部双向性的起点。

---

## 2. 仿射坐标与唯一 CRT 候选

定义

\[
\boxed{H=J+\ell.}
\tag{2.1}
\]

由 (1.19) 和 (1.11)，

\[
M5^Fw-\ell\rho=\eta+\rho J
\]

严格等价于

\[
\boxed{M5^Fw=\eta+\rho H.}
\tag{2.2}
\]

正商的五进规范窗给

\[
\boxed{J+1\le H\le J+5^F-1.}
\tag{2.3}
\]

由

\[
\rho^2=1+B\eta
\]

及 \(M5^F\mid B\)，有

\[
\gcd(\rho,M5^F)=1,
\qquad
\rho^{-1}\equiv\rho\pmod{M5^F}.
\tag{2.4}
\]

因此 (2.2) 强迫

\[
\boxed{H\equiv-\eta\rho\pmod{M5^F}.}
\tag{2.5}
\]

记其最小非负代表为

\[
\boxed{
H_*=\left\langle-\eta\rho\right\rangle_{M5^F}
\in\{0,\ldots,M5^F-1\}.
}
\tag{2.6}
\]

因 (2.3) 的长度为 \(5^F-1<M5^F\)，每个固定
\((a,t,h,J,F)\) 至多有一个候选。若命中，则唯一恢复

\[
\boxed{\ell=H_*-J.}
\tag{2.7}
\]

当 \(F=0\) 时，(2.3) 为空；故

\[
\boxed{F=0\Longrightarrow\mathscr P_0\text{ 自动为空}.}
\tag{2.8}
\]

---

## 3. 纯二进—纯五进拆分与规范 CRT 闭式

因为

\[
\rho\equiv1\pmod M,
\qquad
\rho\equiv-1\pmod{5^F},
\]

(2.5) 严格拆成

\[
\boxed{H\equiv-\eta\pmod M,}
\tag{3.1}
\]

\[
\boxed{H\equiv\eta\pmod{5^F}.}
\tag{3.2}
\]

定义

\[
h_2=\langle-\eta\rangle_M,
\qquad
h_5=\langle\eta\rangle_{5^F}.
\tag{3.3}
\]

两种完全等价的规范 CRT 闭式为

\[
\boxed{
H_*=h_5+5^F
\left\langle
(h_2-h_5)(5^F)^{-1}
\right\rangle_M,
}
\tag{3.4}
\]

\[
\boxed{
H_*=h_2+M
\left\langle
(h_5-h_2)M^{-1}
\right\rangle_{5^F}.
}
\tag{3.5}
\]

这里两个同余必须同时使用；单独的 (3.1) 或 (3.2) 都不是充分条件。

若暂不使用正商大小，(3.4) 已给出题设四个分室的精确字典：

1. 当 \(5^F<M\) 时，优先使用 (3.5)，小区间命中由
   \(h_2\) 及一个五进进位决定；
2. 当 \(5^F\ge M\) 时，优先使用 (3.4)，写
   \[
   q_F=
   \left\langle
   (h_2-h_5)(5^F)^{-1}
   \right\rangle_M;
   \tag{3.6}
   \]
   则 \(H_*=h_5+q_F5^F\)；
3. \(h_5=0\) 等价于 \(5^F\mid\eta\)；
4. \(h_2\le J+5^F-1\) 只是二进必要门；其补集可立即拒绝，但前者仍须
   通过五进 CRT 进位。

第 4 节将证明，\(\mathscr P_0\) 实际只进入第 2 室，并把第 3 室
整体删除。

---

## 4. 正商强迫 \(F\ge a+1\) 与 \(5^F>10M\)

### 4.1 两个统一斜率界

先由尾窗证明

\[
\boxed{h<\frac{7a}{8}.}
\tag{4.1}
\]

若反之 \(8h\ge7a\)，则

\[
5^{8h}\ge5^{7a}>2^{16a},
\]

其中 \(5^7=78125>65536=2^{16}\)；但尾窗又给

\[
5^{8h}<2^{16a-8}<2^{16a},
\]

矛盾。

其次，继承提升界 (1.4) 强迫

\[
\boxed{t\le\frac a3.}
\tag{4.2}
\]

对 \(a\ge11\)，若 \(3t>a\)，把 (1.4) 立方得到

\[
125^{3t}<22^3\,2^{6a-3},
\]

从而

\[
\left(\frac{125}{64}\right)^a<1331.
\]

但在 \(a=11\) 已有精确反向比较

\[
125^{11}
=116415321826934814453125
>
98210465448429652803584
=1331\cdot64^{11},
\]

以后左、右比值每步再乘 \(125/64>1\)，矛盾。对
\(3\le a\le10\)，由 (1.4) 的直接整数端点分别得到最大

\[
T_a=1,1,1,2,2,2,3,3,
\]

也都满足 \(3T_a\le a\)。故 (4.2) 对全部 \(a\ge3\) 成立。

### 4.2 正商五进指数的统一下界

若 \(\ell>0\)，由 \(w>0\) 及整数性，

\[
p>J\ell5^s\ge5^s.
\tag{4.3}
\]

反设 \(F\le a\)。由 (4.1)、(4.2)，

\[
\begin{aligned}
\frac{p}{5^s}
&=\frac{2^{h+F-t}}{5^{2a-t-F}}\\
&<\frac{2^{15a/8-t}}{5^{a-t}}\\
&\le
\frac{2^{15a/8-a/3}}{5^{a-a/3}}
=\frac{2^{37a/24}}{5^{2a/3}}<1,
\end{aligned}
\tag{4.4}
\]

最后一步来自

\[
2^{37}=137438953472
<152587890625=5^{16}.
\]

这与 (4.3) 矛盾。因此

\[
\boxed{F\ge a+1.}
\tag{4.5}
\]

当 \(a\ge4\) 时，

\[
5^F\ge5^{a+1}
=5\left(\frac54\right)^aM
>10M.
\tag{4.6}
\]

只剩 \(a=3\) 需核对。此时 (1.4) 只允许 \(t=0,1\)。完整局部门
(1.12)–(1.14) 在 \(t=0\) 只留下 \(J=4\)，而 \(t=1\) 没有
局部状态。对 \(t=0,J=4,F=4\)，即使取最大的尾窗值 \(h=2\)，

\[
p=64<4\cdot5^2=100,
\]

故没有正商；正商只能有 \(F=5\)，此时

\[
5^F=3125>640=10M.
\]

综上，全部 \(\mathscr P_0\) 状态都满足

\[
\boxed{F\ge a+1,\qquad5^F>10M.}
\tag{4.7}
\]

所以题设的 \(5^F<M\) 分室在本族中严格为空。

---

## 5. 五进低块与唯一零高位进位

由 \(F<c_0\)，模 \(5^F\) 有

\[
Mc=Cx-2\equiv-2.
\]

又 \(5\nmid c\)，因为 \(M\) 是五进单位。若
\(h_5=\langle\eta\rangle_{5^F}\)，则

\[
Mh_5+2x\equiv M\eta+2x
=Mcx+2x\equiv0\pmod{5^F}.
\tag{5.1}
\]

若 \(0\le h_5\le8\)，由 \(0<x<M\) 和 (4.7)，

\[
0<Mh_5+2x<10M<5^F,
\]

与 (5.1) 矛盾。因此

\[
\boxed{h_5\ge9.}
\tag{5.2}
\]

这特别证明

\[
\boxed{h_5=0\text{ 分室为空}.}
\tag{5.3}
\]

现在使用 (3.4)：

\[
H_*=h_5+q_F5^F,
\qquad0\le q_F<M.
\tag{5.4}
\]

若命中 (2.3)，则 \(H_*\le5^F+8\)。由 (5.2)：

- \(q_F\ge2\) 时，\(H_*>2\cdot5^F>5^F+8\)；
- \(q_F=1\) 时，命中要求 \(h_5\le8\)，与 (5.2) 矛盾。

故候选必须满足

\[
\boxed{q_F=0,\qquad H_*=h_5.}
\tag{5.5}
\]

这已经把小区间 CRT 命中压成一个明确的“最高五进块进位为零”条件；但
\(q_F\) 仍是随 \(a\) 移动的高位二进数字，不能由固定低位状态恢复。

---

## 6. 第二 Bezout 闭式：直接恢复 \(H_*\)

令

\[
\mathfrak M_a=\frac{M^2}{4}=2^{4a-2},
\tag{6.1}
\]

并定义唯一正标准逆元

\[
\boxed{
I_{a,t,F}
=\left\langle5^{-(c_0+F)}\right\rangle_{\mathfrak M_a}^{+}
\in\{1,\ldots,\mathfrak M_a-1\}.
}
\tag{6.2}
\]

### 定理 6.1

规范 CRT 代表 (2.6) 有闭式

\[
\boxed{
H_*=\frac{4I_{a,t,F}5^F-2x}{M}.
}
\tag{6.3}
\]

#### 证明

由 (6.2)，

\[
5^{c_0+F}\,4I_{a,t,F}\equiv4\pmod{M^2}.
\tag{6.4}
\]

先模 \(M\) 使用 \(Cx\equiv2\)，得到

\[
C(4I_{a,t,F}5^F)\equiv4\equiv C(2x)\pmod M.
\]

因 \(C\) 为模 \(M\) 单位，(6.3) 的右端是整数；记它为
\(\widetilde H\)。将

\[
4I_{a,t,F}5^F=M\widetilde H+2x
\tag{6.5}
\]

代回 (6.4)，并用 \(Cx=2+Mc\)，得到

\[
C(M\widetilde H+2x)-4
=M(C\widetilde H+2c)\equiv0\pmod{M^2}.
\]

故

\[
\widetilde H\equiv-2cC^{-1}\equiv-cx=-\eta\pmod M.
\tag{6.6}
\]

另一方面，(6.5) 模 \(5^F\) 给

\[
M\widetilde H\equiv-2x\pmod{5^F}.
\]

而 \(Mc\equiv-2\pmod{5^F}\)，所以

\[
M\eta=Mcx\equiv-2x\pmod{5^F},
\]

从而

\[
\widetilde H\equiv\eta\pmod{5^F}.
\tag{6.7}
\]

又因 \(0<I_{a,t,F}<M^2/4\)，有 \(\widetilde H<M5^F\)。若
\(\widetilde H<0\)，由 (6.3) 只能有 \(-2<\widetilde H<0\)；但
(6.6) 说明 \(\widetilde H\) 与偶数 \(-\eta\) 同奇偶，故不可能是
唯一整数 \(-1\)。于是

\[
0\le\widetilde H<M5^F.
\]

(6.6)–(6.7) 与标准区间唯一性证明 \(\widetilde H=H_*\)。\(\square\)

### 6.2 小区间命中的高位逆元障碍

若 (2.3) 命中，则 \(H_*\le5^F+8\)。由 (6.3)、\(x<M\) 与
(4.7)，

\[
\begin{aligned}
4I_{a,t,F}5^F
&=MH_*+2x\\
&<M5^F+10M,
\end{aligned}
\]

故

\[
I_{a,t,F}<\frac M4+\frac{10M}{4\cdot5^F}
<\frac M4+\frac14.
\]

由于 \(I_{a,t,F}\) 是奇数，而 \(M/4\) 是偶数，候选必要条件严格为

\[
\boxed{
1\le I_{a,t,F}\le\frac M4-1.
}
\tag{6.8}
\]

这就是本轮的准确停止障碍：要统一删除 \(\mathscr P_0\)，只需证明全部
允许 \((a,t,F)\) 满足

\[
\left\langle5^{-(2a-t+F)}\right\rangle_{2^{4a-2}}^{+}
>2^{2a-2},
\tag{6.9}
\]

但现有材料没有这一移动高位逆元不等式。

---

## 7. 第二套 Bezout 坐标与高位数字的等价来源

定义

\[
V_H=x+MH,
\qquad
D_H=c+CH.
\tag{7.1}
\]

直接计算得

\[
\boxed{CV_H-MD_H=2.}
\tag{7.2}
\]

而 (2.2) 等价于

\[
\boxed{M5^Fw=cV_H+H.}
\tag{7.3}
\]

与原始 Bezout 对的差分为

\[
\boxed{V_H-U=M\ell,\qquad D_H-D=C\ell.}
\tag{7.4}
\]

由 (3.1)–(3.2)，唯一存在正整数

\[
z_5=\frac{MH+2x}{5^F},
\qquad
z_2=\frac{CH+2c}{M}.
\tag{7.5}
\]

两式作交叉消去：

\[
\begin{aligned}
C(MH+2x)-M(CH+2c)
&=2(Cx-Mc)=4.
\end{aligned}
\]

所以

\[
\boxed{C5^Fz_5-M^2z_2=4.}
\tag{7.6}
\]

候选中 \(H\) 为偶数、\(v_2(x)=1\)，故 \(v_2(z_5)=2\)。写
\(z_5=4I\)，(7.6) 除以 \(4\) 后正是

\[
5^{c_0+F}I-\frac{M^2}{4}z_2=1.
\tag{7.7}
\]

由小区间和 (4.7)，\(0<z_5\le M\)，所以
\(0<I\le M/4\)；规范唯一性随即给 \(I=I_{a,t,F}\)。因此第二
Bezout 坐标没有产生一个只依赖 \(\ell\) 的下降；它精确重现了 (6.8)
的移动高位逆元数字。这证明障碍不是选取 \(H\) 坐标时引入的人为现象。

---

## 8. 唯一候选的精确等式与双向性

若 \(H_*\) 通过 (2.3)，定义

\[
\ell=H_*-J.
\tag{8.1}
\]

由 (2.5)，

\[
\boxed{
w_*=\frac{\eta+\rho H_*}{M5^F}
\in\mathbb Z_{>0}.
}
\tag{8.2}
\]

唯一需要检查的完整等式是

\[
\boxed{
w_*
=2^{h+F-t}
-J(H_*-J)5^{2a-t-F}.
}
\tag{8.3}
\]

等价地，

\[
\boxed{
\eta+\rho H_*
=M5^F\left[
2^{h+F-t}
-J(H_*-J)5^{2a-t-F}
\right].
}
\tag{8.4}
\]

### 定理 8.1

\[
\boxed{(2.3)+(8.3)}
\]

与原来的

\[
E^*=E_0,qquad1\le\ell\le L
\]

严格双向等价。

#### 正向

原候选给 \(H=J+\ell\)、(2.2) 和 (2.5)。由标准代表唯一性
\(H=H_*\)，于是 (2.3)、(8.2)–(8.3) 全部成立。

#### 反向

(2.3) 给

\[
1\le\ell=H_*-J\le5^F-1.
\]

由 (8.2) 有 \(w_*>0\)。若 (8.3) 成立，则

\[
p-J\ell5^s=w_*>0.
\]

因全部量为整数，

\[
J\ell5^s\le p-1,
\]

故

\[
\ell\le
\left\lfloor\frac{p-1}{J5^s}\right\rfloor.
\]

联合五进上界即得 \(1\le\ell\le L\)。最后从

\[
M5^Fw_*=\eta+\rho H_*
\]

减去 \(\ell\rho\)，得到

\[
M5^Fw_*-\ell\rho
=\eta+\rho J=E_0.
\]

所以原静态走廊和直接终端等式全部恢复。\(\square\)

---

## 9. 覆盖全部 \(a\) 的有限递推

本节明确给出 GFPmP0-3 所要求的无界完备递推；它不枚举 \(\ell\)。

### 9.1 尾窗与提升初段

令

\[
H_a=\max\{h:5^h<2^{2a-1}\}.
\]

则 \(H_3=2\)，并且

\[
H_{a+1}=
\begin{cases}
H_a+1,&5^{H_a+1}<2^{2a+1},\\
H_a,&\text{否则}.
\end{cases}
\tag{9.1}
\]

随后

\[
\mathcal H(a)
=\{H_a\}\cup
\{H_a-1:5^{H_a}\ge2^{2a-2}\}.
\tag{9.2}
\]

令

\[
T_a=\max\{t:125^t<22\cdot2^{2a-1}\}.
\]

则 \(T_3=1\)，且

\[
T_{a+1}\in\{T_a,T_a+1\},
\tag{9.3}
\]

由下一幂是否满足严格不等式唯一决定；再与 \(t<a/2\) 及 \(h\ge t\)
相交。

### 9.2 低精度逆元 \(x\)

令

\[
P_a=\left\langle5^{-2a}\right\rangle_{4^a},
\qquad P_3=57.
\tag{9.4}
\]

若

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
=\left\langle25^{-1}\widehat P_a\right\rangle_{4^{a+1}}.
}
\tag{9.5}
\]

对允许的 \(t\)，

\[
\boxed{x_{a,t}=\left\langle2\cdot5^tP_a\right\rangle_{4^a}.}
\tag{9.6}
\]

### 9.3 高精度 Bezout 逆元

置

\[
\mathfrak M_a=2^{4a-2},
\qquad
g_a=\langle5^{-1}\rangle_{\mathfrak M_a}.
\tag{9.7}
\]

基值为

\[
\mathfrak M_3=1024,
\qquad g_3=205.
\]

若

\[
5g_a=1+e_a\mathfrak M_a,
\]

取唯一 \(d_a\in\{0,\ldots,15\}\) 使

\[
e_a+5d_a\equiv0\pmod{16},
\]

则

\[
\boxed{g_{a+1}=g_a+d_a\mathfrak M_a}
\tag{9.8}
\]

是 \(5^{-1}\) 模 \(\mathfrak M_{a+1}=16\mathfrak M_a\) 的标准代表。

固定 \(a\) 后，定义

\[
R_{a,1}=g_a,
\qquad
\boxed{
R_{a,K+1}=\langle g_aR_{a,K}\rangle_{\mathfrak M_a}.
}
\tag{9.9}
\]

归纳即得

\[
R_{a,K}=\langle5^{-K}\rangle_{\mathfrak M_a}.
\]

所以本报告所需的唯一高位数字为

\[
\boxed{I_{a,t,F}=R_{a,,2a-t+F}.}
\tag{9.10}
\]

### 9.4 每个状态的无枚举判别

对每个 \(a\ge3\)，递推执行：

1. 由 (9.1)–(9.3) 生成全部 \((t,h)\)；
2. 由 (9.4)–(9.6) 生成 \(x,c,\rho,\eta\)；
3. 对九个 \(J\) 检查 (1.12)–(1.14)；
4. 只取
   \[
   a+1\le F\le2a-t-1;
   \]
5. 先检查正商区间非空，即 \(L\ge1\)；
6. 由 (9.10)、(6.3) 只计算一个 \(I\) 和一个 \(H_*\)；
7. 若 \(H_*\notin[J+1,J+5^F-1]\)，拒绝；否则唯一置
   \(\ell=H_*-J\)；
8. 计算唯一 \(w_*\)，只检查 (8.3)；
9. 若成立，直接回代 (1.18)–(1.19) 及全部继承门。

每个状态没有自由 CRT 选择、自由 \(\ell\)、自由提升深度或移动模 \(r\)
余数搜索。递推覆盖全部 \(a\)，但状态数仍随 \(a\) 增长，且
\(I_{a,t,F}\) 的被询问二进位区间也随 \(a\) 向高位移动。

---

## 10. 精确计算诊断（不承担无界证明）

为攻击端点、符号和公式错误，使用两条独立整数路径检查
\(3\le a\le150\)：

1. 直接计算
   \[
   H_*=\langle-\eta\rho\rangle_{M5^F};
   \]
2. 独立计算
   \[
   I=\langle5^{-(c_0+F)}\rangle_{M^2/4}^{+},
   \qquad
   H_*=(4I5^F-2x)/M.
   \]

两路在全部状态上逐项相同。保留全部局部门、尾窗和正商边界后的计数为

```text
raw local (a,t,h,J,F) states = 59302
states with nonempty positive corridor = 24986
states with I <= M/4 = 0
CRT interval hits = 0
full E2 hits = 0
```

这组有限前缀只用于实现和公式诊断；本文没有把它外推为
\(a\ge151\) 的证明，也没有据此制作“规范证书包”。

---

## 11. 主动审计

### 11.1 是否遗漏 \(F=0\)

没有。\(F=0\) 时 (2.3) 为空，故正商自动为空。

### 11.2 是否把 \(H_*\) 的唯一性误写成存在性

没有。唯一性来自区间长度小于模数；存在仍须检查 (2.3) 和 (8.3)。

### 11.3 是否把 C2 或 C5 单独当成充分条件

没有。(3.4)–(3.5) 始终同时恢复两个同余；第 6 节也逐项重建二者。

### 11.4 是否遗漏原来的第二个正商上界

没有。(8.3) 给 \(w_*>0\)，从而严格恢复

\[
\ell\le\left\lfloor\frac{p-1}{J5^s}\right\rfloor.
\]

所以 (2.3)+(8.3) 恢复的是完整 \(L\)，不只是 \(\ell<5^F\)。

### 11.5 是否把 \(5^F<M\) 的空性建立在数值样本上

没有。第 4 节用 (4.1)–(4.5) 对全部 \(a\) 符号证明
\(F\ge a+1\)，并只对唯一小端 \(a=3\) 作完整局部门整数核对。

### 11.6 是否把有限前缀当成无界证书

没有。第 10 节明确只属于诊断。无界完备性来自第 9 节递推；空性尚未证明。

### 11.7 是否发现继承错误

没有。题设的 H2、C2/C5、E2 与 GFPmR-3 的静态双走廊完全相容。
新增的是更强的 (4.7)、(5.5)、(6.3) 和 (6.8)，不是对继承结论的修正。

### 11.8 为什么不生成周期证书

现存条件 (6.9) 询问的是

\[
5^{-(2a-t+F)}\bmod2^{4a-2}
\]

中随 \(a\) 移动的整块高位数字。第 9 节给出有限数字递推，但没有得到固定
有限状态集合，也没有找到一个外部素数周期能双向决定不等式 (6.9)。有限
\(a\) 前缀不能承担这个无界结论，故不制作伪周期证书。

---

## 12. 最终分类与停止点

本轮严格证明

\[
\boxed{
\begin{gathered}
F\ge a+1,\qquad5^F>10M;\\
H_*=h_5+q_F5^F,\qquad
\text{区间命中}\Longrightarrow q_F=0;\\
I_{a,t,F}
=\left\langle5^{-(2a-t+F)}\right\rangle_{2^{4a-2}}^{+};\\
H_*=\dfrac{4I_{a,t,F}5^F-2x}{M};\\
\text{区间命中}\Longrightarrow
1\le I_{a,t,F}\le2^{2a-2}-1;\\
w_*=\dfrac{\eta+\rho H_*}{M5^F},\\
(2.3)+(8.3)
\Longleftrightarrow
E^*=E_0,\quad1\le\ell\le L.
\end{gathered}
}
\tag{12.1}
\]

第 9 节给出了覆盖全部 \(a\) 的有限递推；每个
\((a,t,h,J,F)\) 至多产生一个显式整数候选，且不再枚举 \(\ell\)。

但是，尚未证明标准逆元 (6.2) 永远不落入 (6.8)；\(a\) 未绝对有界；
也没有完整周期模证书。因此准确分类为

\[
\boxed{
\mathrm{GFPmP0\text{-}3}:
\quad
\mathscr P_0\text{ 的每个递推状态至多一个候选，并有覆盖全部 }a
\text{ 的有限递推，但仍有无界高位 Bezout 残余。}
}
\tag{12.2}
\]

没有找到合法原题解，也没有发现 GFPmR-3、GFPmZ-6 或继承系统错误。

本文到此停止，不研究
\(\mathscr P_1\)、六条零商族、\(\mathcal F_{E-}\)、\(\varphi<a\)、
B、C、\(\gamma>1\)、C2/C5、Q 或严格层。
