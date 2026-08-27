# 三项十进制拼接平方和问题：临界 G 模板 A2 高 \(\varphi\) 主二进室负符号族正商 \(j=1\) 报告

日期：2026-08-02（Asia/Tokyo）

本文严格限定于

\[
\boxed{
\mathscr P_1:
\quad j=1,\quad \epsilon=0,\quad d=1,\quad \ell>0.
}
\]

接受 GFPmP0-3、GFPmZ-6、GFPmR-3、GFPm-3、GA2H-2、GA2-6、
PR6、SD6 与 v3 总账中和本分支相容的冻结结论。本文不研究
\(\mathscr P_0\)、六条零商族、\(\mathcal F_{E-}\)、\(\varphi<a\)、
B、C、\(\gamma>1\)、C2/C5、Q 或严格层。

本轮得到的严格推进是：

1. 独立重建并反向回放了深度一平方 Bezout 正规形；
2. 每个固定 \((a,t,h,J,F)\) 至多产生一个正商候选，且唯一候选不再通过
   任何随 \(a\) 增长的 \(\ell\) 区间枚举；
3. 正商严格强迫
   \[
   \boxed{F\ge a+1,\qquad 5^F>10M;}
   \]
4. 五进低块和二进高位数字分别有显式二次型闭式：
   \[
   e_5=
   \left\langle-(n_1+U^2)M^{-2}\right\rangle_{5^F},
   \]
   \[
   \delta_1=
   \left\langle\frac{n_1}{4}(D^2-m_1)\right\rangle_M;
   \]
5. 二进接受门精确等价于
   \[
   \boxed{e_5\ne0,\qquad e_5\equiv\delta_1\pmod M,}
   \]
   其中 \(\delta_1\) 是
   \[
   \left\langle U^2r^{-1}\right\rangle_{M^3}^{+}
   \]
   从模 \(M^2\) 提升到模 \(M^3\) 时出现的下一基 \(M\) 数字；
6. 给出了唯一候选的完整等式、严格双向恢复，以及一个保持平方 Bezout
   行列式的第二坐标系。

但是，现有结构没有证明上述移动高位数字永远不能与五进低块对齐，也没有把
该对齐条件压到绝对有限的 \(a\) 或固定外部素数周期证书。有限前缀中没有命中，
但该事实不承担无界证明。因此不能诚实分类为 GFPmP1-1 或 GFPmP1-2。
没有找到合法原题解，也没有发现 GFPmR-3、GFPmP0-3 或深度一正规形错误。
最终分类为

\[
\boxed{\mathrm{GFPmP1\text{-}3}.}
\]

---

## 1. 继承参数与 \(\mathscr P_1\) 指数室

保留

\[
a\ge3,\qquad 0\le t<\frac a2,
\qquad h\in\mathcal H(a),\qquad J\in\{1,\ldots,9\},
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
\rho=Cx-1=1+Mc,
\qquad \eta=cx,
\tag{1.7}
\]

\[
U=x+MJ,
\qquad D=c+CJ.
\tag{1.8}
\]

直接计算给出

\[
\boxed{CU-MD=2,}
\tag{1.9}
\]

\[
\boxed{r=-1+CU=1+MD=\rho+BCJ,}
\tag{1.10}
\]

\[
\boxed{E_0=\eta+\rho J=cU+J=xD-J.}
\tag{1.11}
\]

同时始终保留全部局部门

\[
v_5\!\left(U+\frac M2\right)=3t,
\tag{1.12}
\]

\[
W=\frac{U+M/2}{5^{3t}},
\qquad -2W\equiv1\ \text{或}\ 4\pmod5,
\tag{1.13}
\]

\[
v_2(k^2-1)=2a,
\qquad
\frac{k^2-1}{2^{2a}}\equiv3\ \text{或}\ 7\pmod8,
\tag{1.14}
\]

其中

\[
k=-1+C\left(U+\frac M2\right)=r+\frac B2.
\tag{1.15}
\]

在 \(\mathscr P_1\) 中

\[
\nu=2a+v_0,
\qquad0\le v_0<2a,
\qquad v_0+2t<2a,
\tag{1.16}
\]

\[
A=2a-t+h+v_0,
\qquad F=v_0+t,
\tag{1.17}
\]

\[
q_*=c_0-F=2a-v_0-2t\ge1,
\tag{1.18}
\]

\[
p=2^{A-2a}=2^{h+v_0-t}=2^{h+F-2t}.
\tag{1.19}
\]

正商区间为

\[
1\le\ell\le
L=\min\left(
5^F-1,
\left\lfloor\frac{p-1}{J5^{q_*}}\right\rfloor
\right),
\tag{1.20}
\]

并定义

\[
w=p-J\ell5^{q_*}>0,
\tag{1.21}
\]

