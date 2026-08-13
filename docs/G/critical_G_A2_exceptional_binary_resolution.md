# 三项十进制拼接平方和问题：临界 G 模板 A2 异常二进室终结报告

日期：2026-08-06（Asia/Tokyo）

本文严格研究

\[
\boxed{
G_{\mathrm{prim}},\qquad
\gamma=1,\qquad
\mathrm{A2},\qquad
a\ge2,\qquad
\mathrm E_2.
}
\]

接受 PR6、SD6 与 GA2-6 的完整判别式—尺度恢复系统，并核对
GA2H-2、GFPmR-3、GFPmZ-6、GFPmP0-3、GFPmP1-3 及 v3 总账中
与本分支相容的状态。本文不研究 \(\mathcal F_{P-}\)、\(\varphi<a\)、
B、C、\(\gamma>1\)、非本原 C2/C5、Q 或严格层。

本轮得到纯符号分支关闭

\[
\boxed{
\mathrm E_2\Longrightarrow\text{无完整候选},
}
\tag{GE2-1a}
\]

从而 GA2-6 的二进必要二分严格升级为

\[
\boxed{
v_2(k^2-1)=2a
}
\tag{GE2-1b}
\]

对全部完整 A2 候选成立。最终分类为

\[
\boxed{\mathrm{GE2\text{-}1}.}
\]

该证明只发生在判别式平方、精确尺度恢复和共轭因子乘积层；不使用终端
\(J,r,m\)、五进提升、递推族、指数级数、\(a_2\) 枚举或有限计算。

---

## 1. 判别式与精确恢复系统

为避免与其他报告中的 \(A\) 冲突，置

\[
\boxed{\mathcal A=2ZH_1,}
\qquad
\boxed{H_1=a_1T+10a_2,}
\tag{1.1}
\]

\[
\boxed{
R=(5^ea_1)^2+(2a_2)^2,
}
\qquad
\boxed{K=k^2-1.}
\tag{1.2}
\]

归一化判别式为

\[
\boxed{w_0^2=\mathcal A^2-KR,}
\tag{1.3}
\]

两个共轭恢复因子为

\[
\boxed{
L_\varepsilon=\mathcal A+\varepsilon kw_0,
\qquad \varepsilon\in\{\pm1\}.
}
\tag{1.4}
\]

完整候选必须存在一个恢复符号 \(\varepsilon\)，使

\[
\boxed{
d=\frac K{\gcd(K,L_\varepsilon)}=2^a5^\varphi.
}
\tag{1.5}
\]

SD6 还保证 \(k>1\)、\(K>0\)，所以后文的
\(\alpha=v_2(K)\) 总是有限；A2 的原始正整数系统还给
\(Z>0\)、\(H_1>0\)。

---

## 2. 基础赋值核对与恢复因子的精确二进阶

### 2.1 奇偶性与 \(A_2\)

A2 的首块

\[
a_1\in\{5,7,9,11,13\}
\]

全为奇数。因此 \((5^ea_1)^2\) 为奇数，而 \((2a_2)^2\) 被 \(4\)
整除，故

\[
\boxed{v_2(R)=0.}
\tag{2.1}
\]

继承终端系统给 \(k\) 为奇数。又因 \(T=10^m\)、\(m\ge2\)，
\(a_1T\) 与 \(10a_2\) 都是偶数，所以

\[
\boxed{u_2:=v_2(H_1)\ge1.}
\tag{2.2}
\]

A2 中 \(v_2(Z)=2a-1\)，于是

\[
\boxed{
A_2:=v_2(\mathcal A)
=1+(2a-1)+u_2
=2a+u_2.
}
\tag{2.3}
\]

特别地

\[
\boxed{\mathcal A\text{ 为正偶数},\qquad A_2> a.}
\tag{2.4}
\]

### 2.2 从完整恢复严格推出 \(v_2(L_\varepsilon)=\alpha-a\)

记

