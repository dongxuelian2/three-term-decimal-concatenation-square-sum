# 三项十进制拼接平方和问题：临界 G 模板 A2 高 \(\varphi\) 主二进室负符号族零商报告

日期：2026-08-01（Asia/Tokyo）

本文严格限定于

\[
\boxed{
\mathscr Z=
\bigcup_{j=0}^{2}\bigcup_{\epsilon=0}^{1}
\mathscr Z_{j,\epsilon}
}
\]

即 `critical_G_A2_high_phi_Fprimary_minus_dual_corridor_campaign.md`
留下的六条零商族。本文不研究
\(\mathscr P_0,\mathscr P_1\)、\(\mathcal F_{E-}\)、\(\varphi<a\)、
B、C、\(\gamma>1\)、C2/C5、Q 或严格层。

接受 GFPmR-3、GFPm-3、GFP-1、GA2H-2、GA2-6、PR6、SD6 与 v3
总账中和本分支相容的冻结结论。

本轮严格完成了下列推进。

1. 逐项核对了题设的三个 \(E_0\) 表达式以及全部 Bezout、反向回放、
   对偶进位与幂同余公式。
2. 把零商的确定性反向回放写成完整双向定理，并给出
   \((P_i,Q_i)\) 的严格符号窗口；其中 \(Q_i\) 确实允许为负。
3. 对深度零，得到一个比 \(M\mid 2c+CJ\) 更精确的“下一高位逆元数字”
   等价式：零商必须使 \(C^{-1}\) 从模 \(M/2\) 提升到模 \(M^2/4\)
   时的新基 \(M/2\) 数字恰为 \(J/2\in\{1,3\}\)。
4. 对深度一，完全消去移动模数 \(r\)，把继承余项 \(E_1\) 写成固定
   二次型
   \[
   E_1=s_1+p_1J-J^2,
   \qquad p_1^2+4s_1=n_1m_1,
   \]
   其中 \((n_1,m_1)\) 是与 \(J\) 无关的唯一平方 Bezout 对。
5. 对深度二、三，得到只有一个二值高位进位的双坐标商公式，并给出
   其二进、五进字母。

但是，这些结果没有把六室全部删除，也没有把剩余状态压成绝对有限边界或
题设所要求的固定有限自动机。决定性障碍已经定位：深度零所需的逆元数字位于
随 \(a\) 线性向高位移动的区间；固定的
\(P_i\bmod2^s,Q_i\bmod5^s\) 不包含该数字。深度一的二次型系数也正是同一
移动高位 Bezout 数据。现有继承链没有给出这些高位数字的统一界、周期或有限状态
递推。

因此不能诚实分类为 GFPmZ-1、GFPmZ-2 或 GFPmZ-3；没有发现合法原题解，
也没有发现 GFPmR-3 或继承系统错误。给定分级没有单列“有结构推进但未达到
固定有限化”这一中间档。为避免把移动高位数据冒充有限自动机，本轮保守记为

\[
\boxed{\mathrm{GFPmZ\text{-}6}.}
\]

这里的 GFPmZ-6 是按交付门槛记录“没有达到六族的全局关闭、绝对有限化或
固定有限自动机”；按其字面短语，本文又确实增加了下述高位 Bezout 正规形。
这个分级空档在结论中明确保留，不用较强标签掩盖。

---

## 1. 参数与三个初值表达式

全部结论均保留继承参数域

\[
a\ge3,\qquad
0\le t<\frac a2,\qquad
h\in\mathcal H(a),\qquad
J\in\{1,\ldots,9\},
\tag{1.0a}
\]

其中

\[
\mathcal H(a)=
\left\{h\ge0:
2^{2a-2}\le5^{h+1},\quad5^h<2^{2a-1}
\right\},
\qquad
1\le h\le a-1,
\qquad h\ge t.
\tag{1.0b}
\]

同时保留 GA2H-2/GFPm-3 的局部门

\[
125^t<22\cdot2^{2a-1},
\qquad
v_5\!\left(U+\frac M2\right)=3t,
\tag{1.0c}
\]

\[
W=\frac{U+M/2}{5^{3t}},
\qquad
-2W\equiv1\ \text{或}\ 4\pmod5,
\tag{1.0d}
\]

以及对

\[
k=-1+C\left(U+\frac M2\right)=r+\frac B2
\]

成立的

\[
v_2(k^2-1)=2a,
\qquad
\frac{k^2-1}{2^{2a}}\equiv3\ \text{或}\ 7\pmod8.
\tag{1.0e}
\]

下文的等价式是在这个完整参数域内成立；没有把局部门放松成更大的候选集。

置

\[
M=2^{2a},\qquad
C=5^{c_0},\qquad
c_0=2a-t,\qquad
B=MC,
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
D=CJ+c.
\tag{1.3}
\]

于是

\[
CU=CJM+Cx=M(CJ+c)+2=MD+2,
\]

故

\[
\boxed{CU-MD=2.}
\tag{1.4}
\]

负符号主室给出

\[
\boxed{r=-1+CU=1+MD.}
\tag{1.5}
\]

再置