\[
E^*=M5^Fw-\ell\rho.
\tag{1.22}
\]

因为下降深度恰为 \(d=1\)，完整终端条件是

\[
\boxed{E^*=E_1,}
\tag{1.23}
\]

而不是 \(E^*=E_0\)。

---

## 2. 两个统一大小事实

### 2.1 \(C>10M>U\)

由 \(t<a/2\)，

\[
c_0=2a-t>\frac{3a}{2}.
\]

所以

\[
C^2=5^{2c_0}>5^{3a}.
\]

对 \(a=3\)，有

\[
5^9=1{,}953{,}125>409{,}600=100\cdot16^3;
\]

以后左右比值每步再乘 \(125/16>1\)。故

\[
5^{3a}>100\cdot16^a=(10M)^2,
\]

从而

\[
\boxed{C>10M.}
\tag{2.1}
\]

又因 \(J\le9\) 且 \(0<x<M\)，

\[
\boxed{0<U<10M<C.}
\tag{2.2}
\]

特别地

\[
\boxed{U^2<CU-1=r.}
\tag{2.3}
\]

### 2.2 \(\gcd(\rho,M)=1\)

由

\[
\rho=1+Mc
\]

直接有

\[
\boxed{\gcd(\rho,M)=1.}
\tag{2.4}
\]

所以后文模 \(M^2\) 使用 \(\rho^{-1}\) 完全合法。这里没有、也不需要
假设 \(\rho\) 在模 \(r\) 下可逆。

---

## 3. 深度一平方 Bezout 对的独立重建

定义

\[
\boxed{
n_1=
\left\langle x^2\rho^{-1}\right\rangle_{M^2}^{+}
\in\{1,\ldots,M^2-1\}.
}
\tag{3.1}
\]

因为 \(v_2(x)=1\)、\(\rho\) 为奇数，所以

\[
\boxed{v_2(n_1)=2.}
\tag{3.2}
\]

特别地 \(n_1\ne0\)，正代表定义没有端点歧义。

### 3.1 第一平方 Bezout 恒等式

恒等式

\[
(Cx)^2-4(Cx-1)=(Cx-2)^2=M^2c^2
\]

给出

\[
C^2x^2\equiv4\rho\pmod{M^2}.
\]

由 \(\rho n_1\equiv x^2\pmod{M^2}\) 并约去模 \(M^2\) 的单位
\(\rho\)，得到

\[
C^2n_1\equiv4\pmod{M^2}.
\]

因此可定义

\[
\boxed{m_1=\frac{C^2n_1-4}{M^2}\in\mathbb Z_{>0},}
\tag{3.3}
\]

并严格得到

\[
\boxed{C^2n_1-M^2m_1=4.}
\tag{3.4}
\]

再定义

\[
\boxed{p_1=\frac{Cn_1-2x}{M},}
\tag{3.5}
\]

\[
\boxed{s_1=\frac{\rho n_1-x^2}{M^2}.}
\tag{3.6}
\]

整数性分别来自

\[
n_1\equiv x^2\pmod M,
\qquad Cx\equiv2\pmod M,
\]

以及 (3.1)。由 \(C>x\)、\(n_1\ge1\) 和

\[
\rho=Cx-1>x^2
\]

还得 \(s_1>0\)。

直接展开：

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
\tag{3.7}
\]

### 3.2 \(E_1\) 的二次型闭式

先证明 \(n_1\) 同时是 \(U^2r^{-1}\) 模 \(M^2\) 的标准正代表。
由

\[
r=\rho+MCJ,
\qquad U=x+MJ,
\]

有

\[
\begin{aligned}
\rho U^2-x^2r
&=MJ(2\rho x-Cx^2)+M^2\rho J^2\\
&=M^2(Jcx+\rho J^2),
\end{aligned}
\tag{3.8}
\]

其中使用

\[
2\rho x-Cx^2=x(Cx-2)=Mcx.
\]

故

\[
U^2r^{-1}\equiv x^2\rho^{-1}\pmod{M^2}.
\tag{3.9}
\]

定义

\[
M^2E_1=rn_1-U^2.
\tag{3.10}
\]

式 (3.9) 保证右端被 \(M^2\) 整除。又由 (2.3)、
\(1\le n_1<M^2\)，

\[
0<rn_1-U^2<rM^2,
\]

所以

\[
\boxed{0<E_1<r.}
\tag{3.11}
\]

展开 (3.10)：

\[
\begin{aligned}
rn_1-U^2
&=(\rho+MCJ)n_1-(x+MJ)^2\\
&=M^2(s_1+p_1J-J^2).
\end{aligned}
\]

因此

\[
\boxed{E_1=s_1+p_1J-J^2.}
\tag{3.12}
\]

联合 (3.7)，得到

