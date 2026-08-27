# 三项十进制拼接平方和问题：临界 (G) 模板本原 (gamma=1) 的 C2 二进判别式报告

日期：2026-08-07（Asia/Tokyo）

本文严格限定于

\[
\boxed{G_{\mathrm{prim}},\qquad \gamma=1,\qquad \mathrm{C2}.}
\]

接受 PR6、SD6、E4 与 GCU-2 的 C2 终端系统。全文冻结 C1，不研究
A2、B、\(\gamma>1\)、非本原 C2/C5、Q、O 或严格层。

---

## 0. 裁决

本轮严格证明了三条统一二进结论：

\[
\boxed{v_2(k^2-1)=2a,}
\tag{0.1}
\]

\[
\boxed{
q\equiv
\begin{cases}
1\pmod{2^{2a}},&\mathscr C_{2,+},\\
-1\pmod{2^{2a}},&\mathscr C_{2,-},
\end{cases}}
\tag{0.2}
\]

\[
\boxed{
\frac{k^2-1}{2^{2a}}\equiv7\pmod8.
}
\tag{0.3}
\]

并把高位字恢复成显式小模数门。另有两个附加推进：

1. 全部完整 C2 候选满足 \(F\ge1\)；
2. 负支路若有完整候选，则必须落在极端五进端层
   \[
   \boxed{\varphi=e=0,}
   \tag{0.4}
   \]
   且满足一个长度小于 \(\log_2 10\) 的尾窗区间、
   \(v_2(R)=O(\log a)\) 及固定 Jacobi 类。

但是，正支仍有无界外层；负支的 \(\varphi=e=0\) 端层也没有获得
参数无关的 \(a\) 上界。模 (16,32) 的归一化判别式不比 (0.3)
更强，第三块尺度窗口也未产生统一阿基米德间隙。因此准确分类为

\[
\boxed{
\mathrm{GC2B\text{-}4}:
\quad
\alpha=2a,
\quad q\equiv\pm1\pmod{2^{2a}},
\quad (k^2-1)/2^{2a}\equiv7\pmod8,
\text{但仍有无界残余}.}
\tag{0.5}
\]

没有找到合法原题六元组，也没有发现 GCU-2、SD6 或上游 C2 系统错误。

题设第 1 节曾把局部结论 \(\alpha=2a\) 拟名为“GC2B-1”，而第 15 节
又把“GC2B-1”保留给整个 C2 的关闭。为避免同名冲突，本文把局部二进
锁定记为 **GC2B-L1**，最终分类仍按第 15 节使用 GC2B-4。

---

## 1. 继承的 C2 系统

沿用

\[
K=k^2-1,\qquad \alpha=v_2(K),
\]

\[
\mathscr A=ZH_1,\qquad
H_1=a_1T+10a_2,
\qquad v_2(\mathscr A)=A+1,
\]

\[
\mathcal R=(ua_1)^2+a_2^2,
\]

\[
w_0^2=\mathscr A^2-K\mathcal R,
\qquad
L_\pm=\mathscr A\pm kw_0.
\tag{1.1}
\]

C2 中

\[
a\ge3,\qquad a+1\le A\le2a-2,
\tag{1.2}
\]

\[
N=5^R,\qquad
Z=2^A5^F,\qquad
F=A+S-R,
\tag{1.3}
\]

\[
qr=1+ZN=1+2^A5^{A+S},
\qquad k=r+Z,
\tag{1.4}
\]

\[
\frac{5^R}{J+1}<q<\frac{5^R}{J},
\qquad J\in\{1,\ldots,9\}.
\tag{1.5}
\]

又有

\[
qk-1=Z(q+N),
\qquad
v_2(qk-1)=2a-1.
\tag{1.6}
\]

因为 \(m\ge2\)，\(u\) 被 (4) 整除；又因 \(u\mid b_2\) 与
\(\gcd(a_2,b_2)=1\)，有 \(a_2\) 为奇数。因此

