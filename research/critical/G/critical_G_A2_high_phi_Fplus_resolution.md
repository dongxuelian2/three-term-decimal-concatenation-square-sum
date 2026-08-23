# 三项十进制拼接平方和问题：临界 G 模板 A2 高 \(\varphi\) 正符号主室族终结报告

日期：2026-08-01（Asia/Tokyo）

本文严格限定于

\[
\boxed{
\mathcal F_+:
\quad
G_{\mathrm{prim}},\quad
\gamma=1,\quad
\mathrm{A2},\quad
a\ge3,\quad
t=0,\quad
\varphi=a,\quad
\mathrm P_2,\quad
\sigma=+1,\quad
J\in\{5,9\}.
}
\]

接受 `critical_G_A2_high_phi_single_lift_campaign.md` 的 GA2H-2 双向正规形、
`critical_G_A2_unit_determinant_campaign.md` 的 GA2-6 终端系统与判别式大小门，
以及 PR6、SD6、GA1-1 和 v3 总账中与上述继承链相容的结论。本文不研究
\(\mathcal F_{P-}\)、\(\mathcal F_{E-}\)、\(\varphi<a\)、B、C、
\(\gamma>1\)、C2/C5、Q 或严格层。

最终结论为

\[
\boxed{
\mathcal F_+\Longrightarrow\text{无候选}.
}
\tag{GFP}
\]

结论在终端因子层完成，不进入 \(a_2\)、判别式平方、两个恢复符号或原题回代。
按题设分类，这是

\[
\boxed{\mathrm{GFP\text{-}1}.}
\]

---

## 1. 闭式终端系统及其完整恢复

固定

\[
a\ge3,\qquad h\in\mathcal H(a),\qquad J\in\{5,9\},
\]

并置

\[
A=100^a=10^{2a},\qquad d_{\mathrm{sc}}=10^a,\qquad
Z=\frac A2,\qquad e=2a+h,
\tag{1.1}
\]

这里把继承尺度记为 \(d_{\mathrm{sc}}\)，以免与题设第三下降中临时使用的
字母 \(d\) 冲突；该尺度在终端整除论证中不再单独出现。第三下降的新整数将在
本文记为 \(\delta\)。

\[
r=1+JA,
\qquad
k=1+\frac{2J+1}{2}A.
\tag{1.2}
\]

令

\[
\nu=m-e\ge0,
\qquad
N=2^{2a+h}10^\nu.
\tag{1.3}
\]

继承终端方程为

\[
qr=1+2ZN=1+AN.
\tag{1.4}
\]

由于 \(JA\equiv-1\pmod r\)，若 \(r\mid1+AN\)，则

\[
J(1+AN)\equiv J-N\equiv0\pmod r,
\]

所以 \(r\mid N-J\)。反过来，若

\[
N=J+s_0r,
\qquad
s_0=\frac{N-J}{r},
\tag{1.5}
\]

则

\[
1+AN
=1+A(J+s_0r)
=r(1+As_0).
\]

故有严格双向等价

\[
\boxed{qr=1+AN\iff r\mid N-J.}
\tag{1.6}
\]

本支中 \(h\ge1\)，故 \(N\ge2^{2a+1}>J\)，从而 \(s_0>0\)。并且

\[
\boxed{q=1+As_0.}
\tag{1.7}
\]

由 \(2JZ=JA\)，

\[
\boxed{\rho_0=r-2JZ=1.}
\tag{1.8}
\]

最后

\[
Jq+s_0
=J(1+As_0)+s_0
=J+s_0(1+JA)
=N.
\]

因此完整恢复确为

\[
\boxed{
q=1+As_0,\qquad
\rho_0=1,\qquad
N=Jq+s_0.
}
\tag{1.9}
\]

所以本族唯一的终端整除门就是

\[
\boxed{
1+J100^a
\mid
2^{2a+h}10^\nu-J.
}
\tag{1.10}
\]