\[
\boxed{4E_1=n_1m_1-(p_1-2J)^2.}
\tag{3.13}
\]

这逐项证明了题设 (D1.5)–(D1.8)。

### 3.3 一次反向余数回放

由

\[
\rho r=1+BE_0
\tag{3.14}
\]

得

\[
BE_0\equiv-1\pmod r,
\qquad B^{-1}\equiv-E_0\pmod r.
\tag{3.15}
\]

另一方面，继承恒等式

\[
UD=E_0+Jr,
\qquad MD=r-1
\]

给

\[
ME_0\equiv-U\pmod r.
\tag{3.16}
\]

由 (3.10) 模 \(r\) 及 \(\gcd(M,r)=1\)，

\[
E_1\equiv-U^2M^{-2}\equiv-E_0^2
\equiv B^{-1}E_0\pmod r.
\]

结合 (3.11) 的严格正余数窗口，唯一性给出

\[
\boxed{
E_1=
\left\langle B^{-1}E_0\right\rangle_r^{+},
\qquad0<E_1<r.
}
\tag{3.17}
\]

因此平方 Bezout 公式与一次真实 \(B\)-下降完全一致，不是未经复核的继承
黑箱。

---

## 4. 正商的唯一 CRT 候选

由 \(E^*=E_1\)，

\[
M5^Fw=E_1+\ell\rho.
\tag{4.1}
\]

所以

\[
\ell\rho\equiv-E_1\pmod{M5^F}.
\tag{4.2}
\]

由

\[
\rho^2=1+B\eta,
\qquad M5^F\mid B,
\]

有

\[
\boxed{\gcd(\rho,M5^F)=1,}
\qquad
\boxed{\rho^{-1}\equiv\rho\pmod{M5^F}.}
\tag{4.3}
\]

故

\[
\boxed{\ell\equiv-E_1\rho\pmod{M5^F}.}
\tag{4.4}
\]

定义完整 CRT 的最小非负代表

\[
\boxed{
\ell_{\mathrm{CRT}}
=\left\langle-E_1\rho\right\rangle_{M5^F}
\in\{0,\ldots,M5^F-1\}.
}
\tag{4.5}
\]

合法五进窗口

\[
1\le\ell\le5^F-1
\]

的长度严格小于模数 \(M5^F\)。因此

\[
\boxed{
\text{每个固定 }(a,t,h,J,F)
\text{ 至多产生一个正商候选}.}
\tag{4.6}
\]

候选存在必须满足

\[
\boxed{1\le\ell_{\mathrm{CRT}}\le5^F-1.}
\tag{4.7}
\]

当 \(F=0\) 时 \(5^F-1=0\)，故

\[
\boxed{F=0\Longrightarrow\mathscr P_1\text{ 自动为空}.}
\tag{4.8}
\]

---

## 5. 纯二进—纯五进拆分

因为

\[
\rho\equiv1\pmod M,
\qquad
\rho\equiv-1\pmod{5^F},
\]

式 (4.4) 严格拆成

\[
\boxed{\ell\equiv-E_1\pmod M,}
\tag{5.1}
\]

\[
\boxed{\ell\equiv E_1\pmod{5^F}.}
\tag{5.2}
\]

定义

\[
e_2=\langle-E_1\rangle_M,
\qquad
e_5=\langle E_1\rangle_{5^F}.
\tag{5.3}
\]

因为合法 \(\ell\) 已经位于 \(1\le\ell<5^F\)，五进同余 (5.2)
唯一强迫

\[
\ell=e_5.
\]

于是 (4.7) 与下列条件严格等价：

\[
\boxed{
1\le e_5\le5^F-1,
\qquad e_5\equiv-E_1\pmod M.
}
\tag{5.4}
\]

在这种情况下

\[
\boxed{\ell_{\mathrm{CRT}}=\ell_*=e_5.}
\tag{5.5}
\]

所以五进低块直接给出唯一 \(\ell\)，二进条件只负责接受或拒绝；不再需要
计算模 \(M5^F\) 的完整 CRT 代表，更不存在自由 \(\ell\) 搜索。

### 5.1 双商与赋值

在 (5.4) 成立时定义

\[
\boxed{u=\frac{E_1-\ell_*}{5^F}\in\mathbb Z_{\ge0},}
\tag{5.6}
\]

\[
\boxed{v=\frac{E_1+\ell_*}{M}\in\mathbb Z_{\ge0}.}
\tag{5.7}
\]

这里必须允许 \(u=0\)。两式相减给出

\[
\boxed{Mv-5^Fu=2\ell_*.}
\tag{5.8}
\]

令 \(f=v_5(\ell_*)<F\)。由

\[
Mv=5^Fu+2\ell_*
\]

右端第二项具有唯一较低的五进赋值，故