\[
\boxed{\mathcal R\equiv1\pmod8.}
\tag{1.7}
\]

事实上

\[
\mathcal R\pmod{32}\in\{1,9,17,25\}.
\tag{1.8}
\]

---

## 2. GC2B-L1：完整共轭尺度强迫 \(\alpha=2a\)

GCU-2 已证明任何完整 C2 候选满足

\[
\alpha<2(A+1),\qquad \alpha\equiv0\pmod2.
\tag{2.1}
\]

由于判别式两项的二进赋值分别为 (2(A+1)) 与 \(\alpha\)，且二者
不同，(1.1) 严格给出

\[
v_2(w_0^2)=\alpha,
\qquad
\boxed{v_2(w_0)=\alpha/2.}
\tag{2.2}
\]

特别地 \(w_0\ne0\)。又因

\[
\frac\alpha2<A+1=v_2(\mathscr A),
\]

两个符号均没有同层消去：

\[
\boxed{v_2(L_+)=v_2(L_-)=\alpha/2.}
\tag{2.3}
\]

现在完整审计尺度恢复。若 \(\varepsilon\in\{+1,-1\}\) 是恢复符号，
则

\[
d=\frac K{\gcd(K,L_\varepsilon)}=2^a5^\varphi.
\]

由于 \(a>0\)，\(\alpha-a<\alpha\)，故

\[
\boxed{v_2(L_\varepsilon)=\alpha-a.}
\tag{2.4}
\]

这一步同时排除 \(L_\varepsilon=0\)。另一方面，逐项展开给出

\[
L_+L_-=K\bigl(k^2\mathcal R-\mathscr A^2\bigr).
\tag{2.5}
\]

括号内是“奇数减偶数”，故为奇非零整数。因此两个共轭因子都非零，
且赋值对其正负号均正常定义，并有

\[
v_2(L_+)+v_2(L_-)=\alpha.
\tag{2.6}
\]

由 (2.4)、(2.6)，共轭符号满足精确等式

\[
\boxed{v_2(L_{-\varepsilon})=a.}
\tag{2.7}
\]

把 (2.3) 与 (2.4)、(2.7) 比较：

\[
\frac\alpha2=\alpha-a=a.
\]

所以

\[
\boxed{\alpha=2a.}
\tag{2.8}
\]

该证明独立使用 C2 的 \(\mathscr A=ZH_1\)、
\(\mathcal R=(ua_1)^2+a_2^2\) 与 \(v_2(\mathscr A)=A+1\)，没有
把 A2 的 GE2-1 结论套入 C2。

### 2.1 零值、符号和端点审计

- 若 \(w_0=0\)，则判别式两项相等，但其赋值分别为
  (2(A+1)) 与 \(\alpha<2(A+1))，不可能；
- (2.5) 的右端非零，故 \(L_+=0\) 与 \(L_-=0\) 均不可能；
- \(L_-<0\) 不影响 (v_2(L_-)\)；只有正的共轭因子可作为恢复符号，
  但 (2.3)、(2.5)–(2.7) 对两个非零因子都成立；
- 恢复符号交换只交换 (2.4) 与 (2.7)，结论不变。

---

## 3. 归一化判别式的模 (8) 门

由 (2.2)、(2.8)，写

\[
\bar w=\frac{w_0}{2^a},\qquad
\bar A=\frac{\mathscr A}{2^{A+1}},\qquad
\bar K=\frac K{2^{2a}}.
\]

三者均为整数，且 \(\bar w,\bar A,\bar K\) 为奇数。判别式化为

\[
\bar w^2
=2^{2(A+1-a)}\bar A^2-\bar K\mathcal R.
\tag{3.1}
\]

C2 中 \(A+1-a\ge2\)，故第一项被 (16) 整除。由 (1.7) 与奇平方
模 (8) 等于 (1)，得到

\[
1\equiv-\bar K\pmod8.
\]

因此

\[
\boxed{\bar K=\frac{k^2-1}{2^{2a}}\equiv7\pmod8.}
\tag{3.2}
\]