没有遗漏额外的 \(q,s_0,\rho_0\) 恢复条件。

---

## 2. 精确指数上界与三层穷尽

继承的必要大小门为

\[
20\cdot10^m<194029Z^2Y,
\qquad
Z=\frac{10^{2a}}2,
\qquad
Y=10^{3a}.
\tag{2.1}
\]

因

\[
Z^2Y=\frac{10^{7a}}4,
\]

(2.1) 等价于

\[
80\cdot10^m<194029\cdot10^{7a}.
\tag{2.2}
\]

若 \(m\ge7a+4\)，则左端至少为

\[
80\cdot10^{7a+4}=800000\cdot10^{7a}
>194029\cdot10^{7a},
\]

与 (2.2) 矛盾。因此完全不用浮点对数便得到

\[
\boxed{m\le7a+3.}
\tag{2.3}
\]

由 \(e=2a+h\) 和 \(\nu=m-e\ge0\)，

\[
\boxed{0\le\nu\le5a+3-h.}
\tag{2.4}
\]

尾窗为

\[
\mathcal H(a)=
\left\{h\ge0:
2^{2a-2}\le5^{h+1},\quad
5^h<2^{2a-1}
\right\}.
\tag{2.5}
\]

当 \(a\ge3\) 时，\(h=0\) 会给 \(2^{2a-2}\le5\)，而左端至少为
\(16\)，不可能；故 \(h\ge1\)。若 \(h\ge a\)，则

\[
5^h\ge5^a>4^a>\frac{4^a}{2}=2^{2a-1},
\]

又与尾窗上端矛盾。因此

\[
\boxed{1\le h\le a-1.}
\tag{2.6}
\]

由 (2.4)、(2.6)，

\[
\nu\le5a+2<6a.
\tag{2.7}
\]

对 \(\nu\) 关于 \(2a\) 作唯一欧几里得分解：

\[
\boxed{
\nu=2aj+v,
\qquad
j\in\{0,1,2\},
\qquad
0\le v<2a.
}
\tag{2.8}
\]

若 \(j=2\)，再由 (2.4) 得

\[
4a+v\le5a+3-h,
\]

即

\[
\boxed{0\le v\le a+3-h.}
\tag{2.9}
\]

所以三层 \(j=0,1,2\) 严格穷尽全部允许指数，没有无界残余。

---

## 3. 第一下降层 \(j=0\)

设

\[
\nu=v,
\qquad
L_v=2^{2a}5^v.
\tag{3.1}
\]

因 \(0\le v<2a\)，有 \(L_v\mid A\)，所以

\[
r\equiv1\pmod{L_v}.
\]

同时

\[
N=2^{2a+h}10^v
\equiv0\pmod{L_v}.
\]

将 \(N=J+s_0r\) 模 \(L_v\) 化简，得到

\[
\boxed{s_0\equiv-J\pmod{L_v}.}
\tag{3.2}
\]

另一方面，由 \(r>JA\)，

\[
0<s_0=\frac{N-J}{r}<\frac{N}{JA}
=\frac{2^{h+v}}{J5^{2a-v}}.
\tag{3.3}
\]

又因 \(h\le a-1\)、\(v\le2a-1\)，有 \(h+v\le3a-2\)，故

\[
\frac{\dfrac{2^{h+v}}{J5^{2a-v}}}{L_v/2}
=\frac{2^{h+v-2a+1}}{J5^{2a}}
\le\frac{2^{a-1}}{J5^{2a}}<1.
\]

因此

\[
s_0<\frac{L_v}{2}.
\tag{3.4}
\]

并且

\[
L_v\ge2^{2a}\ge64>18\ge2J,
\]

所以

\[
\frac{L_v}{2}<L_v-J.
\tag{3.5}
\]

式 (3.2) 的最小正代表为 \(L_v-J\)，但 (3.4)–(3.5) 给出

\[
0<s_0<L_v-J,
\]

矛盾。故