\[
\rho=Cx-1=1+Mc,
\qquad
\eta=cx.
\tag{1.6}
\]

题设要求核对的三个表达式确实逐项相同：

\[
\begin{aligned}
\eta+\rho J
&=cx+(Cx-1)J\\
&=x(CJ+c)-J\\
&=xD-J,
\end{aligned}
\tag{1.7}
\]

而

\[
\begin{aligned}
(xD-J)-(cU+J)
&=x(CJ+c)-J-c(JM+x)-J\\
&=J(Cx-Mc-2)=0.
\end{aligned}
\tag{1.8}
\]

因此

\[
\boxed{
E_0=\eta+\rho J=cU+J=xD-J.
}
\tag{1.9}
\]

还保留两个以后反复使用的单位恒等式：

\[
\rho^2=1+B\eta,
\tag{1.10}
\]

\[
\rho r
=(\rho^2)+B\rho J
=1+B(\eta+\rho J)
=1+BE_0.
\tag{1.11}
\]

特别地

\[
\boxed{BE_0\equiv-1\pmod r,}
\qquad
\boxed{\gcd(E_0,r)=1.}
\tag{1.12}
\]

另由 (1.9) 与 (1.5)，

\[
\rho E_0-J=\eta r.
\tag{1.13}
\]

---

## 2. 六个室及严格指数边界

写

\[
\nu=2aj+v_0,
\qquad
j\in\{0,1,2\},
\qquad
0\le v_0<2a.
\tag{2.1}
\]

下降前

\[
A_j=2a-t+h+v_0,
\qquad
F_j=v_0+tj.
\tag{2.2}
\]

若 \(F_j<c_0\)，则 \(\epsilon=0\)；若 \(F_j\ge c_0\)，则
\(\epsilon=1\) 并再作一次 \(B\)-下降。完整表为

\[
\boxed{
\begin{array}{c|c|c|c}
(j,\epsilon)&d&A&F\\ \hline
(0,0)&0&2a-t+h+v_0&v_0\\
(1,0)&1&2a-t+h+v_0&v_0+t\\
(2,0)&2&2a-t+h+v_0&v_0+2t\\
(0,1)&1&h+v_0-t&v_0+t-2a\\
(1,1)&2&h+v_0-t&v_0+2t-2a\\
(2,1)&3&h+v_0-t&v_0+3t-2a
\end{array}}
\tag{2.3}
\]

其中

\[
\boxed{
\epsilon=0\iff v_0+(j+1)t<2a,
}
\tag{2.4}
\]

\[
\boxed{
\epsilon=1\iff v_0+(j+1)t\ge2a.
}
\tag{2.5}
\]

所有 \(F\) 均非负。对 \(\epsilon=0\) 这是显然的；对
\(\epsilon=1\)，(2.5) 正好给

\[
F=v_0+(j+1)t-2a\ge0.
\]

由继承的

\[
h\ge t,
\qquad
t<\frac a2,
\tag{2.6}
\]

得到严格二进下界。

当 \(\epsilon=0\) 时，

\[
\boxed{A=2a+(h-t)+v_0\ge2a.}
\tag{2.7}
\]

当 \(\epsilon=1\) 时，使用 (2.5)：

\[
A=h+v_0-t
\ge2a+h-(j+2)t.
\tag{2.8}
\]

所以三个溢出室分别满足

\[
\boxed{
\begin{array}{c|c}
j&A\text{ 的严格下界}\\ \hline
0&A\ge2a+h-2t\ge2a-t>3a/2\\
1&A\ge2a+h-3t\ge2a-2t>a\\
2&A\ge2a+h-4t\ge2a-3t>a/2
\end{array}}
\tag{2.9}
\]

这明确保留了 \(\epsilon=1\) 时 \(A<2a\) 的可能性，但保证
\(A>0\)。下降深度始终为

\[
\boxed{d=j+\epsilon\le3.}
\tag{2.10}
\]

当 \(j=2\) 时还保留继承的第三层精确上界

\[
0\le v_0\le
\begin{cases}
a+3-h,&t=0,\\
a+t+2-h,&t\ge1.
\end{cases}
\tag{2.11}
\]

并且六室全部满足

\[
\boxed{0\le F<c_0.}
\tag{2.12}
\]

零商终端值记为

\[
\boxed{R_d=S=2^A5^F.}
\tag{2.13}
\]

---

## 3. 确定性反向回放的双向定理

### 定理 3.1

固定一个六室参数状态，并令 \(S=2^A5^F\)。若 \(S\notin(0,r)\)，
立即拒绝；以下假设 \(0<S<r\)。从

\[
R_d=S
\]

开始，对 \(i=d-1,d-2,\ldots,0\) 定义

\[
\boxed{
\kappa_i=\left\lfloor\frac{BR_{i+1}}r\right\rfloor,
}
\tag{3.1}
\]

\[
\boxed{
R_i=BR_{i+1}-\kappa_i r.
}
\tag{3.2}
\]

则每一步都有

\[
\boxed{0\le\kappa_i<B,\qquad0\le R_i<r.}
\tag{3.3}
\]