这里的负号来自 (3.1)，不能改成 (+\bar K\mathcal R\)。C3 中
\(A+1-a=1\)，第一项只含一个 (4)，所以 (3.2) 不能反向套入 C3。

---

## 4. (q) 的模 (2^{2a}) 主根提升

令

\[
H=2^{2a-1}.
\]

由 (1.6)，存在奇数 (T_2\) 使

\[
qk=1+HT_2,
\qquad
qk\equiv1+H\pmod{2H}.
\tag{4.1}
\]

由 (2.8)，

\[
k^2\equiv1\pmod{2H}.
\tag{4.2}
\]

平方 (4.1)：

\[
(qk)^2\equiv(1+H)^2\equiv1\pmod{2H}.
\]

联合 (4.2) 立即得到

\[
\boxed{q^2\equiv1\pmod{2^{2a}}.}
\tag{4.3}
\]

模 (2^{2a}) 的四个平方根为

\[
1,\quad -1,\quad1+H,\quad-1+H.
\]

若 (k\equiv\pm1\pmod{2^{2a}})，则
\(v_2(k^2-1)\ge2a+1\)，与 (2.8) 矛盾。因此

\[
k\equiv1+H
\quad\text{或}\quad
k\equiv-1+H
\pmod{2^{2a}}.
\tag{4.4}
\]

又因 (k^{-1}\equiv k\pmod{2^{2a}})，由 (4.1) 得

\[
\boxed{
q\equiv
\begin{cases}
1\pmod{2^{2a}},&k\equiv1+H,\\
-1\pmod{2^{2a}},&k\equiv-1+H.
\end{cases}}
\tag{4.5}
\]

所以 GCU-2 的两支严格升级为

\[
\boxed{
\begin{array}{ll}
\mathscr C_{2,+}:&
\eta_2=1,\quad A=2a-2,\quad q\equiv1\pmod{2^{2a}},\\[1mm]
\mathscr C_{2,-}:&
\eta_2=2+v_2(R),\quad A=2a-3-v_2(R),
\quad q\equiv-1\pmod{2^{2a}}.
\end{array}}
\tag{4.6}
\]

当 \(a=3\) 时模数为 (64)，四根恰为

\[
1,\ 63,\ 33,\ 31.
\]

精确赋值排除 (1,63) 作为 (k) 的根，只保留 (33,31)；
负支还因 (0\le v_2(R)\le a-4\) 为空。因此 (a=3) 只可能位于正支。

---

## 5. 高位字与统一小模数门

令 \(\varepsilon=+1\) 表示正支，\(\varepsilon=-1\) 表示负支。
由 (4.4)–(4.6)，唯一写成

\[
\boxed{
k=\varepsilon+HU,
\qquad
q=\varepsilon+2^{2a}Q,
}
\tag{5.1}
\]

其中 (U\) 为正奇数；正支 (Q\ge0\)，负支因 (q>0\) 有 (Q\ge1\)。
第 7 节将证明正支实际也有 (Q\ge1\)。

直接展开：

\[
\frac{k^2-1}{2^{2a}}
=\varepsilon U+2^{2a-2}U^2
\equiv\varepsilon U\pmod8.
\tag{5.2}
\]

所以 (3.2) 等价于

\[
\boxed{
\varepsilon U\equiv7\pmod8.
}
\tag{5.3}
\]

即

\[
U\equiv7\pmod8\quad(\varepsilon=+1),
\qquad
U\equiv1\pmod8\quad(\varepsilon=-1).
\tag{5.4}
\]

定义奇数

\[
W=\frac{q+5^R}{2^{\eta_2}}.
\]

由 (qk-1=Z(q+5^R)) 与 (A+\eta_2=2a-1)，

\[
qk=1+H5^FW.
\tag{5.5}
\]

把 (5.1) 代入并除以 (H)：

\[
5^FW
=\varepsilon U+2\varepsilon Q+2HQU.
\]