\[
\boxed{j=0\text{ 全空}.}
\tag{3.6}
\]

---

## 4. 第二下降层 \(j=1\)

设

\[
\nu=2a+v,
\qquad0\le v<2a.
\tag{4.1}
\]

此时 \(A\mid N\)、\(r\equiv1\pmod A\)，故

\[
s_0\equiv-J\pmod A.
\]

唯一写成

\[
s_0=-J+Ac,
\qquad c\in\mathbb Z_{>0}.
\tag{4.2}
\]

将其代入 \(N=J+s_0r\)，得到

\[
N=A(cr-J^2).
\]

而本层

\[
\frac NA=2^{2a+h}10^v,
\]

所以

\[
\boxed{cr=J^2+2^{2a+h}10^v.}
\tag{4.3}
\]

模 \(L_v=2^{2a}5^v\) 使用 \(r\equiv1\)、
\(L_v\mid2^{2a+h}10^v\)，得到

\[
\boxed{c\equiv J^2\pmod{L_v}.}
\tag{4.4}
\]

由 (4.3)、\(r>JA\) 及第 3 节已经证明的同一上界，

\[
0<c
<\frac{J^2}{JA}
+\frac{2^{2a+h}10^v}{JA}
<1+\frac{L_v}{2}
<L_v.
\tag{4.5}
\]

若 \(L_v>J^2\)，则 (4.4)、(4.5) 强迫

\[
c=J^2.
\]

代入 (4.3)，消去公共因子后得到

\[
\boxed{J^3 5^{2a-v}=2^{h+v}.}
\tag{4.6}
\]

由于 \(v<2a\)，左端含正次数的奇素因子：\(J=5\) 时含 \(5\)，
\(J=9\) 时含 \(3\)；右端是纯二次幂，矛盾。

现处理 \(L_v\le J^2\)。因为

\[
L_v=2^{2a}5^v\ge64,
\]

当 \(J=5\) 时已有 \(L_v>25\)；当 \(J=9\) 时，若 \(a\ge4\) 则
\(L_v\ge256>81\)，若 \(a=3,v\ge1\) 则 \(L_v\ge320>81\)。故唯一边界是

\[
\boxed{(a,v,J)=(3,0,9).}
\tag{4.7}
\]

此时 \(L_v=64\)，由 (4.4)、(4.5)，

\[
c\equiv81\equiv17\pmod{64},
\qquad0<c<64,
\]

故 \(c=17\)。又 \(\mathcal H(3)=\{1,2\}\)，于是 (4.3) 右端至多为

\[
81+2^{8}=337,
\]

而左端为

\[
17(1+9\cdot100^3)=153000017,
\]

不可能相等。因此

\[
\boxed{j=1\text{ 全空}.}
\tag{4.8}
\]

---

## 5. 第三下降层 \(j=2\)：统一大端删除

设

\[
\nu=4a+v,
\qquad
0\le v<2a,
\qquad
v\le a+3-h.
\tag{5.1}
\]

仍写

\[
s_0=-J+Ac.
\]

为避免把第二层公式机械照搬到第三层，先明确本层的正确缩放。现在

\[
\frac NA
=A\,2^{2a+h}10^v.
\]

所以由 \(N=A(cr-J^2)\) 得

\[
\boxed{
cr=J^2+A\,2^{2a+h}10^v.
}
\tag{5.2}
\]

模 \(A\) 使用 \(r\equiv1\pmod A\)，得到

\[
c\equiv J^2\pmod A.
\]

唯一写成

\[
c=J^2+A\delta,
\qquad \delta\in\mathbb Z.
\tag{5.3}
\]

代入 (5.2)，并用 \(r=1+JA\)，严格得到

\[
\boxed{
\delta r=2^{2a+h}10^v-J^3.
}
\tag{5.4}
\]

这就是题设 (D2.1)，其中题设临时记作 \(d\) 的下降整数在本文为
\(\delta\)。下面证明 \(\delta>0\)。由 (5.2) 有 \(c>0\)。若
\(\delta\le-1\)，则