若某一步 \(R_i=0\)，该状态不可能为继承候选。否则零商候选存在当且仅当

\[
\boxed{R_0=E_0.}
\tag{3.4}
\]

若 (3.4) 成立，令

\[
L_d=0,
\qquad
L_i=\kappa_i+BL_{i+1},
\tag{3.5}
\]

则

\[
\boxed{
N=E_0+L_0r=B^dS,
}
\tag{3.6}
\]

并唯一恢复

\[
\boxed{
q=\rho+BL_0,
\qquad
s=\eta+\rho L_0,
\qquad
0<s<q.
}
\tag{3.7}
\]

#### 证明

由 \(0<R_{i+1}<r\)，

\[
0<\frac{BR_{i+1}}r<B,
\]

所以 (3.1) 给 \(0\le\kappa_i<B\)，而 (3.2) 正是欧几里得余数，
自动给 \(0\le R_i<r\)。

若状态来自继承零商候选，则

\[
BE_{i+1}=E_i+\lambda_i r,
\qquad0<E_i<r.
\]

故

\[
\lambda_i=\left\lfloor\frac{BE_{i+1}}r\right\rfloor.
\]

确定性保证 \(\kappa_i=\lambda_i\)、\(R_i=E_i\)。继承余项始终严格
位于 \((0,r)\)，所以回放中出现 \(R_i=0\) 时不可能匹配。

反向地，若全部余项非零且 \(R_0=E_0\)，由 (3.2)、(3.5) 归纳得到

\[
B^{d-i}S=R_i+L_ir.
\]

取 \(i=0\) 得 (3.6)。(3.7) 正是 GFPm-3 已证明的双向恢复；并且

\[
q-s=(\rho-\eta)+L_0(B-\rho)>0,
\]

其中继承正规形给出 \(0<\eta<\rho<B\)。

故定理为充要判别，不是必要筛。\(\square\)

当 \(d=0\) 时循环为空，定理严格退化为

\[
R_0=S,
\qquad
S=E_0,
\qquad
L_0=0.
\tag{3.8}
\]

没有把空循环误当成至少一步下降。

---

## 4. 对偶坐标及其完整符号窗口

对每个 \(i<d\)，定义

\[
P_i=\frac{R_i+\kappa_i}{M},
\qquad
Q_i=\frac{R_i-\kappa_i}{C}.
\tag{4.1}
\]

由

\[
R_i=BR_{i+1}-\kappa_i(1+MD)
\]

得到

\[
R_i+\kappa_i
=M(CR_{i+1}-D\kappa_i),
\]

故

\[
\boxed{
P_i=CR_{i+1}-D\kappa_i\in\mathbb Z.
}
\tag{4.2}
\]

由

\[
R_i=BR_{i+1}-\kappa_i(-1+CU)
\]

得到

\[
R_i-\kappa_i
=C(MR_{i+1}-U\kappa_i),
\]

故

\[
\boxed{
Q_i=MR_{i+1}-U\kappa_i\in\mathbb Z.
}
\tag{4.3}
\]

使用 \(CU-MD=2\)：

\[
\begin{aligned}
UP_i-DQ_i
&=U(CR_{i+1}-D\kappa_i)
 -D(MR_{i+1}-U\kappa_i)\\
&=(CU-MD)R_{i+1}=2R_{i+1}.
\end{aligned}
\]

因此

\[
\boxed{UP_i-DQ_i=2R_{i+1}.}
\tag{4.4}
\]

直接相加、相减还得

\[
\boxed{2R_i=MP_i+CQ_i,}
\tag{4.5}
\]

\[
\boxed{2\kappa_i=MP_i-CQ_i.}
\tag{4.6}
\]

这些式子也反向恢复 \((R_i,\kappa_i)\)，故没有丢失信息。

符号不能粗暴写成 \(Q_i\ge0\)。由 \(R_i\ge1\)、
\(0\le\kappa_i\le B-1\)，有

\[
\frac{1-B}{C}<Q_i.
\]

又由 \(R_i\le r-1\)、\(\kappa_i\ge0\)，

\[
Q_i<\frac rC=U-\frac1C.
\]

所以严格整数窗口为

\[
\boxed{1-M\le Q_i\le U-1.}
\tag{4.7}
\]

另一方面，\(P_i>0\)，并且

\[
P_i=\frac{R_i+\kappa_i}{M}
\le\frac{(r-1)+(B-1)}M
=D+C-\frac1M.
\]

故

\[
\boxed{1\le P_i\le D+C-1.}
\tag{4.8}
\]

这给出每一步的真实符号字母：

\[
P_i>0,
\qquad
Q_i\in\{<0,=0,>0\},
\]

其中负号分支不能删除。

### 4.1 深度一、二、三的展开链

式 (4.4)–(4.6) 在每一层同时给出“上一余项”和“下一余项”。因此
深度一严格展开为

\[
\boxed{
2S=UP_0-DQ_0,
\qquad
2E_0=MP_0+CQ_0,
\qquad
2\kappa_0=MP_0-CQ_0.
}
\tag{4.9}
\]

深度二严格展开为