由于 (a\ge3)，末项被 (8) 整除，故

\[
\boxed{5^FW\equiv\varepsilon U+2\varepsilon Q\pmod8.}
\tag{5.6}
\]

同时

\[
\boxed{
\frac{q^2-1}{2^{2a}}\equiv2\varepsilon Q\pmod8.
}
\tag{5.7}
\]

因此

\[
\boxed{
\frac K{2^{2a}}
\equiv
5^FW-\frac{q^2-1}{2^{2a}}
\pmod8.
}
\tag{5.8}
\]

所有符号均已在 (5.6)–(5.8) 中显式保留。

---

## 6. 两支的 (W\bmod8\) 与 (Q\bmod4\)

### 6.1 正支

正支中

\[
q=1+2^{2a}Q,
\qquad
W=\frac{q+5^R}{2}.
\]

因 (2^{2a-1}Q\equiv0\pmod8)，

\[
\boxed{W\equiv\frac{1+5^R}{2}\equiv1+2R\pmod8.}
\tag{6.1}
\]

联合 (3.2)、(5.8)，得到固定接受门

\[
\boxed{
Q\equiv
\begin{cases}
R-3\pmod4,&F\equiv0\pmod2,\\
R-1\pmod4,&F\equiv1\pmod2.
\end{cases}}
\tag{6.2}
\]

### 6.2 负支

令

\[
t=v_2(R),\qquad R=2^tR_0,\qquad R_0\text{ 为奇数}.
\]

负支中

\[
q=-1+2^{2a}Q,
\qquad
W=\frac{5^R-1+2^{2a}Q}{2^{2+t}}.
\]

由 (t\le a-4\)，第二项除去 (2^{2+t}) 后仍被 (2^{a+2})
整除，模 (8) 消失。对第一项用二项式及逐次平方，有

\[
\boxed{
W\equiv\omega_t(R_0)\pmod8,
}
\tag{6.3}
\]

其中

\[
\boxed{
\omega_t(R_0)=
\begin{cases}
R_0+4\binom{R_0}{2}\pmod8,&t=0,\\
3R_0\pmod8,&t=1,\\
-R_0\pmod8,&t\ge2.
\end{cases}}
\tag{6.4}
\]

例如 (t=0) 时，(R_0\equiv1,3,5,7\pmod8) 分别给
\(W\equiv1,7,5,3\pmod8\)。

负支的固定接受门为

\[
\boxed{
Q\equiv\frac{7-5^F\omega_t(R_0)}2\pmod4.
}
\tag{6.5}
\]

右侧含义明确：先把偶数剩余类取模 (8)，再除以 (2) 得模 (4)
剩余类。式 (6.2)、(6.5) 等价于对因子 (q) 指定模
\(2^{2a+2}) 的唯一高两位类。

---

## 7. (Q) 的精确区间与 (q=1\) 审计

由 (1.5) 与 (q=\varepsilon+2^{2a}Q)，严格得到

\[
\boxed{
\frac{5^R/(J+1)-\varepsilon}{2^{2a}}
<Q<
\frac{5^R/J-\varepsilon}{2^{2a}}.
}
\tag{7.1}
\]

区间长度恰为

\[
\boxed{
\frac{5^R}{2^{2a}J(J+1)}.
}
\tag{7.2}
\]

因此 (Q) 不是新自由变量：一旦终端因子 (q) 固定，

\[
Q=\frac{q-\varepsilon}{2^{2a}}
\]

唯一确定。但是 (7.2) 没有统一小于 (4)。例如正支取

\[
A=2a-2,\qquad R=S=3a.
\]

则 (F=A,\ \varphi=a\)，且

\[
H(3a)\ge2a
\]

（因为 (5^{3a}=125^a>10^{2a})），所以全部尾窗合法性条件成立；
而 (7.2) 随 (a) 至少按 ((125/4)^a\) 增长。该外层族不宣称存在
因子候选，只严格说明“单靠 (q\sim5^R/J) 的区间长度”不能统一确定
\(Q\bmod4\)。