\[
\boxed{v_5(v)=v_5(\ell_*).}
\tag{5.9}
\]

这是无条件结论。

令 \(e=v_2(\ell_*)\)，并约定 \(v_2(0)=+\infty\)。从 (5.8) 模
\(M\) 得到精确的二进分流：

\[
\boxed{
\begin{array}{ll}
e\le2a-2:&v_2(u)=e+1,\\
e\ge2a-1:&M\mid u.
\end{array}}
\tag{5.10}
\]

仅凭 CRT 不能进一步固定 \(v_2(v)\)，因为 (5.8) 的两项会在达到模
\(M\) 后发生高位消去。

若完整终端等式成立，则还恢复双走廊中的两个等式

\[
2^A=u+\ell_*5^{q_*}U,
\tag{5.11}
\]

\[
2^{A-2a}5^F=v+\ell_*D.
\tag{5.12}
\]

因此完整候选还满足

\[
\boxed{
v_2(u)=v_2(\ell_*)+1
\quad\text{若 }v_2(\ell_*)+1<A,
}
\tag{5.13}
\]

\[
\boxed{
v_2(v)=v_2(\ell_*)
\quad\text{若 }v_2(\ell_*)<A-2a.
}
\tag{5.14}
\]

式 (5.9)、(5.13)–(5.14) 正好复核 GFPmR-3 的局部赋值字典；本文没有
在同层消去时非法套用两项赋值的最小值。

---

## 6. 正商强迫 \(F\ge a+1\)

### 6.1 两个整数斜率界

尾窗给出