\[
c=J^2+A\delta\le J^2-A<0
\]

（这里 \(A\ge10^6>81\)），矛盾；故 \(\delta\ge0\)。若
\(\delta=0\)，
(5.4) 会令偶数 \(2^{2a+h}10^v\) 等于奇数 \(J^3\)，仍不可能。因此

\[
\boxed{\delta>0.}
\tag{5.5}
\]

令

\[
L_v=2^{2a}5^v.
\]

因 \(v<2a\)，有 \(L_v\mid A\)；又
\(L_v\mid2^{2a+h}10^v\)。将 (5.4) 模 \(L_v\) 化简：

\[
\boxed{\delta\equiv-J^3\pmod{L_v}.}
\tag{5.6}
\]

由 (5.4)、\(r>JA\) 及 (5.5)，

\[
0<\delta
<\frac{2^{2a+h}10^v}{JA}
=\frac{2^{h+v}}{J5^{2a-v}}.
\tag{5.7}
\]

第三层尾端 \(v\le a+3-h\) 给出 \(h+v\le a+3\)，故

\[
\frac{\dfrac{2^{h+v}}{J5^{2a-v}}}{L_v/2}
=\frac{2^{h+v-2a+1}}{J5^{2a}}
\le\frac{2^{4-a}}{J5^{2a}}<1.
\]

因此

\[
\boxed{0<\delta<\frac{L_v}{2}.}
\tag{5.8}
\]

若

\[
L_v>2J^3,
\]

则 \(0<J^3<L_v/2\)，而 (5.6) 的最小正代表为

\[
L_v-J^3>\frac{L_v}{2},
\]

与 (5.8) 矛盾。于是全部大端被一个符号不等式统一删除，只剩

\[
\boxed{L_v=2^{2a}5^v\le2J^3.}
\tag{5.9}
\]

该边界由固定常数 \(J\in\{5,9\}\) 控制，因而是真正有限边界，而不是
对无界 \(a\) 的抽样。

---

## 6. 第三层有限边界的完整枚举

### 6.1 边界参数穷尽

当 \(J=5\) 时，阈值为

\[
2J^3=250.
\]

若 \(a\ge4\)，则 \(L_v\ge2^8=256>250\)；故只能有 \(a=3\)。
此时 \(v\ge1\) 又给 \(L_v\ge64\cdot5=320>250\)，所以只能有
\(v=0\)。由尾窗直接算得

\[
\mathcal H(3)=\{1,2\}.
\]

当 \(J=9\) 时，阈值为

\[
2J^3=1458.
\]

若 \(a\ge6\)，则 \(L_v\ge2^{12}=4096>1458\)。对剩余三个 \(a\)：

\[
\begin{array}{c|c|c}
a&\mathcal H(a)&\text{允许的 }v\text{（同时满足第三层上界）}\\
\hline
3&\{1,2\}&0,1\\
4&\{2,3\}&0,1\\
5&\{3\}&0
\end{array}
\tag{6.1}
\]

这里阈值相邻比较分别为

\[
320\le1458<1600,
\qquad
1280\le1458<6400,
\qquad
1024\le1458<5120.
\tag{6.2}
\]

因此 (5.9) 恰产生以下 11 个 \((a,h,v,J)\) 状态，没有遗漏。

### 6.2 对 (5.4) 的逐项整数核对

下表记

\[
B=2^{2a+h}10^v,
\qquad
R=B-J^3.
\]

方程 (5.4) 即 \(\delta r=R\)，其中 \(\delta\in\mathbb Z_{>0}\)。