\[
\boxed{
\begin{aligned}
2S&=UP_1-DQ_1,\\
2R_1&=MP_1+CQ_1=UP_0-DQ_0,\\
2E_0&=MP_0+CQ_0,
\end{aligned}}
\tag{4.10}
\]

并且

\[
2\kappa_i=MP_i-CQ_i,
\qquad i=0,1.
\tag{4.11}
\]

深度三严格展开为

\[
\boxed{
\begin{aligned}
2S&=UP_2-DQ_2,\\
2R_2&=MP_2+CQ_2=UP_1-DQ_1,\\
2R_1&=MP_1+CQ_1=UP_0-DQ_0,\\
2E_0&=MP_0+CQ_0,
\end{aligned}}
\tag{4.12}
\]

以及

\[
2\kappa_i=MP_i-CQ_i,
\qquad i=0,1,2.
\tag{4.13}
\]

这正是长度分别为一、二、三的 Bezout 进位链。每个字母都必须同时满足
(4.7)–(4.8)，且由 (3.1) 的地板商唯一确定；所以展开没有引入自由
的 \((P_i,Q_i)\) 搜索。

---

## 5. 幂同余与不可约分审计

由 (1.11)，

\[
B^{-1}\equiv-E_0\pmod r.
\tag{5.1}
\]

实际下降满足

\[
E_d\equiv B^{-d}E_0\pmod r,
\]

所以

\[
\boxed{
E_d\equiv(-1)^dE_0^{d+1}\pmod r.
}
\tag{5.2}
\]

因 \(0<E_d<r\)，零商条件等价于

\[
\boxed{
2^A5^F
=\left\langle(-1)^dE_0^{d+1}\right\rangle_r^+.
}
\tag{5.3}
\]

由 (1.13)，

\[
\rho E_0\equiv J\pmod r.
\]

把 (5.2) 乘以 \((-1)^d\rho^{d+1}\)，得到

\[
\boxed{
(-1)^d\rho^{d+1}E_d
\equiv J^{d+1}\pmod r.
}
\tag{5.4}
\]

但不能从这里未经审计地除以 \(\rho\)。确实，

\[
\gcd(\rho,B)=1
\]

来自 \(\rho^2\equiv1\pmod B\)，而

\[
\begin{aligned}
\gcd(\rho,r)
&=\gcd(\rho,\rho+BJ)\\
&=\gcd(\rho,BJ)\\
&=\boxed{\gcd(\rho,J)}.
\end{aligned}
\tag{5.5}
\]

该公因数可以大于 \(1\)。本文从不以 \(\rho^{-1}\pmod r\) 为前提。
与此不同，\(E_0\) 的可逆性已经由 (1.12) 严格证明。

---

## 6. 深度零：下一高位逆元数字

深度零只有 \(\mathscr Z_{0,0}\)。此时

\[
E_0=S=2^A5^F,
\qquad
A=2a-t+h+v_0\ge2a.
\tag{6.1}
\]

所以 \(M\mid E_0\)。由 \(E_0=cU+J\)，

\[
\begin{aligned}
CE_0
&=c(CU)+CJ\\
&=c(MD+2)+CJ\\
&=McD+(2c+CJ).
\end{aligned}
\]

故

\[
\boxed{M\mid2c+CJ.}
\tag{6.2}
\]

定义

\[
\boxed{z=\frac{2c+CJ}{M}\in\mathbb Z_{>0}.}
\tag{6.3}
\]

上式给出完整下降：

\[
CE_0=M(cD+z).
\]

代入 \(C=5^{c_0}\)、\(M=2^{2a}\) 与 (6.1)，得到

\[
\boxed{
2^{A-2a}5^{F+c_0}=cD+z.
}
\tag{6.4}
\]

这正是题设 Z0.3。

先作题设要求的同层消去审计。由 \(Cx=2+Mc\) 及 \(a\ge3\)，有
\(v_2(x)=1\)，从而

\[
v_2(U)=v_2(JM+x)=1.
\tag{6.5a}
\]

由 (6.2) 的奇偶性，\(J\) 必为偶数。主室局部门给 \(D\) 为奇数；由
\(D=CJ+c\) 又知 \(c\) 为奇数，所以 \(v_2(cU)=1\)。若
\(v_2(J)\ne1\)，则 \(cU\) 与 \(J\) 不在同一二进层，因而

\[
v_2(cU+J)=\min\{v_2(cU),v_2(J)\}=1,
\]

与 \(A\ge2a\ge6\) 矛盾。故真正可能发生同层消去的只有

\[
\boxed{J\in\{2,6\}.}
\tag{6.5}
\]

对于 \(J=2,6\)，两项都恰有二进阶 \(1\)，所以本文不再使用两项赋值的
最小值，而保留完整消去。事实上 (6.4) 还精确给出

\[
\boxed{
v_2(cU+J)=A=2a+v_2(cD+z).
}
\tag{6.5b}
\]

现在定义

\[
y=U+x=JM+2x.
\tag{6.6}
\]

由 \(Cx=2+Mc\) 与 (6.3)，