\[
\boxed{h<\frac{7a}{8}.}
\tag{6.1}
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

提升界 (1.4) 还给

\[
\boxed{t\le\frac a3.}
\tag{6.2}
\]

对 \(a\ge11\)，若 \(3t>a\)，将 (1.4) 立方得到

\[
125^{3t}<1331\cdot64^a.
\]

但在 \(a=11\) 已有精确反向比较

\[
125^{11}
=116415321826934814453125
>
98210465448429652803584
=1331\cdot64^{11};
\]

以后左、右比值每步再乘 \(125/64>1\)。对 \(3\le a\le10\)，
(1.4) 允许的最大 \(t\) 依次为

\[
1,1,1,2,2,2,3,3,
\]

同样满足 \(3t\le a\)。故 (6.2) 对全部 \(a\ge3\) 成立。

### 6.2 大 \(F\) 定理

若 \(\ell>0\)，由 \(w>0\) 及整数性，

\[
p>J\ell5^{q_*}\ge5^{q_*}.
\tag{6.3}
\]

反设 \(F\le a\)。由 (6.1)、(6.2)，

\[
\begin{aligned}
\frac{p}{5^{q_*}}
&=\frac{2^{h+F-2t}}{5^{2a-F-t}}\\
&<\frac{2^{15a/8-2t}}{5^{a-t}}\\
&\le\frac{2^{29a/24}}{5^{2a/3}}<1.
\end{aligned}
\tag{6.4}
\]

最后一步只使用整数幂比较

\[
2^{29}=536870912
<152587890625=5^{16}.
\]

这与 (6.3) 矛盾。因此

\[
\boxed{F\ge a+1.}
\tag{6.5}
\]

---

## 7. 全部状态满足 \(5^F>10M\)

当 \(a\ge4\) 时，由 (6.5)，

\[
5^F\ge5^{a+1}>10\cdot4^a=10M.
\tag{7.1}
\]

端点 \(a=4\) 是

\[
5^5=3125>2560=10\cdot4^4,
\]

以后左右比值每步再乘 \(5/4>1\)。

只剩 \(a=3\)。此时

\[
\mathcal H(3)=\{1,2\},
\qquad t\in\{0,1\}.
\]

直接按 (1.12)–(1.14) 作完整局部门：

- \(t=0\) 时只留下 \(J=4\)；
- \(t=1\) 时没有局部状态。

由 (6.5) 和 \(F<c_0=6\)，只需检查 \(F=4,5\)。当 \(F=4\) 时

\[
q_*=2,
\qquad p=2^{h+4}\le64<4\cdot5^2=100,
\]

故正商区间为空。于是正商只能有 \(F=5\)，且

\[
5^F=3125>640=10M.
\]

综上，全部 \(\mathscr P_1\) 状态都满足

\[
\boxed{F\ge a+1,\qquad5^F>10M.}
\tag{7.2}
\]

这里的小端核对使用了完整局部门，不是仅检查指数室。

---

## 8. 五进低块的固定二次型闭式

由 (3.10) 以及

\[
r\equiv-1\pmod{5^F},
\qquad F<c_0,
\]

有

\[
M^2E_1\equiv-(n_1+U^2)\pmod{5^F}.
\]

因为 \(M\) 是模 \(5^F\) 的单位，得到

\[
\boxed{
e_5=
\left\langle-(n_1+U^2)M^{-2}\right\rangle_{5^F}.
}
\tag{8.1}
\]

代入 \(U=x+MJ\)，这就是关于固定数字 \(n_1,x,M\) 和
\(J\in\{1,\ldots,9\}\) 的显式二次型低块。它不需要先构造完整大整数
\(E_1\)。

若 \(e_5=0\)，则正商候选立即删除；本文没有把该边界误当成合法
\(\ell=5^F\)。

---

## 9. 从模 \(M^2\) 到模 \(M^3\) 的高位 Bezout 数字

定义更高精度的标准正代表

\[
\boxed{
n_2=
\left\langle U^2r^{-1}\right\rangle_{M^3}^{+}
\in\{1,\ldots,M^3-1\}.
}
\tag{9.1}
\]

由 (3.9)，其模 \(M^2\) 的标准余数就是 \(n_1\)。所以唯一存在

\[
\boxed{\delta_1\in\{0,\ldots,M-1\}}
\tag{9.2}
\]

使

\[
\boxed{n_2=n_1+M^2\delta_1.}
\tag{9.3}
\]

这就是从精度 \(M^2\) 提升到 \(M^3\) 时出现的下一基 \(M\) 数字。

由

\[
rn_1-U^2=M^2E_1,
\]

以及 \(rn_2-U^2\equiv0\pmod{M^3}\)，有

\[
E_1+r\delta_1\equiv0\pmod M.
\]

而 \(r\equiv1\pmod M\)，故

\[
\boxed{\delta_1=\langle-E_1\rangle_M=e_2.}
\tag{9.4}
\]

因此题设的二进接受门不是一个新的自由同余：它恰好询问这个移动高位
Bezout 数字。

### 9.1 \(\delta_1\) 的固定二次型闭式

由 (3.4) 和 (3.2)，写

\[
\iota_1=\frac{n_1}{4}.
\tag{9.5}
\]

则

\[
\boxed{
\iota_1=
\left\langle C^{-2}\right\rangle_{M^2/4}^{+}
=
\left\langle5^{-2c_0}\right\rangle_{M^2/4}^{+},
}
\tag{9.6}
\]

并且

\[
C^2\iota_1-\frac{M^2}{4}m_1=1.
\tag{9.7}
\]

从 (3.4)–(3.7) 还可直接推出对偶恒等式

\[
\boxed{C^2E_1=rm_1-D^2.}
\tag{9.8}
\]

一种验证是令 \(y_1=p_1-2J\)，使用

\[
Cn_1-My_1=2U,
\qquad Mm_1-Cy_1=2D,
\]

再展开 (3.13)。

把 (9.8) 模 \(M\) 化简，并用

\[
r\equiv1\pmod M,
\qquad \iota_1\equiv C^{-2}\pmod M,
\]

得到

\[
\boxed{
\delta_1
=\left\langle
\iota_1(D^2-m_1)
\right\rangle_M.
}
\tag{9.9}
\]

这是题设所要求的“由 \((n_1,m_1,p_1,s_1)\) 固定二次型恢复高位数字”
的精确实现。因为 \(D=c+CJ\)，(9.9) 对 \(J\) 是固定二次型；指数
\(2c_0\) 由平方 Bezout 式 (3.4) 严格推出，没有猜测新的逆元指数。

### 9.2 唯一候选的高位数字判别

联合 (8.1)、(9.4) 和第 5 节，候选存在的 CRT 部分严格等价于

\[
\boxed{
\begin{gathered}
e_5=
\left\langle-(n_1+U^2)M^{-2}\right\rangle_{5^F},\\
1\le e_5\le5^F-1,\\
e_5\equiv
\left\langle\iota_1(D^2-m_1)\right\rangle_M
\pmod M.
\end{gathered}}
\tag{9.10}
\]

若 (9.10) 成立，唯一置

\[
\boxed{\ell_*=e_5.}
\tag{9.11}
\]

式 (9.10) 是本轮的准确高位 Bezout 残余。虽然 \(5^F>10M\)，合法
五进窗包含许多基 \(M\) 块；所以 (9.2) 的单个数字并不会仅由大小自动
排除。另一方面，\(e_5\) 已由 (8.1) 唯一确定，故这里也没有重新引入
任何 \(\ell\) 枚举。

---

## 10. 唯一候选的完整等式与双向恢复

若 (9.10) 成立，置 \(\ell=\ell_*\)，并定义

\[
\boxed{
w_*=
\frac{E_1+\ell_*\rho}{M5^F}
\in\mathbb Z_{>0}.
}
\tag{10.1}
\]

整数性来自完整 CRT；正性来自 \(E_1,\ell_*,\rho>0\)。唯一需要检查的
完整等式为

\[
\boxed{
w_*
=2^{h+F-2t}
-J\ell_*5^{2a-F-t}.
}
\tag{10.2}
\]

### 定理 10.1

\[
\boxed{(4.7)+(10.2)}
\]

与原条件

\[
E^*=E_1,
\qquad1\le\ell\le L
\]

严格双向等价。

#### 正向

原候选满足 (4.1)，故 \(\ell\) 满足唯一 CRT 类。因
\(1\le\ell<5^F\)，必有 \(\ell=\ell_*\)，并由 (1.21) 直接得到
(10.2)。

#### 反向

(4.7) 给

\[
1\le\ell_*\le5^F-1.
\]

由 (10.1) 有 \(w_*>0\)。若 (10.2) 成立，则

\[
p-J\ell_*5^{q_*}=w_*>0.
\]

全部量均为整数，所以

\[
J\ell_*5^{q_*}\le p-1,
\]

从而

\[
\ell_*\le
\left\lfloor\frac{p-1}{J5^{q_*}}\right\rfloor.
\]

联合五进上界即得 \(1\le\ell_*\le L\)。最后 (10.1) 给

\[
M5^Fw_*-\ell_*\rho=E_1,
\]

所以原静态走廊与深度一终端条件全部恢复。\(\square\)

---

## 11. 一次下降的第二平方 Bezout 坐标

令

\[
y_1=p_1-2J.
\tag{11.1}
\]

对任意整数 \(\ell\ge0\)，定义

\[
\boxed{N_\ell=n_1+M^2\ell,}
\tag{11.2}
\]

\[
\boxed{P_\ell=y_1+CM\ell,}
\tag{11.3}
\]

\[
\boxed{Q_\ell=m_1+C^2\ell.}
\tag{11.4}
\]

由第 3、9 节的恒等式逐项计算得

\[
\boxed{C^2N_\ell-M^2Q_\ell=4,}
\tag{11.5}
\]

\[
\boxed{CN_\ell-MP_\ell=2U,}
\tag{11.6}
\]

\[
\boxed{MQ_\ell-CP_\ell=2D,}
\tag{11.7}
\]

以及

\[
\boxed{
N_\ell Q_\ell-P_\ell^2
=4(E_1+\ell r).
}
\tag{11.8}
\]

式 (11.2)–(11.4) 表明，增加正商 \(\ell\) 正好沿

\[
(M^2,CM,C^2)
\]

移动到平方 Bezout 方程的下一组正解，同时保持三个线性 Bezout 坐标
(11.5)–(11.7)。

若完整候选成立，则

\[
E_1+\ell r=M5^Fp,
\]

所以 (11.8) 精确化为

\[
\boxed{
N_\ell Q_\ell-P_\ell^2
=4M5^Fp
=2^{A+2}5^F.
}
\tag{11.9}
\]

这就是题设第十节所要求的“两个平方 Bezout 解之间的差”的严格实现。
它没有引入新的自由参数，因为 \(\ell\) 已由 (9.10) 唯一确定。

但是，(11.9) 目前没有强迫标准逆元落到统一禁区。若二进接受成立，只能写

\[
\ell_*=\delta_1+Mz
\]

其中 \(z\) 由唯一五进低块 \(e_5\) 固定；\(5^F/M\) 随 \(a\) 增长，
现有平方 Bezout 恒等式没有把该固定高块 \(z\) 压成绝对有限集合。因此
(11.5)–(11.9) 是更强的正规形，而不是分支关闭。

---

## 12. 覆盖全部 \(a\) 的无枚举递推

本节明确给出 GFPmP1-3 所需的完备递推。它对每个状态只计算一个五进低块、
一个二进高位数字和一个完整等式。

### 12.1 尾窗与提升初段

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
\tag{12.1}
\]