\[
\alpha=v_2(K).
\]

对完成恢复的符号 \(\varepsilon\)，由 (1.5) 取二进赋值得

\[
v_2\bigl(\gcd(K,L_\varepsilon)\bigr)=\alpha-a.
\tag{2.5}
\]

约定 \(v_2(0)=+\infty\)。一般地

\[
v_2\bigl(\gcd(K,L_\varepsilon)\bigr)
=\min\bigl(\alpha,v_2(L_\varepsilon)\bigr).
\tag{2.6}
\]

因为 \(a>0\)，有 \(\alpha-a<\alpha\)。所以 (2.5)–(2.6) 的最小值
不可能由第一项 \(\alpha\) 取得，只能强迫

\[
\boxed{v_2(L_\varepsilon)=\alpha-a.}
\tag{2.7}
\]

这不是下界，而是精确等式；它也同时排除了恢复因子
\(L_\varepsilon=0\)。

---

## 3. 异常室给两个恢复因子的共同二进因子

GA2-6 的异常二进室定义为

\[
\boxed{
\mathrm E_2:\qquad \alpha\ge2A_2.
}
\tag{3.1}
\]

由 \(v_2(\mathcal A)=A_2\)，有

\[
2^{2A_2}\mid\mathcal A^2.
\tag{3.2}
\]

又由 (2.1)、(3.1)，

\[
v_2(KR)=v_2(K)=\alpha\ge2A_2,
\]

所以

\[
2^{2A_2}\mid KR.
\tag{3.3}
\]

将 (3.2)–(3.3) 代入判别式 (1.3)，得到

\[
2^{2A_2}\mid w_0^2.
\]

由于 \(w_0\in\mathbb Z_{\ge0}\)，包括 \(w_0=0\) 在内，均有

\[
\boxed{v_2(w_0)\ge A_2.}
\tag{3.4}
\]

因此 \(\mathcal A\) 与 \(kw_0\) 都被 \(2^{A_2}\) 整除。无论两项
是否在同层发生更高阶消去，对两个符号都严格有

\[
\boxed{
v_2(L_+)\ge A_2,
\qquad
v_2(L_-)\ge A_2.
}
\tag{3.5}
\]

这里同时覆盖 \(\alpha=2A_2\) 与 \(\alpha>2A_2\)，没有使用
“两项赋值的最小值”等式。

---

## 4. 共轭乘积的精确二进赋值

由 (1.3)–(1.4) 逐项展开：

\[
\begin{aligned}
L_+L_-
&=(\mathcal A+kw_0)(\mathcal A-kw_0)\\
&=\mathcal A^2-k^2w_0^2\\
&=\mathcal A^2-k^2(\mathcal A^2-KR)\\
&=(1-k^2)\mathcal A^2+k^2KR\\
&=\boxed{K(k^2R-\mathcal A^2)}.
\end{aligned}
\tag{4.1}
\]

因为 \(k\) 与 \(R\) 都是奇数，而 \(\mathcal A\) 为偶数，

\[
k^2R\equiv1\pmod2,
\qquad
\mathcal A^2\equiv0\pmod2.
\]

故

\[
\boxed{k^2R-\mathcal A^2\text{ 为奇数}.}
\tag{4.2}
\]

该奇因子尤其非零。结合 \(K>0\)，(4.1) 的乘积非零，两个
\(L_\pm\) 都非零，并且

\[
\boxed{
v_2(L_+L_-)=v_2(K)=\alpha.
}
\tag{4.3}
\]

因而可以无损使用非零整数乘积的赋值可加性：

\[
\boxed{v_2(L_+)+v_2(L_-)=\alpha.}
\tag{4.4}
\]

---

## 5. 最终矛盾

假设异常室中存在完整候选，并令 \(\varepsilon\) 为完成 (1.5) 的恢复
符号。由 (2.7)，

\[
v_2(L_\varepsilon)=\alpha-a.
\tag{5.1}
\]