\[
\begin{aligned}
Cy
&=CJM+2Cx\\
&=MCJ+4+2Mc\\
&=4+M(CJ+2c)\\
&=4+M^2z.
\end{aligned}
\]

所以深度零必要条件被精确提升为

\[
\boxed{Cy-M^2z=4.}
\tag{6.7}
\]

同时

\[
0<y=JM+2x<11M<M^2
\tag{6.8}
\]

因为 \(J\le9\)、\(x<M\)、\(M\ge64\)。故 (6.7) 中的 \(y\)
必须是唯一标准逆元

\[
\boxed{
y=\left\langle4C^{-1}\right\rangle_{M^2}^{+}.
}
\tag{6.9}
\]

又 \(v_2(x)=1\)，而 \(J\) 为偶数，所以 \(v_2(y)=2\)。将 (6.9)
除以 \(4\)：

\[
\boxed{
\frac y4
=\left\langle C^{-1}\right\rangle_{M^2/4}^{+}.
}
\tag{6.10}
\]

另一方面，(1.2) 除以 \(2\) 给

\[
\frac x2\equiv C^{-1}\pmod{M/2},
\qquad
0<\frac x2<\frac M2.
\tag{6.11}
\]

而 (6.6) 给

\[
\boxed{
\frac y4
=\frac x2+\frac J2\frac M2.
}
\tag{6.12}
\]

因此得到深度零的准确高位数字定理：

\[
\boxed{
\mathscr Z_{0,0}\text{ 的零商候选存在}
\Longrightarrow
C^{-1}\text{ 从模 }M/2\text{ 提升到模 }M^2/4
\text{ 时，下一基 }M/2\text{ 数字为 }J/2\in\{1,3\}.
}
\tag{6.13}
\]

式 (6.13) 严格强于原来的 \(M\mid2c+CJ\)，但它尚未产生绝对边界。
该数字取自 \(C=5^{2a-t}\) 的逆元在二进展开中从约第 \(2a\) 位到第
\(4a\) 位的移动区间；现有递推只给低阶逆元或逐 \(a\) 的完整大整数，
没有证明该高位数字永不落入 \(\{1,2,3,4\}\)。因此不能把
\(\mathscr Z_{0,0}\) 写成已关闭。

---

## 7. 深度一：平方 Bezout 对与二次型闭式

深度一包括

\[
\mathscr Z_{1,0},\qquad\mathscr Z_{0,1}.
\]

本节完全消去这两室中的移动模余数 \(E_1\bmod r\)。

### 7.1 一个统一大小事实

由 \(c_0=2a-t>3a/2\)，

\[
C^2=5^{2c_0}>5^{3a}.
\]

对 \(a\ge3\)，

\[
5^{3a}>100\cdot16^a=(10M)^2,
\]

因为在 \(a=3\) 时 \((125/16)^3>100\)，以后比值继续乘
\(125/16>1\)。所以

\[
\boxed{C>10M>U.}
\tag{7.1}
\]

特别地

\[
\boxed{U^2<r=CU-1.}
\tag{7.2}
\]

### 7.2 与 \(J\) 无关的唯一平方 Bezout 对

定义

\[
\boxed{
n_1=
\left\langle x^2\rho^{-1}\right\rangle_{M^2}^{+}
\in\{1,\ldots,M^2-1\}.
}
\tag{7.3}
\]

这里 \(\gcd(\rho,M)=1\)，故逆元合法。由

\[
(Cx)^2-4(Cx-1)=(Cx-2)^2=M^2c^2,
\]

有

\[
C^2x^2\equiv4\rho\pmod{M^2}.
\]

因此

\[
C^2n_1\equiv4\pmod{M^2}.
\]

定义

\[
\boxed{
m_1=\frac{C^2n_1-4}{M^2}\in\mathbb Z_{>0}.
}
\tag{7.4}
\]

于是

\[
\boxed{C^2n_1-M^2m_1=4.}
\tag{7.5}
\]

这是与 \(J\) 无关、且在规范窗 \(0<n_1<M^2\) 内唯一的正平方
Bezout 对。

再定义两个整数系数

\[
\boxed{
p_1=\frac{Cn_1-2x}{M},
}
\tag{7.6}
\]

\[
\boxed{
s_1=\frac{\rho n_1-x^2}{M^2}.
}
\tag{7.7}
\]

整数性分别来自

\[
n_1\equiv x^2\pmod M,
\qquad
C x\equiv2\pmod M,
\]

以及 (7.3)。又因 \(C>10M>x\)，有 \(\rho=Cx-1>x^2\)；结合
\(n_1\ge1\)，得到 \(\rho n_1>x^2\)，故 \(s_1>0\)。

直接展开还得到

\[
\begin{aligned}
p_1^2+4s_1
&=\frac{(Cn_1-2x)^2+4(\rho n_1-x^2)}{M^2}\\
&=\frac{n_1(C^2n_1-4)}{M^2}\\
&=n_1m_1.
\end{aligned}
\]

所以

\[
\boxed{p_1^2+4s_1=n_1m_1.}
\tag{7.8}
\]

### 7.3 \(E_1\) 的固定二次型