最后，PR6 已有 (q\ge3\)。也可直接从严格窗口看出：若 (q=1\)，则

\[
J<5^R<J+1,
\]

与 (5^R\) 为整数矛盾。所以正支的 (Q=0\) 不可能，实际有

\[
\boxed{Q\ge1}
\]

对两个支路均成立。

---

## 8. 模 (16,32) 判别式不会进一步分支关闭

由 (1.8)，模 (32) 的 \(\mathcal R\) 总在奇平方子群

\[
\mathscr S_{32}=\{1,9,17,25\}.
\]

\(\bar w^2,\bar A^2\) 也在该集合。

令

\[
h_2=A+1-a\ge2.
\]

若 (h_2\ge3\)，(3.1) 的第一项模 (32) 消失；若 (h_2=2\)，
该项恒为 (16\pmod{32})。两种情况下

\[
2^{2h_2}\bar A^2-\bar w^2
\]

的可达集合都恰为

\[
\mathscr N_{32}=\{7,15,23,31\}.
\]

由于 \(\mathscr S_{32}\) 是乘法子群，除以
\(\mathcal R\in\mathscr S_{32}\) 后仍得到

\[
\boxed{
\bar K\pmod{32}\in\{7,15,23,31\}.
}
\tag{8.1}
\]

这与 \(\bar K\equiv7\pmod8\) 完全等价，没有增加新限制。模 (16)
同理只得到

\[
\bar K\pmod{16}\in\{7,15\}.
\]

所以题设建议的模 (16,32) 提升经过完整 residue-set 审计后不能关闭
任一 C2 支路；特别地，(A=a+1) 的额外 (16) 项不会改变可达集合。

---

## 9. 全因子 Jacobi 门与负支五进端层

记

\[
B_5=A+S=F+R.
\]

由 (q\mid1+2^A5^{B_5})，

\[
2^A5^{B_5}\equiv-1\pmod q.
\]

对正奇复合数 (q) 使用 Jacobi 符号。因两个支路都有
\(q\equiv\pm1\pmod8\)，故

\[
\left(\frac2q\right)=1.
\]

于是

\[
\left(\frac5q\right)^{B_5}
=\left(\frac{-1}q\right)
=\varepsilon.
\tag{9.1}
\]

又因 (5\equiv1\pmod4)，

\[
\left(\frac5q\right)=\left(\frac q5\right).
\]

因此：

\[
\boxed{
\begin{array}{ll}
\mathscr C_{2,+}:&B_5\text{ 为奇数时 }q\equiv\pm1\pmod5;\\
\mathscr C_{2,-}:&B_5\text{ 必为奇数，且 }q\equiv\pm2\pmod5.
\end{array}}
\tag{9.2}
\]

### 9.1 统一排除 (F=0\)

若 (F=0\)，则

\[
Z=2^A,\qquad \varphi=n=a+A.
\]

完整尺度恢复给 (d\mid K\)，而终端窗口给

\[
k<(J+2)Z\le11Z.
\]

所以

\[
2^a5^{a+A}=d\le K<k^2<121\cdot2^{2A}.
\]

即

\[
10^a\left(\frac54\right)^A<121.
\]

但 C2 有 (a\ge3,A\ge a+1\)，左侧至少为

\[
10^3\left(\frac54\right)^4>121,
\]

矛盾。因此

\[
\boxed{F\ge1}
\tag{9.3}
\]

对两个 C2 支路统一成立。

### 9.2 负支只能有 \(\varphi=e=0\)

负支若 \(\varphi\ge1\)，则 (5^\varphi\mid K\) 给
\(k\equiv\pm1\pmod5\)。又由 (9.3)，(5\mid Z\)，故

\[
qk\equiv1\pmod5,
\]

从而 (q\equiv\pm1\pmod5\)。这与负支的 (9.2) 矛盾。
所以