将其代入 (4.4)，共轭因子的赋值被精确强迫为

\[
\boxed{
v_2(L_{-\varepsilon})
=\alpha-(\alpha-a)=a.
}
\tag{5.2}
\]

另一方面，(3.5) 对两个符号同时成立，故

\[
v_2(L_{-\varepsilon})\ge A_2.
\tag{5.3}
\]

联合 (2.3)、(5.2)–(5.3)：

\[
a=v_2(L_{-\varepsilon})
\ge A_2
=2a+u_2
>a,
\]

矛盾。因此

\[
\boxed{
\mathrm E_2\Longrightarrow\text{无完整候选}.
}
\tag{5.4}
\]

注意 (5.2) 的等号来自乘积精确赋值 (4.4)，不是把 SD6 的一般下界
\(v_2(L_{-\varepsilon})\ge a\) 擅自加强。

---

## 6. 十项主动反例攻击

### 6.1 \(\alpha=2A_2\)

式 (3.2)–(3.5) 只使用“至少整除”，故等号端点完整包含。乘积式仍给
\(v_2(L_+L_-)=2A_2\)，再由恢复赋值得到同一矛盾。

### 6.2 \(\alpha>2A_2\)

严格异常室同样满足 (3.5)；(4.3)–(5.3) 不要求
\(\alpha=2A_2\)，所以没有遗漏高层状态。

### 6.3 \(w_0=0\)

若 \(w_0=0\)，(1.3) 给 \(\mathcal A^2=KR\)。由 \(R\) 为奇数，

\[
\alpha=2A_2,
\]

所以它只能落在异常室的等号端点。此时

\[
L_+=L_-=\mathcal A,
\qquad
v_2(L_\pm)=A_2,
\]

且 (4.1) 仍成立。若任一相同因子完成恢复，(2.7) 要求
\(A_2=2A_2-a\)，即 \(A_2=a\)，与 \(A_2=2a+u_2>a\) 矛盾。

### 6.4 两个恢复因子相等或互为相反数

因 \(k>1\)，\(L_+=L_-\) 当且仅当 \(w_0=0\)，已由 6.3 删除。
若 \(L_+=-L_-\)，则 \(L_++L_-=2\mathcal A=0\)，但
\(\mathcal A=2ZH_1>0\)，不可能发生。

### 6.5 \(L_\varepsilon=0\)

一方面，(1.5) 会给

\[
d=K/\gcd(K,0)=1,
\]

与 \(d=2^a5^\varphi>1\) 矛盾；另一方面，(4.1) 的右端是非零的
\(K\) 乘以奇数，也独立排除了零因子。

### 6.6 恢复 gcd 是否真的强迫 (2.7)

是。关键是 \(\alpha-a<\alpha\)，故
\(\min(\alpha,v_2(L_\varepsilon))=\alpha-a\) 不可能停在第一项。
因此只能有精确等式 \(v_2(L_\varepsilon)=\alpha-a\)。

### 6.7 \(k^2R-\mathcal A^2\) 是否可能为偶数

不可能。奇数 \(k^2R\) 减去偶数 \(\mathcal A^2\) 始终为奇数；该结论
与其正负无关。

### 6.8 是否把共轭因子的下界误写成等号

没有。一般互补尺度只给 \(v_2(L_{-\varepsilon})\ge a\)；本文的
\(v_2(L_{-\varepsilon})=a\) 专门由非零乘积的精确赋值
(4.4) 减去 (5.1) 得到。

### 6.9 乘积是否遗漏符号或零因子

赋值对负非零整数按绝对值定义，不受 \(L_-\) 的符号影响；(4.2) 又保证
乘积非零。因此 (4.3)–(4.4) 没有符号或零因子例外。

### 6.10 是否依赖 \(\varphi\ge a\)