由 (5.2) 在 \(d=1\) 时的形式，

\[
r\mid U^2+M^2E_1.
\tag{7.9}
\]

令

\[
n=\frac{U^2+M^2E_1}{r}.
\]

由 (7.2) 与 \(0<E_1<r\)，

\[
0<n<M^2+1.
\]

又 \(n\not=M^2\)，因为模 \(M\) 有

\[
n\equiv U^2\equiv x^2\not\equiv0\pmod M.
\]

故

\[
0<n<M^2.
\tag{7.10}
\]

下面证明其标准剩余与 \(J\) 无关。由

\[
r=\rho+MCJ,
\qquad
U=x+MJ,
\]

有

\[
\begin{aligned}
\rho U^2-x^2r
&=MJ(2\rho x-Cx^2)+M^2\rho J^2\\
&=M^2\bigl(Jcx+\rho J^2\bigr),
\end{aligned}
\]

因为

\[
2\rho x-Cx^2=x(Cx-2)=Mcx.
\]

所以

\[
U^2r^{-1}\equiv x^2\rho^{-1}\pmod{M^2}.
\]

由 (7.3)、(7.10) 的唯一性，\(n=n_1\)。于是

\[
M^2E_1=rn_1-U^2.
\]

逐项展开：

\[
\begin{aligned}
rn_1-U^2
&=(\rho+MCJ)n_1-(x+MJ)^2\\
&=(\rho n_1-x^2)
 +MJ(Cn_1-2x)-M^2J^2\\
&=M^2(s_1+p_1J-J^2).
\end{aligned}
\]

故得到深度一闭式

\[
\boxed{
E_1=s_1+p_1J-J^2.
}
\tag{7.11}
\]

联合 (7.8)，也可写成

\[
\boxed{
4E_1=n_1m_1-(p_1-2J)^2.
}
\tag{7.12}
\]

式 (7.11)–(7.12) 完全不含移动模数 \(r\) 或反向商 \(\kappa_0\)。

### 7.4 两个深度一室的准确残余方程

在 \(\mathscr Z_{1,0}\) 中，

\[
v_0+2t<2a,
\]

且零商等价于

\[
\boxed{
s_1+p_1J-J^2
=2^{2a-t+h+v_0}5^{v_0+t}.
}
\tag{7.13}
\]

在 \(\mathscr Z_{0,1}\) 中，令

\[
f=v_0+t-2a.
\]

室条件给

\[
0\le f<t,
\qquad
v_0=2a-t+f.
\]

因此零商等价于

\[
\boxed{
s_1+p_1J-J^2
=2^{h+2a-2t+f}5^f,
\qquad0\le f<t.
}
\tag{7.14}
\]

每个 \((a,t,J)\) 只产生同一个二次型值；\(h,v_0\) 只负责检查它是否
落入 (7.13) 或 (7.14) 的 \((2,5)\)-单位指数窗。这个正规形严格强于
“对每个 \(a\) 递推计算 \(E_1\)”；但系数
\((n_1,m_1,p_1,s_1)\) 仍是从模 \(M\) 到模 \(M^2\) 的移动高位
Bezout 数据。现有材料没有证明二次型 (7.11) 不能是所列 \((2,5)\)-单位，
也没有给它们绝对有限的 \(a\) 上界。因此两个深度一室尚未关闭。

---

## 8. 深度二、三的双商高位进位

本节给出一个统一的短商公式。它适用于 \(d=2,3\)，也可复核
\(d=0,1\)。

由 (5.2) 及

\[
CE_0\equiv D\pmod r,
\tag{8.1}
\]

可得

\[
\boxed{
r\mid U^{d+1}+M^{d+1}E_d,
}
\tag{8.2}
\]

以及

\[
\boxed{
r\mid C^{d+1}E_d-(-1)^dD^{d+1}.
}
\tag{8.3}
\]

定义

\[
\boxed{
K_d=\frac{U^{d+1}+M^{d+1}E_d}{r}>0,
}
\tag{8.4}
\]

\[
\boxed{
H_d=\frac{C^{d+1}E_d-(-1)^dD^{d+1}}r
\in\mathbb Z.
}
\tag{8.5}
\]

因为 \(v_2(U)=1\)，而第二项
\(M^{d+1}E_d\) 的二进阶严格大于 \(d+1\)，所以

\[
\boxed{v_2(K_d)=d+1.}
\tag{8.6}
\]

又因 \(D\) 是五进单位、\(r\equiv-1\pmod5\)，而
\(C^{d+1}E_d\) 被 \(5\) 整除，故

\[
\boxed{v_5(H_d)=0.}
\tag{8.7}
\]

令

\[
n_d=\left\langle U^{d+1}r^{-1}\right\rangle_{M^{d+1}}^+
\in\{1,\ldots,M^{d+1}-1\}.
\tag{8.8}
\]

由 \(E_d<r\)，

\[
K_d<M^{d+1}+\frac{U^{d+1}}r.
\]

而 \(U<10M\)、\(r=CU-1>(C-1)U\)、\(C>10M\)、\(d\le3\)
给