随后

\[
\mathcal H(a)=
\{H_a\}\cup
\{H_a-1:5^{H_a}\ge2^{2a-2}\}.
\tag{12.2}
\]

令

\[
T_a=\max\{t:125^t<22\cdot2^{2a-1}\}.
\]

则 \(T_3=1\)，且

\[
T_{a+1}\in\{T_a,T_a+1\},
\tag{12.3}
\]

由下一幂是否满足严格不等式唯一决定；再与 \(2t<a\)、\(h\ge t\)
相交。

### 12.2 低精度逆元 \(x\)

令

\[
P_a=\left\langle5^{-2a}\right\rangle_{4^a},
\qquad P_3=57.
\tag{12.4}
\]

若

\[
25^aP_a=1+Q_a4^a,
\]

取唯一 \(\varepsilon_a\in\{0,1,2,3\}\) 使

\[
Q_a+\varepsilon_a25^a\equiv0\pmod4,
\]

并置 \(\widehat P_a=P_a+\varepsilon_a4^a\)，则

\[
\boxed{
P_{a+1}=
\left\langle25^{-1}\widehat P_a\right\rangle_{4^{a+1}}.
}
\tag{12.5}
\]

对允许的 \(t\)，

\[
\boxed{x_{a,t}=\left\langle2\cdot5^tP_a\right\rangle_{4^a}.}
\tag{12.6}
\]