不依赖。\(\varphi\) 只通过 \(d=2^a5^\varphi\) 提供
\(v_2(d)=a\)；证明没有使用 \(\varphi\ge a\)、五进提升或
\(\sigma=\pm1\)。

---

## 7. 与 GA2-6 的关系

GA2-6 已正确证明全部完整 A2 候选必须落入互斥必要二分

\[
\mathrm P_2:\quad\alpha=2a,
\]

或

\[
\mathrm E_2:\quad\alpha\ge2A_2.
\]

该推导没有错误。它在异常室中也正确识别出：恢复只能使用高消去因子，
而共轭归一化因子的二进阶为 \(1\)。本报告新增的是把

1. GA2-6 的精确恢复赋值；
2. SD6 的完整共轭乘积；
3. 异常室对两个因子的共同整除

三者合并，从而删除此前作为过宽必要室保留的 \(\mathrm E_2\)。因此这是
对 GA2-6 的严格加强，不是继承错误或 GA2-5。

由 (5.4) 与 GA2-6 的完备二分，严格得到

\[
\boxed{
v_2(k^2-1)=2a
}
\tag{7.1}
\]

对全部完整 A2 候选成立。

---

## 8. 对高 \(\varphi\) 三族的影响

GA2H-2 将

\[
G_{\mathrm{prim}},\quad
\gamma=1,\quad
\mathrm{A2},\quad
a\ge3,\quad
\varphi\ge a
\]

完备压成

\[
\mathcal F_+,qquad
\mathcal F_{P-},\qquad
\mathcal F_{E-}.
\]

其中 \(\mathcal F_{E-}\subset\mathrm E_2\)，故 (5.4) 立即给

\[
\boxed{
\mathcal F_{E-}\Longrightarrow\text{无候选}.
}
\tag{8.1}
\]

联合已经冻结的

\[
\mathcal F_+\Longrightarrow\text{无候选},
\]

高 \(\varphi\) 区只剩

\[
\boxed{\mathcal F_{P-}.}
\tag{8.2}
\]

其当前状态必须保持为：

1. 六条零商族已压成移动高位 Bezout 正规形；
2. \(\mathscr P_0\) 与 \(\mathscr P_1\) 的每个递推状态至多一个显式
   整数候选；
3. 零商与两个正商族均仍受随 \(a\) 移动的高位二进 Bezout 数字控制；
4. 尚未得到统一关闭、绝对有限化或固定外部素数周期证书。

所以本报告没有、也不得把整个高 \(\varphi\) 区误报为空。

---

## 9. 证明的精确作用域

GE2-1：

- 不依赖恢复符号之外的 \(\sigma=\pm1\) 五进根类；
- 不依赖 \(\varphi\ge a\)；
- 不依赖终端 \(J,r,m\)；
- 不依赖五进提升；
- 不依赖递推族或指数级数；
- 不依赖 \(a_2\) 的有限枚举；
- 不依赖判别式平方以外的机器筛选。

其准确范围是：只要处于

\[
G_{\mathrm{prim}},\quad\gamma=1,\quad\mathrm{A2}
\]

的完整判别式—恢复系统，并满足 \(\alpha\ge2A_2\)，即被删除。该结论
不外推到 B、C、\(\gamma>1\)、非本原层、Q 或严格层。

---

## 10. 最终分类与停止点

十项主动反例攻击全部通过；没有找到合法原题解，也没有发现 GA2-6、SD6、
PR6 或恢复公式错误。因此准确分类为

\[
\boxed{
\mathrm{GE2\text{-}1}:
\quad
\mathrm E_2\Longrightarrow\text{无完整候选},
\qquad
v_2(k^2-1)=2a.
}
\]

高 \(\varphi\) 区据此删除 \(\mathcal F_{E-}\)，但
\(\mathcal F_{P-}\) 仍开放。本文到此停止，不研究
\(\mathcal F_{P-}\)、\(\varphi<a\)、B、C、\(\gamma>1\)、
C2/C5、Q 或严格层。