\[
\frac{U^{d+1}}r<\frac{U^d}{C-1}<M^{d+1}.
\]

所以

\[
0<K_d<2M^{d+1}.
\]

结合 (8.8) 的标准剩余，唯一存在

\[
\boxed{\theta_d\in\{0,1\}}
\tag{8.9}
\]

使

\[
\boxed{
K_d=n_d+\theta_dM^{d+1}.
}
\tag{8.10}
\]

因此

\[
\boxed{
E_d=
\frac{r(n_d+\theta_dM^{d+1})-U^{d+1}}{M^{d+1}}.
}
\tag{8.11}
\]

这是深度二、三的二值高位进位公式。它把任意大小的商压成一个标准
\(M^{d+1}\)-逆元与一个比特 \(\theta_d\)，没有预设二进赋值上界。

两个商还满足短 Bezout 恒等式。由 \(CU=r+1\)、\(MD=r-1\)，

\[
\begin{aligned}
C^{d+1}K_d-M^{d+1}H_d
&=\frac{(r+1)^{d+1}+(-1)^d(r-1)^{d+1}}r.
\end{aligned}
\tag{8.12}
\]

逐深度为

\[
\boxed{
\begin{array}{c|c}
d&C^{d+1}K_d-M^{d+1}H_d\\ \hline
0&2\\
1&4\\
2&2r^2+6\\
3&8r^2+8
\end{array}}
\tag{8.13}
\]

深度二对应

\[
\mathscr Z_{2,0},\qquad\mathscr Z_{1,1},
\]

深度三对应

\[
\mathscr Z_{2,1}.
\]

三个室的终端方程分别是

\[
\boxed{
\begin{aligned}
\mathscr Z_{2,0}:\quad
&v_0+3t<2a,\\
&\frac{r(n_2+\theta_2M^3)-U^3}{M^3}
 =2^{2a-t+h+v_0}5^{v_0+2t};\\
\mathscr Z_{1,1}:\quad
&v_0+2t\ge2a,\\
&\frac{r(n_2+\theta_2M^3)-U^3}{M^3}
 =2^{h+v_0-t}5^{v_0+2t-2a};\\
\mathscr Z_{2,1}:\quad
&v_0+3t\ge2a,\\
&\frac{r(n_3+\theta_3M^4)-U^4}{M^4}
 =2^{h+v_0-t}5^{v_0+3t-2a}.
\end{aligned}}
\tag{8.14}
\]

其中两个 \(j=2\) 室还必须满足 (2.11)，所有指数满足 (2.12)，并且
\(\theta_2,\theta_3\in\{0,1\}\)。这样六室中深度零由第 6 节、
两个深度一室由 (7.13)–(7.14)、两个深度二室和一个深度三室由
(8.14) 分别明确列出，没有合并丢失室条件。

零商要求 (8.11) 的右端恰为表 (2.3) 指定的 \(2^A5^F\)，并同时
满足 (8.6)–(8.7)。这已经是固定长度的双商链；但
\(n_d\) 仍是模 \(M^{d+1}=2^{2a(d+1)}\) 的移动高位逆元。
题设允许的状态不能保存完整 \(n_d\)，而固定低阶剩余并不能恢复它。
故 (8.11) 还不是题设意义下的固定有限自动机。

---

## 9. 为什么不能从当前结果构造所要求的有限自动机

题设要求自动机状态只依赖

\[
i,j,\epsilon,J,
\qquad
P_i\bmod2^s,
\qquad
Q_i\bmod5^s,
\]

和有限个符号、同层消去标签，而不能依赖完整 \(a,r\) 或大整数。

第 6 节给出一个直接审计。深度零零商要求

\[
\left\langle C^{-1}\right\rangle_{M^2/4}^{+}
=\frac x2+\frac J2\frac M2.
\tag{9.1}
\]

右端的 \(J/2\) 不是 \(C^{-1}\) 的固定低位剩余，而是从精度
\(2a-1\) 提升到精度 \(4a-2\) 时出现的下一整块数字。随着 \(a\) 增大，
被询问的位区间也向高位移动。对任意固定 \(s\)，数据

\[
C^{-1}\bmod2^s,
\qquad
P_i\bmod2^s,
\qquad
Q_i\bmod5^s
\]

都不包含这一整块高位数字。

深度一的 \(n_1\) 是同一现象的平方版本：

\[
C^2n_1-M^2m_1=4,
\qquad0<n_1<M^2.
\tag{9.2}
\]

式 (7.11) 所需的 \(p_1,s_1\) 正是 (9.2) 的高位商。深度二、三的
\(n_d\) 又把所需精度推进到 \(M^{d+1}\)。

因此，当前链条只证明了“每条候选有固定长度、有限个高位进位比特”，没有证明
“所有高位 Bezout 数字属于固定有限状态”。若把完整 \(n_d\) 或
\(C^{-1}\bmod M^{d+1}\) 塞入状态，就违反题设的状态限制；若只保留固定低位，
则转移不再双向，可能把不同高位数字合并成伪存活循环。

所以本文不把 (8.9) 的一个比特夸大成 GFPmZ-3。要真正得到 GFPmZ-3，
还必须新增至少一种未在继承材料中出现的输入：