\[
\boxed{\mathscr C_{2,-}\Longrightarrow\varphi=0.}
\tag{9.4}
\]

K5 的支撑门 \(\operatorname{rad}(u)\mid qg\) 与
\(5\nmid qg\) 随即强迫 (e=0\)。于是负支残余满足完整端层正规形

\[
\boxed{
\begin{gathered}
\varphi=e=0,\qquad S=a+R,\qquad F=a+A,\qquad m=R,\\
A=2a-3-t,\qquad t=v_2(R),\qquad0\le t\le a-4,\\
A+H(a+R)=R,\qquad F+R\text{ 为奇数},\\
q\equiv-1\pmod{2^{2a}},\qquad q\equiv\pm2\pmod5.
\end{gathered}}
\tag{9.5}
\]

尾窗等式还等价于

\[
\boxed{
10^{a+A-1}\le2^{a+R}<10^{a+A}.
}
\tag{9.6}
\]

故固定 \((a,t)\)、即固定 (A\) 后，(R\) 落在

\[
(a+A-1)\log_2 10-a
\le R<
(a+A)\log_2 10-a,
\tag{9.7}
\]

一个长度为 \(\log_2 10<4\) 的区间内，至多有四个整数。

另一方面，负支尾带给

\[
3R<27a-30-10t<27a,
\]

而 (2^t\mid R\)。所以

\[
\boxed{2^t\le R<9a,\qquad t<\log_2(9a).}
\tag{9.8}
\]

这把负支压成每个 (a) 的 (O(\log a)\) 个尾窗状态，但没有给
\(a\) 的绝对上界。奇偶门还给

\[
t=0\Longrightarrow a\text{ 为奇数},
\qquad
t\ge1\Longrightarrow a\equiv t\pmod2.
\tag{9.9}
\]

因此负支获得了显著薄化，但尚未关闭。

---

## 10. 五进尺度恢复的一个严格子走廊

以下结论不是关闭 C2 所必需，但记录第二轮五进审计的有效部分。

若

\[
e\ge1,\qquad F\ge\varphi,
\tag{10.1}
\]

则 K5 支撑与逐项既约给

\[
\varphi\ge1,\qquad5\nmid a_2,
\]

并且

\[
v_5(\mathcal R)=0,
\qquad
v_5(H_1)=1,
\qquad
v_5(\mathscr A)=F+1>\varphi.
\tag{10.2}
\]

令 \(\beta=v_5(K)\)。若 \(\beta<2(F+1)\)，判别式的唯一最低项
是 (K\mathcal R\)，与第 2 节同样的恢复赋值比较给

\[
\beta=2\varphi.
\]

若 \(\beta\ge2(F+1)\)，则 (5^{F+1}\) 同时整除 (L_+,L_-\)。
而

\[
k^2\mathcal R-\mathscr A^2
\]

为五进单位，故乘积精确赋值与恢复分别强迫共轭因子的五进阶为
\(\varphi\)，与 (F+1>\varphi\) 矛盾。因此高层室也不存在，严格得到

\[
\boxed{v_5(k^2-1)=2\varphi}
\tag{10.3}
\]

以及

\[
\boxed{
\frac{k^2-1}{5^{2\varphi}}\equiv1\text{ 或 }4\pmod5.
}
\tag{10.4}
\]

该子走廊不覆盖 (e=0\) 或 (F<\varphi\)，所以不能把 (10.3)
写成全 C2 定理。特别地，负支残余恰在 (e=\varphi=0\)，不受此门关闭。

---

## 11. 第三块尺度与阿基米德窗口的审计

SD6 对恢复符号给出

\[
a_3=\frac{L_\varepsilon}{\gcd(K,L_\varepsilon)}
\in[Y,10Y),
\]

\[
Ka_3+d^2\mathscr R_3=2YH_1.
\tag{11.1}
\]

继承的严格符号窗口分别给

\[
L_+\text{ 恢复}:\quad(k-1)a_3<YH_1,
\]