### 12.3 平方逆元与高位数字

置

\[
\mathfrak M_a=\frac{M^2}{4}=2^{4a-2},
\qquad
g_a=\langle5^{-1}\rangle_{\mathfrak M_a}.
\tag{12.7}
\]

固定 \(a\) 后，以

\[
R_{a,1}=g_a,
\qquad
R_{a,K+1}=\langle g_aR_{a,K}\rangle_{\mathfrak M_a}
\tag{12.8}
\]

得到

\[
R_{a,K}=\langle5^{-K}\rangle_{\mathfrak M_a}.
\]

本报告所需的平方逆元是

\[
\boxed{\iota_1=R_{a,2c_0}.}
\tag{12.9}
\]

然后

\[
n_1=4\iota_1,
\qquad
m_1=\frac{C^2\iota_1-1}{\mathfrak M_a},
\tag{12.10}
\]

并由 (9.9) 只计算一个

\[
\delta_1=\langle\iota_1(D^2-m_1)\rangle_M.
\tag{12.11}
\]

等价地，可用奇数逆元的标准 Hensel–Newton 递推

\[
z^{-1}\pmod{2^{2s}}
=z^{-1}(2-zz^{-1})\pmod{2^{2s}}
\tag{12.12}
\]

把 \(r^{-1}\) 提升到模 \(M^3\)，再由 (9.1)–(9.3) 直接读取
\(\delta_1\)。两条路径必须给出相同数字。

### 12.4 每状态判别

对每个 \(a\ge3\)，递推执行：

1. 由 (12.1)–(12.3) 生成全部 \((t,h)\)；
2. 由 (12.4)–(12.6) 生成 \(x,c,\rho,\eta\)；
3. 对九个 \(J\) 检查全部局部门 (1.12)–(1.14)；
4. 只取
   \[
   a+1\le F\le2a-t-1;
   \]
5. 先检查正商区间 (1.20) 非空；
6. 由 (12.9)–(12.11) 计算唯一 \(n_1,m_1,\delta_1\)；
7. 由 (8.1) 计算唯一 \(e_5\)；
8. 若 \(e_5=0\) 或 \(e_5\not\equiv\delta_1\pmod M\)，拒绝；
9. 否则唯一置 \(\ell_*=e_5\)，并检查 \(\ell_*\le L\)；
10. 只计算一个 \(w_*\)，检查 (10.2)；
11. 若成立，直接回代 (1.21)–(1.23) 和全部继承门。

每个状态没有自由 CRT 选择、自由 \(\ell\)、自由下降深度或移动模 \(r\)
余数搜索。递推覆盖全部 \(a\)，但 \(\delta_1\) 所在的二进位块随 \(a\)
移动，尚未被固定有限状态化。

---

## 13. 精确计算诊断（不承担无界证明）

为攻击公式、端点和符号错误，对 \(3\le a\le150\) 使用两条独立整数路径：

1. 由 \(n_1,m_1,p_1,s_1\) 的二次型计算 \(E_1\)；
2. 独立计算
   \[
   E_1=\left\langle B^{-1}E_0\right\rangle_r^+;
   \]
3. 独立以 \(n_2=\langle U^2r^{-1}\rangle_{M^3}^+\) 读取
   \(\delta_1\)，并与 (9.9) 比较；
4. 以完整 CRT 代表 (4.5) 复核 (8.1)、(9.10)。

全部逐项相同。保留全部局部门、尾窗、大 \(F\) 定理和指数室后的计数为

```text
large-F parameter states = 29266
states with nonempty positive corridor = 24986
e5 = 0 states = 0
binary high-digit accepts = 0
full E2 hits = 0
```

这只说明实现和公式在该前缀没有暴露错误；本文没有把它外推为
\(a\ge151\) 的证明，也没有据此生成规范有限证书包。

---

## 14. 外部素数周期路线的停止点

完整等式 (10.2) 的确可以模外部奇素数检查。但是，在使用该路线制作规范
证书前，必须先把下列移动数据化成固定有限周期：

\[
2^a,\quad5^a,\quad x,\quad\iota_1,\quad m_1,
\quad\delta_1,\quad e_5,
\]

以及由严格整数不等式决定的 \(t,h,F\) 窗口。

当前最早的未决门已经是

\[
e_5\equiv\delta_1\pmod{2^{2a}},
\]