| \(J\) | \(a\) | \(h\) | \(v\) | \(L_v\) | \(B\) | \(R=B-J^3\) | \(r=1+J100^a\) |
|---:|---:|---:|---:|---:|---:|---:|---:|
| 5 | 3 | 1 | 0 | 64 | 128 | 3 | 5,000,001 |
| 5 | 3 | 2 | 0 | 64 | 256 | 131 | 5,000,001 |
| 9 | 3 | 1 | 0 | 64 | 128 | -601 | 9,000,001 |
| 9 | 3 | 1 | 1 | 320 | 1,280 | 551 | 9,000,001 |
| 9 | 3 | 2 | 0 | 64 | 256 | -473 | 9,000,001 |
| 9 | 3 | 2 | 1 | 320 | 2,560 | 1,831 | 9,000,001 |
| 9 | 4 | 2 | 0 | 256 | 1,024 | 295 | 900,000,001 |
| 9 | 4 | 2 | 1 | 1,280 | 10,240 | 9,511 | 900,000,001 |
| 9 | 4 | 3 | 0 | 256 | 2,048 | 1,319 | 900,000,001 |
| 9 | 4 | 3 | 1 | 1,280 | 20,480 | 19,751 | 900,000,001 |
| 9 | 5 | 3 | 0 | 1,024 | 8,192 | 7,463 | 90,000,000,001 |

每一行都满足

\[
R\ne0,
\qquad
|R|<r.
\]

若 \(R<0\)，显然不可能等于 \(\delta r>0\)；若 \(R>0\)，则
\(0<R<r\)，也不可能等于正整数倍 \(\delta r\)。故 11 行全部失败，得到

\[
\boxed{j=2\text{ 全空}.}
\tag{6.3}
\]

---

## 7. 独立有限边界证书

附件包含：

1. `critical_G_A2_high_phi_Fplus_finite_generator.py`：只从
   \(L_v\le2J^3\) 出发生成有限边界，不枚举一般 \(a\)；
2. `critical_G_A2_high_phi_Fplus_finite_verifier.py`：不导入生成器，改用
   尾窗最大指标公式独立重建 \(\mathcal H(a)\)、第三层 \(v\) 上界、阈值前沿及
   11 行整数数据；
3. `critical_G_A2_high_phi_Fplus_finite_certificate.json`：排序键、无空白歧义、
   末尾单换行的规范 UTF-8 JSON 证书。

验证器检查：

- 每个 \(h\) 确属 \(\mathcal H(a)\)；
- 每个 \(v\) 满足 \(0\le v<2a\) 与 \(v\le a+3-h\)；
- 边界内状态恰为 11 个；
- 每行 (5.4) 均无正整数 \(\delta\)；
- 阈值相邻状态分别位于正确的内外侧；
- 删除一行、篡改算术值、放入非法 \(h\)、越过第三层 \(v\) 上界、加入首个
  阈值外状态时，验证器均必须拒绝。

规范运行输出为

```text
independently verified F+ finite boundary: states=11 positive_integer_d_solutions=0
certificate_sha256=8000471c2a80bec6e3f63a6687a9baded0637b59524f03533fb95c8f49e6e529
destruction tests: passed
```

其中机器字段 `positive_integer_d_solutions` 沿用题设 (D2.1) 的临时字母
\(d\)，对应本文的 \(\delta\)，不对应继承尺度 \(d_{\mathrm{sc}}=10^a\)。

验证命令：

```bash
python3 critical_G_A2_high_phi_Fplus_finite_verifier.py \
  critical_G_A2_high_phi_Fplus_finite_certificate.json --destruction-tests
```

SHA-256：

```text
critical_G_A2_high_phi_Fplus_finite_generator.py
b1f470f41ec62631b701e102567d09fcc48945130e300ac7247dce2c470f30b6

critical_G_A2_high_phi_Fplus_finite_verifier.py
a7935fed12d093ff7d9a76de65d08a13a4def20d45785d1039896a44af84b65f

critical_G_A2_high_phi_Fplus_finite_certificate.json
8000471c2a80bec6e3f63a6687a9baded0637b59524f03533fb95c8f49e6e529
```

该证书只承担第 6 节的有限小端；第 2–5 节的一般定理均为符号证明，未用有限
\(a\) 样本外推。