\[
L_-\text{ 恢复}:\quad Ka_3\le YH_1.
\tag{11.2}
\]

所以必要条件仍为

\[
k-1<H_1,
\]

负号恢复还要求

\[
K\le H_1.
\tag{11.3}
\]

在 C2 中 (H_1\) 随 (T=10^m\) 移动，而尾窗只给
\(m=A+H(S)\)。正支存在第 7 节所示的无界合法外层，负支端层又有
\(m=R\asymp a\)。因此 (11.2)–(11.3) 没有产生与
\(a_1,a_2\) 无关的统一上、下界把 (a_3/Y\) 排出 \([1,10)\)。

本轮没有把“判别式为平方”误写成候选；任何后继状态仍必须逐符号检查
精确 gcd、(a_3=Y\) 的允许端点、(a_3=10Y\) 的拒绝端点、逐项既约
及两条主方程回代。

---

## 12. 精确有限诊断

为核对新门而重建了 GCU-2 的 (a\le5\) 完整终端枚举。枚举使用：

1. 全部合法 \((a,A,R,S,J)\) 外层；
2. (q\mid1+2^A5^{A+S}\) 的全部奇因子及严格 (J\)-窗口；
3. 两条旧 \(\eta_2\) 支路；
4. (d\mid K\)；
5. 新的 \(\alpha=2a\)；
6. 新的 (q\bmod2^{2a}\) 根类；
7. 新的 \(\bar K\equiv7\pmod8\)；
8. 全因子 Jacobi 门。

计数如下；括号内依次为正支、负支。

| 阶段 | 总数 | 支路分解 |
|---|---:|---:|
| 合法外层 | 7,749 | 5,337 + 2,412 |
| 双 Euclid 窗口因子 | 997 | 666 + 331 |
| 两条旧二进支路 | 474 | 443 + 31 |
| (d\mid K\) | 77 | 67 + 10 |
| \(\alpha=2a\) | 1 | 1 + 0 |
| (q\equiv\pm1\pmod{2^{2a}}\) | 1 | 1 + 0 |
| \(\bar K\equiv7\pmod8\) | 0 | 0 + 0 |

唯一到达 \(\alpha=2a\) 的状态为

\[
\begin{gathered}
(a,A,R,S,J)=(3,4,18,21,4),\\
q=773634046401,\qquad
r=6163601,\qquad
k=7413601,\\
\varphi=0,\qquad F=7.
\end{gathered}
\]

此时

\[
Q=12088031975\equiv3\pmod4,
\]

而正支 (F\) 为奇、(R=18\) 的门 (6.2) 要求
\(Q\equiv R-1\equiv1\pmod4\)。等价地，

\[
\frac K{2^{2a}}equiv3\pmod8,
\]

故被 (3.2) 删除。

这完整复现了 GCU-2 的旧计数 (7749\to474\to77\)，并把该有限前缀
继续压成 (77\to1\to0\)。该结果只作诊断；它没有被外推到 (a\ge6\)。
对更高 (a\) 的完整因数分解成本快速增长，且在没有绝对有限化前建立证书
不改变理论等级。

---

## 13. 主动审计清单

1. **(a=3\)：** 只有正支；模 (64) 四根已逐个处理，有限诊断的唯一
   \(\alpha=2a\) 状态由模 (8) 门删除。
2. **负支小参数：** (a\ge4\) 由 (0\le v_2(R)\le a-4\) 得到。
3. **(q=1,Q=0\)：** 由 PR6 的 (q\ge3\) 或严格窗口直接排除。
4. **(R\) 奇数、(t=0\)：** 包含在 (6.4)、(9.9) 中。
5. **(t=a-4\)：** (6.3) 中被除后的 (q\) 高位仍含
   (2^{a+2}\)，模 (8) 确实消失。
6. **(A=a+1\)：** 模 (32) 时保留 (16\) 项，但可达集合仍为
   \(\{7,15,23,31\}\)。