其模数精度随 \(a\) 增长。现有推导没有把它改写成固定外部奇素数上的有限
周期，也没有先把 \(a\) 压到绝对有限。因此有限 \(a\) 前缀不能承担
无界结论；本轮不制作伪周期证书。

这不是断言外部素数路线原则上不可能，而只是本轮没有得到题设要求的完整周期、
每类删除素数、独立验证器和破坏性测试。

---

## 15. 主动审计

### 15.1 \(F=0\)

正商窗为空；此外第 6 节更强地证明所有正商都满足 \(F\ge a+1\)。

### 15.2 \(\ell_{\mathrm{CRT}}=0\)

立即违反 \(\ell>0\)，不能用代表 \(M5^F\) 或 \(5^F\) 代替。

### 15.3 \(E_1\bmod5^F=0\)

此时 \(e_5=0\)，五进标准窗没有正代表，立即拒绝。

### 15.4 \(\gcd(\rho,r)>1\)

可能发生，并且

\[
\gcd(\rho,r)=\gcd(\rho,J).
\]

本文只在模 \(M5^F\mid B\) 下使用 \(\rho^{-1}\)，其合法性来自
\(\rho^2\equiv1\pmod B\)。全文没有除以 \(\rho\pmod r\)。

### 15.5 \(u=0\)

式 (5.6) 明确保留 \(u=0\)。五进赋值结论 (5.9) 不需要 \(u>0\)；
二进分流以 \(v_2(0)=+\infty\) 解释。

### 15.6 \(E_1\) 的正余数窗口

第 3.2 节用 \(U^2<r\) 和 \(0<n_1<M^2\) 独立证明
\(0<E_1<r\)，第 3.3 节再以一次真实反向回放复核。

### 15.7 小端 \(a=3\)

第 7 节逐项使用全部局部门，只有 \(t=0,J=4\) 存活；\(F=4\) 的
正商窗为空，\(F=5\) 满足 \(5^F>10M\)。

### 15.8 是否把 CRT 唯一性误报为分支关闭

没有。唯一性只给 (9.10)–(9.11) 的单个候选；它仍须通过原正商上界和
完整等式 (10.2)。

### 15.9 是否把有限前缀外推

没有。第 13 节只属于诊断；无界完备性来自第 12 节的符号递推，空性尚未
证明。

### 15.10 是否发现继承错误

没有。深度一二次型、直接反向余数、静态双走廊和局部门全部相容。

---

## 16. 最终分类与停止点

本轮严格证明

\[
\boxed{
\begin{gathered}
C^2n_1-M^2m_1=4,\\
p_1^2+4s_1=n_1m_1,\\
E_1=s_1+p_1J-J^2,
\qquad
4E_1=n_1m_1-(p_1-2J)^2,\\
E_1=\langle B^{-1}E_0\rangle_r^+,
\qquad0<E_1<r;\\
F\ge a+1,
\qquad5^F>10M;\\
e_5=
\left\langle-(n_1+U^2)M^{-2}\right\rangle_{5^F};\\
\iota_1=
\left\langle5^{-2c_0}\right\rangle_{M^2/4}^{+},\\
\delta_1=
\left\langle\iota_1(D^2-m_1)\right\rangle_M;\\
\text{CRT 候选存在}
\Longleftrightarrow
e_5\ne0,\qquad e_5\equiv\delta_1\pmod M;\\
\ell_*=e_5;\\
w_*=\dfrac{E_1+\ell_*\rho}{M5^F};\\
(4.7)+(10.2)
\Longleftrightarrow
E^*=E_1,\qquad1\le\ell\le L.
\end{gathered}}
\tag{16.1}
\]

此外，(11.2)–(11.9) 给出了完整的第二平方 Bezout 坐标；第 12 节给出
覆盖全部 \(a\) 的有限递推。每个 \((a,t,h,J,F)\) 至多产生一个显式
整数候选，且不再枚举 \(\ell\)。

但是，尚未证明五进低块 \(e_5\) 永远不能与从模 \(M^2\) 提升到
模 \(M^3\) 的高位数字 \(\delta_1\) 对齐；\(a\) 未绝对有界；也没有
完整外部素数周期证书。因此准确分类为

\[
\boxed{
\mathrm{GFPmP1\text{-}3}:
\quad
\mathscr P_1\text{ 的每个递推状态至多一个显式候选，}
\text{但仍有无界高位 Bezout 残余。}
}
\tag{16.2}
\]

没有找到合法原题解，也没有发现 GFPmR-3、GFPmP0-3 或深度一正规形错误。

本文到此停止，不研究
\(\mathscr P_0\)、六条零商族、\(\mathcal F_{E-}\)、\(\varphi<a\)、
B、C、\(\gamma>1\)、C2/C5、Q 或严格层。