1. 覆盖移动高位逆元数字的有限递推；或
2. 对 (6.13)、(7.13)–(7.14)、(8.11) 的统一二进/五进赋值上界；或
3. 先由符号不等式把 \(a\) 压到绝对有限范围。

三者目前均未得到。

---

## 10. 主动反例攻击

### 10.1 \(\gcd(\rho,r)>1\)

已由 (5.5) 精确保留：

\[
\gcd(\rho,r)=\gcd(\rho,J)
\]

可以大于 \(1\)。全文没有除以 \(\rho\)。

这不是纯形式警告：完整局部门中的

\[
(a,t,h,J)=(16,0,12,9)
\]

给出 \(\gcd(\rho,r)=\gcd(\rho,J)=3\)。因此任何以
\(\rho^{-1}\pmod r\) 为起点的删除都会漏掉实际可达参数状态。

### 10.2 \(Q_i<0\)

式 (4.7) 给出

\[
1-M\le Q_i\le U-1.
\]

负号是合法状态字母，没有被删除。

完整局部门中的 \((a,t,h,J,j,v_0)=(13,0,10,1,2,0)\) 给出深度二
继承链第一步 \(Q_1=-43920834\)。这个精确反例说明 \(Q_i<0\) 不只是
区间估计留下的形式可能。

### 10.3 \(R_i=0\)

定理 3.1 说明，零余项与继承的严格正余项窗口不相容，必须立即拒绝。

### 10.4 \(F=0\)

表 (2.3)、(7.14)、(8.11) 全部允许 \(F=0\)。没有用五进正性删除该边界。

### 10.5 \(d=0\)

第 3 节把空循环单独化为 \(S=E_0,L_0=0\)，没有套用任何不存在的
\(\kappa_i\)。

### 10.6 \(\epsilon=1\) 时 \(A<2a\)

式 (2.9) 只给随 \(j\) 变化的严格正下界，没有把三个溢出室错误送回
\(A\ge2a\)。

### 10.7 偶数 \(J\) 的同层消去

深度零没有用两项赋值最小值；相反，(6.5) 证明只有 \(J=2,6\) 才可能
发生所需消去，并把其完整提升到高位逆元数字 (6.13)。

### 10.8 六室完备性

表 (2.3) 由 \(j\in\{0,1,2\}\) 与 \(\epsilon\in\{0,1\}\) 的
欧几里得分层给出。删除任一行都会遗漏相应
\(v_0+(j+1)t<2a\) 或 \(\ge2a\) 的指数状态。本文没有删除任何尚未
证明为空的室。

### 10.9 有限前缀外推

本文没有用有限 \(a\) 前缀支持无界结论，也没有生成有限证书包。
没有先得到绝对有限边界时，任何有限枚举都只能是诊断，不能升级为证明。

---

## 11. 证明等级、证书与停止点

本轮没有得到绝对有限参数边界，也没有得到满足题设状态限制的固定有限自动机。
因此不生成所谓“规范有限证书包”：没有符号有限化就制作有限前缀证书，会把
实现核对伪装成无界证明。

严格新增的可冻结结论是：

\[
\boxed{
\begin{gathered}
E_0=\eta+\rho J=cU+J=xD-J;\\
\mathscr Z\text{ 与至多三步确定性反向回放双向等价};\\
1\le P_i\le D+C-1,
\quad1-M\le Q_i\le U-1;\\
\mathscr Z_{0,0}\text{ 强迫 }J\in\{2,6\}
\text{ 及高位逆元数字 }J/2\in\{1,3\};\\
E_1=s_1+p_1J-J^2,
\quad p_1^2+4s_1=n_1m_1,
\quad C^2n_1-M^2m_1=4;\\
E_d=
\dfrac{r(n_d+\theta_dM^{d+1})-U^{d+1}}{M^{d+1}},
\quad\theta_d\in\{0,1\},
\quad d=2,3.
\end{gathered}
}
\tag{11.1}
\]

但是六个零商室仍未被统一删除；\(a\) 未绝对有界；移动高位 Bezout 数字尚未
被固定有限状态化。因此：

- 不是 GFPmZ-1：没有证明 \(\mathscr Z\) 为空；
- 不是 GFPmZ-2：没有绝对有限边界；
- 不是 GFPmZ-3：固定低阶状态不足以双向重建移动高位逆元数字；
- 不是 GFPmZ-4：没有找到合法原题解；
- 不是 GFPmZ-5：B1–B5、R1–R3、C1–C7、P1–P3 与继承系统相容。

按上述保守交付门槛只能取

\[
\boxed{
\mathrm{GFPmZ\text{-}6}:
\quad
\mathscr Z\text{ 获得高位 Bezout 正规形，但没有达到全局关闭、}
\text{绝对有限化或固定有限自动机。}
}
\tag{11.2}
\]

本文到此停止，不研究
\(\mathscr P_0,\mathscr P_1\)、\(\mathcal F_{E-}\)、\(\varphi<a\)、
B、C、\(\gamma>1\)、C2/C5、Q 或严格层。