7. **(A=2a-2\)：** 正支完整保留；没有把它和 C3 的 (A=a\) 混同。
8. **(w_0=0\)：** 与判别式两项的不同赋值矛盾。
9. **(L_+=0,L_-=0\)：** 由奇非零乘积 (2.5) 排除。
10. **(L_-<0\)：** 赋值按绝对值定义；只影响其能否作为恢复符号。
11. **恢复符号交换：** 只交换 \(\alpha-a\) 与 (a\) 的角色，
    不改变 (2.8)。
12. **唯一最低项：** 只在 \(\alpha<2(A+1)\) 后使用；没有跨越同层。
13. **四个平方根：** (k\) 的两个主根由精确 \(\alpha=2a\) 排除，
    没有错误地把 (q\) 从非平凡根直接升级为主根。
14. **\(\bar K\) 符号：** 归一化判别式是
    (\bar w^2=\cdots-\bar K\mathcal R\)，故得到 (7\)，不是 (1\)。
15. **\(\mathcal R\bmod8,16,32\)：** 分别按奇平方及可能的额外 (16\)
    项完整枚举，没有枚举无限 (a_1,a_2\)。
16. **五进高阶：** 只在 (10.1) 的严格子走廊证明
    (v_5(K)=2\varphi\)，没有套用 A2 的特殊结论。
17. **(a_3=Y\)：** 保留；**(a_3=10Y\)：** 拒绝。
18. **平方但尺度失败：** 仍由精确 gcd 恢复删除。
19. **C3 证书：** 未用于 C2 的无界参数。
20. **有限诊断：** 只记录 (a\le5\)，未外推。
21. **负支 Jacobi：** 对正奇复合 (q\) 使用 Jacobi 符号，不假设
    (q\) 为素数或平方自由。
22. **(F=0\)：** 由统一尺度大小门删除，不依赖 Jacobi 奇偶。
23. **\(\varphi=0\)：** 未默默删除；它正是负支唯一剩余端层。
24. **第三块窗口：** 两恢复符号及相邻端点均继续保留。

---

## 14. 准确停止点

正支的完整必要系统为

\[
\boxed{
\begin{gathered}
a\ge3,\quad A=2a-2,\quad F\ge1,\\
q\mid1+2^A5^{A+S},\quad
\frac{5^R}{J+1}<q<\frac{5^R}{J},\\
q\equiv1\pmod{2^{2a}},\\
Q=(q-1)/2^{2a}\text{ 满足 (6.2)},\\
v_2(k^2-1)=2a,\quad
(k^2-1)/2^{2a}\equiv7\pmod8,
\end{gathered}}
\tag{14.1}
\]

再加全部尾窗、五进尺度、判别式、恢复符号和第三块条件。

负支进一步压成

\[
\boxed{
\begin{gathered}
a\ge4,\quad \varphi=e=0,\quad
t=v_2(R)<\log_2(9a),\\
A=2a-3-t,\quad S=a+R,\quad F=a+A,\quad m=R,\\
10^{a+A-1}\le2^{a+R}<10^{a+A},\\
F+R\text{ 为奇数},\quad
q\equiv-1\pmod{2^{2a}},\quad q\equiv\pm2\pmod5,\\
Q=(q+1)/2^{2a}\text{ 满足 (6.5)},\\
v_2(k^2-1)=2a,\quad
(k^2-1)/2^{2a}\equiv7\pmod8.
\end{gathered}}
\tag{14.2}
\]

式 (14.2) 每个 (a\) 只有 (O(\log a)\) 个外层尾窗状态，但 (a\)
仍可无界；式 (14.1) 甚至保留无界宽的因子窗口。当前没有整体关闭、单支
关闭或绝对有限区域，故不能生成规范有限证书，也不更新 v3 总账的关闭表。

最终分类为

\[
\boxed{\mathrm{GC2B\text{-}4}.}
\]

全文到此停止，不研究 C1、A2、B、\(\gamma>1\)、非本原 C2/C5、Q、O
或严格层。