---

## 8. 完整终结

第 2 节已经证明全部允许指数唯一落在

\[
\nu=2aj+v,
\qquad j\in\{0,1,2\},
\qquad0\le v<2a.
\]

第 3、4、5–6 节分别证明

\[
j=0\text{ 全空},
\qquad
j=1\text{ 全空},
\qquad
j=2\text{ 全空}.
\]

故没有任何 \(\nu\)，从而没有任何终端因子状态。由第 1 节的双向恢复，

\[
\boxed{
\mathcal F_+Longrightarrow\text{无候选}.
}
\tag{8.1}
\]

关闭发生在 \((a,h,J,\nu,N,r)\) 的终端因子层，因此自动覆盖：

- 全部 \(a\ge3\)；
- 全部真实 \(h\in\mathcal H(a)\)；
- \(J=5,9\)；
- 判别式大小门允许的全部完整有限指数段；
- 五个 A2 首块；
- 全部真实 \(a_2,a_3\)；
- 两个恢复符号；
- 后续判别式、尺度、逐项既约与原题回代。

这里“自动覆盖”的含义是：这些后续对象只有在终端状态存在时才会被生成；本文已在
其共同前置门处证明终端状态为空，而不是对后续变量另作枚举。

---

## 9. 主动审计

### 9.1 是否用浮点对数决定 \(m\) 的端点

没有。\(m\le7a+3\) 只由整数比较

\[
800000>194029
\]

推出。

### 9.2 是否只检查有限多个 \(a\)

没有。全部 \(a\ge3\) 先由三层符号下降处理；有限核来自必需条件
\(2^{2a}5^v\le2J^3\)，该条件自身严格迫使 \(a\le3\)（\(J=5\)）或
\(a\le5\)（\(J=9\)）。

### 9.3 是否把第二层公式原样误用于第三层

没有。第三层先重新计算 \(N/A\)，得到带额外因子 \(A\) 的 (5.2)，再推出
(5.4)。这也是题设第三下降式的严格来源。

### 9.4 是否在证明 \(\delta>0\) 时循环使用 (5.4)

没有。先由 \(c>0\)、\(A>J^2\) 排除 \(\delta<0\)，再由偶奇性排除
\(\delta=0\)，
最后才使用正性估计 (5.7)。

### 9.5 是否遗漏 \(L_v\le J^2\) 的第二层边界

没有。它唯一为 \((a,v,J)=(3,0,9)\)，且两个真实
\(h\in\{1,2\}\) 被同一个严格大小矛盾删除。

### 9.6 是否把有限证书当作一般证明

没有。证书只核对第三层 \(L_v\le2J^3\) 的 11 行；第一、第二层及第三层
\(L_v>2J^3\) 均由无界符号论证关闭。

### 9.7 是否发现 GA2H-2 或继承公式错误

没有。本文发现的是第三层书写时必须显式保留的缩放因子 \(A\)；从原始
\(N=J+s_0r\) 重新推导后，所得 (5.4) 与题设完全一致，不构成 GA2H-2
或继承链错误。

### 9.8 是否越出本轮研究范围

没有。本文不对 \(\mathcal F_{P-}\)、\(\mathcal F_{E-}\)、
\(\varphi<a\) 或任何其他 G/Q/严格层分支作结论。

---

## 10. 最终分类与停止点

本轮得到纯终端因子层定理

\[
\boxed{
G_{\mathrm{prim}},\quad
\gamma=1,\quad
\mathrm{A2},\quad
a\ge3,\quad
\varphi=a,\quad
\mathrm P_2,\quad
\sigma=+1,\quad
J\in\{5,9\}
\Longrightarrow\text{无候选}.
}
\]

不存在有限例外、无界递推残余、合法原题解或继承错误。因此唯一分类为

\[
\boxed{
\mathrm{GFP\text{-}1}:
\quad
\mathcal F_+\text{ 完整关闭}.
}
\]

本文到此停止。
