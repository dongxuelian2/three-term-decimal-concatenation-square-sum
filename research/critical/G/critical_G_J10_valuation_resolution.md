# 三项十进制拼接平方和问题：临界 \(G\) 模板 \(J=10\) 赋值方程终结报告

## 1. GB2 的唯一剩余条件

本文只处理 `critical_G_J10_boundary_campaign.md` 的 GB2 剩余条件

\[
\boxed{
v_2(1+7\cdot25^\varphi)=3\varphi,
\qquad \varphi\in\mathbb Z_{\ge2}.
}
\tag{V0}
\]

按本轮约定，暂时接受 T1–T18、K5、CG、E4、GT4 和
GB-I.1–GB-III.3，不作整个项目的统一独立审计。特别地，继承：

\[
\mathrm{B10\!-\!1}\text{ 无解},
\qquad
\mathrm{B10\!-\!3}\text{ 无解},
\]

而 B10–2 只有在 (V0) 存在指数解时才需继续处理
\((a_2,a_3)\) 二次曲线。

本文证明：

\[
\boxed{\text{方程 (V0) 无解}.}
\tag{1.1}
\]

最终分类为

\[
\boxed{\mathrm{VA1}}.
\]

因此

\[
\boxed{\mathrm G_{10}\text{ 全部关闭}.}
\tag{1.2}
\]

全文不研究 \((a_2,a_3)\)、\(J=1,\ldots,9\)、O 或 Q。

---

## 2. 偶数指数排除

### 核心引理 VA-I.1

若 \(\varphi\) 为偶数，则

\[
\boxed{
v_2(1+7\cdot25^\varphi)=3.
}
\tag{2.1}
\]

证明：因为

\[
25\equiv9\pmod{16},
\]

偶数 \(\varphi\) 满足

\[
25^\varphi\equiv1\pmod{16}.
\]

于是

\[
1+7\cdot25^\varphi\equiv8\pmod{16},
\]

故其二进赋值恰为 \(3\)。当 \(\varphi\ge2\) 时，
\(3\ne3\varphi\)，所以 (V0) 的任何解都必须为奇数。

---

## 3. 二进 Hensel 根

### 3.1 二进对数与指数

在 \(\mathbb Z_2\) 中，对 \(u\in4\mathbb Z_2\) 定义

\[
\log_2(1+u)=
\sum_{j\ge1}\frac{(-1)^{j+1}u^j}{j},
\]

对 \(z\in4\mathbb Z_2\) 定义

\[
\exp_2(z)=
\sum_{j\ge0}\frac{z^j}{j!}.
\]

二者在 \(1+4\mathbb Z_2\) 与 \(4\mathbb Z_2\) 之间互逆。因为

\[
25=1+24\in1+8\mathbb Z_2,
\qquad
v_2(\log_2 25)=v_2(24)=3,
\tag{3.1}
\]

故对每个 \(x\in\mathbb Z_2\) 可严格定义

\[
\boxed{
25^x=\exp_2(x\log_2 25).
}
\tag{3.2}
\]

它在普通非负整数 \(x\) 上与通常整数幂相同，并满足

\[
25^{x+y}=25^x25^y
\qquad(x,y\in\mathbb Z_2).
\tag{3.3}
\]

主动核对题面中特别指出的目标：

\[
-\frac17-1=-\frac87\in8\mathbb Z_2,
\]

所以

\[
\boxed{-\frac17\in1+8\mathbb Z_2.}
\tag{3.4}
\]

其二进对数确实定义，并且

\[
v_2\!\left(\log_2\!\left(-\frac17\right)\right)=3.
\tag{3.5}
\]

### 3.2 唯一根

### 核心引理 VA-I.2

定义

\[
\boxed{
\alpha=
\frac{\log_2(-1/7)}{\log_2 25}.
}
\tag{3.6}
\]

由 (3.1)、(3.5)，分子分母的二进赋值都为 \(3\)，故

\[
\alpha\in\mathbb Z_2^\times.
\]

并且

\[
25^\alpha
=\exp_2(\log_2(-1/7))
=-\frac17.
\tag{3.7}
\]

若 \(\beta\in\mathbb Z_2\) 也满足 \(25^\beta=-1/7\)，则取二进对数得

\[
(\beta-\alpha)\log_2 25=0.
\]

因 \(\log_2 25\ne0\)，必有 \(\beta=\alpha\)。所以

\[
\boxed{
\alpha\in\mathbb Z_2
\text{ 是 }25^\alpha=-1/7\text{ 的唯一根}.
}
\tag{3.8}
\]

由 (3.6) 在除以 \(8\) 后模 \(2\) 比较两个对数的首项，还得到

\[
\boxed{\alpha\equiv1\pmod2.}
\tag{3.9}
\]

---

## 4. 精确赋值公式

对 \(y\in\mathbb Z_2\setminus\{0\}\)，令

\[
z=y\log_2 25.
\]

则 \(v_2(z)=3+v_2(y)\ge3\)，而二进指数在该收敛域满足

\[
v_2(\exp_2 z-1)=v_2(z).
\]

因此

\[
\boxed{
v_2(25^y-1)=3+v_2(y)
\qquad
(y\in\mathbb Z_2\setminus\{0\}).
}
\tag{4.1}
\]

利用 \(7\cdot25^\alpha=-1\)，对任意
\(x\in\mathbb Z_2\) 有

\[
\begin{aligned}
1+7\cdot25^x
&=1+7\cdot25^\alpha25^{x-\alpha}\\
&=1-25^{x-\alpha}.
\end{aligned}
\]

于是得到题设所需的精确公式：

\[
\boxed{
v_2(1+7\cdot25^x)
=3+v_2(x-\alpha).
}
\tag{V1}
\]

这里对 \(x\ne\alpha\) 按普通有限赋值理解；当 \(x=\alpha\) 时两边都按
\(+\infty\) 理解。特别地，(V1) 对所有普通奇整数 \(x\) 成立，
没有遗漏常数，也没有例外分支。

### 4.1 可执行的 Hensel 递推

对 \(s\ge0\)，定义唯一整数

\[
r_s\in[0,2^s),
\qquad
\alpha\equiv r_s\pmod{2^s}.
\tag{4.2}
\]

取 \(r_0=0\)。由 (4.1)，

\[
25^{2^s}\equiv1+2^{s+3}\pmod{2^{s+4}}.
\tag{4.3}
\]

设

\[
F(X)=1+7\cdot25^X.
\]

因为 \(F(r_s)\equiv0\pmod{2^{s+3}}\)，其模 \(2^{s+4}\)
剩余只能是 \(0\) 或 \(2^{s+3}\)。又由 (4.3)，

\[
F(r_s+2^s)
\equiv
F(r_s)+2^{s+3}
\pmod{2^{s+4}}.
\tag{4.4}
\]

所以两个候选 \(r_s\) 与 \(r_s+2^s\) 中恰有一个提升到下一层。
定义

\[
\boxed{
\varepsilon_s
=
\frac{
F(r_s)\bmod 2^{s+4}
}{2^{s+3}}
\in\{0,1\}.
}
\tag{4.5}
\]

则

\[
\boxed{
r_{s+1}=r_s+\varepsilon_s2^s.
}
\tag{4.6}
\]

式 (4.5) 只需计算

\[
7\cdot25^{r_s}+1\pmod{2^{s+4}},
\]

完全符合只用模 \(2^{s+4}\) 整数运算决定下一位的要求。

初始提升如下：

| \(s\) | \(r_s\) | \(F(r_s)\bmod2^{s+4}\) | \(\varepsilon_s\) | \(r_{s+1}\) |
|---:|---:|---:|---:|---:|
| 0 | 0 | 8 | 1 | 1 |
| 1 | 1 | 16 | 1 | 3 |
| 2 | 3 | 0 | 0 | 3 |
| 3 | 3 | 64 | 1 | 11 |
| 4 | 11 | 128 | 1 | 27 |
| 5 | 27 | 0 | 0 | 27 |

故严格恢复

\[
\boxed{\alpha\equiv1\pmod2,}
\]

\[
\boxed{\alpha\equiv3\pmod8,}
\]

\[
\boxed{\alpha\equiv27\pmod{64}.}
\tag{4.7}
\]

若 \(\varphi\) 满足 (V0)，则它是奇数且 \(\varphi\ge3\)。由 (V1)，

\[
v_2(\varphi-\alpha)=3\varphi-3\ge6,
\]

所以

\[
\boxed{\varphi\equiv27\pmod{64}.}
\tag{4.8}
\]

---

## 5. 固定点方程

令

\[
N=3\varphi-3.
\]

由 (V1)，(V0) 精确等价于

\[
\boxed{
v_2(\varphi-\alpha)=N.
}
\tag{V2}
\]

这里必须区分“至少 \(N\)”和“恰为 \(N\)”：

\[
v_2(\varphi-\alpha)=N
\]

当且仅当

\[
\varphi\equiv r_N\pmod{2^N}
\tag{5.1}
\]

且

\[
\varphi\not\equiv r_{N+1}\pmod{2^{N+1}}.
\tag{5.2}
\]

所以题面单独写出的

\[
\varphi\equiv r_N\pmod{2^N}
\]

只表达 \(v_2(\varphi-\alpha)\ge N\)，并不单独等价于 (V2)。

对 \(\varphi\ge2\)，有

\[
0<\varphi<2^{3\varphi-3}=2^N.
\tag{5.3}
\]

又 \(0\le r_N<2^N\)，故 (5.1) 强迫

\[
\boxed{\varphi=r_N.}
\tag{V4}
\]

若 \(r_N=\varphi\)，则

\[
r_{N+1}=\varphi+\varepsilon_N2^N.
\]

因此 (5.2) 精确等价于

\[
\varepsilon_N=1.
\]

最终的完整固定点版本是

\[
\boxed{
\text{(V0)}
\iff
\left[
\varphi=r_{3\varphi-3}
\ \text{且}\
\varepsilon_{3\varphi-3}=1
\right].
}
\tag{5.4}
\]

这保留了“恰等于 \(3\varphi\)”所需的下一位条件。

---

## 6. 初等闭合尝试

### 6.1 Hensel 位增长

递推 (4.5)–(4.6) 给出了 \(\alpha\) 的全部二进位，但从该递推本身
无法推出统一的非零位间隔上界。

可以初等证明 \(\alpha\) 不是普通非负整数：否则
\(25^\alpha=-1/7\) 会成为不可能的有理数等式。因此
\(\alpha\) 的二进展开含无穷多个非零位。然而，“非零位无穷多”不能排除
任意长的零位间隔；而固定点

\[
r_{3\varphi-3}=\varphi
\]

要求排除的正是一个长度与 \(\varphi\) 成线性关系的零位间隔。
本文没有把有限位计算或“位看起来随机”当作该统一间隔命题的证明。

### 6.2 模周期自反馈

由 (4.1)，对普通正整数 \(h\) 有

\[
v_2(25^h-1)=3+v_2(h).
\]

故对 \(M\ge3\)，

\[
\boxed{
\operatorname{ord}_{2^M}(25)=2^{M-3}.
}
\tag{6.1}
\]

若 (V0) 成立，则

\[
25^\varphi\equiv-7^{-1}\pmod{2^{3\varphi}}.
\]

指数模 \(\operatorname{ord}_{2^{3\varphi}}(25)=2^{3\varphi-3}\)
的唯一性恰给出

\[
\varphi\equiv r_{3\varphi-3}\pmod{2^{3\varphi-3}},
\]

即第 5 节的同一个固定点条件。奇偶性给出偶数指数排除，固定低模继续给出
\(\varphi\equiv27\pmod{64}\)，但模 \(3\)、模 \(8\) 与指数周期之间
没有再产生独立矛盾。

### 6.3 二项展开

题面给出的恒等式正确：

\[
\frac{1+7\cdot25^\varphi}{8}
=
1+21\varphi+
\sum_{j\ge2}
7\cdot3^j2^{3j-3}\binom{\varphi}{j}.
\tag{6.2}
\]

但高赋值来自这些项的同步消去。若要从 (6.2) 证明

\[
v_2(1+7\cdot25^\varphi)
\le C\log\varphi+C_0,
\]

就必须给出整数 \(\varphi\) 对二进根 \(\alpha\) 的有效逼近下界；
由 (V1)，这与控制 \(v_2(\varphi-\alpha)\) 是同一个问题。
本文没有从有限截断或逐项最小赋值中伪造这样的全局上界。

因此阶段 II 的初等机制没有单独关闭 (V0)，需要进入显式二进线性形式。

---

## 7. 二进线性形式与显式界

### 7.1 线性形式及非零性

定义二进线性形式

\[
\boxed{
\Lambda_\varphi
=
\varphi\log_2 25
-\log_2(-1/7).
}
\tag{7.1}
\]

两个二进对数均定义，因为

\[
25\in1+8\mathbb Z_2,
\qquad
-1/7\in1+8\mathbb Z_2.
\]

又

\[
\exp_2(\Lambda_\varphi)
=-7\cdot25^\varphi,
\]

故

\[
\exp_2(\Lambda_\varphi)-1
=-(1+7\cdot25^\varphi).
\tag{7.2}
\]

若 \(\Lambda_\varphi=0\)，则

\[
-7\cdot25^\varphi=1
\]

成为 \(\mathbb Q\) 中的等式，显然不可能。因此

\[
\boxed{\Lambda_\varphi\ne0.}
\tag{7.3}
\]

这里的 \(\log_2\) 是二进对数；下文定理常数中的
\(\log\) 则是代数数高度所使用的自然实对数，二者没有混淆。

### 7.2 使用的显式定理

使用 Bugeaud–Laurent，
*Minoration effective de la distance \(p\)-adique entre puissances de
nombres algébriques*，J. Number Theory 61 (1996), 311–342，
Corollaire 1 du Théorème 3，
[DOI: 10.1006/jnth.1996.0152](https://doi.org/10.1006/jnth.1996.0152)。

其在本文所需的形式如下。设 \(\eta_1,\eta_2\) 是乘法独立的代数数，

\[
v_p(\eta_1)=v_p(\eta_2)=0,
\]

\(b_1,b_2\) 为正整数。设 \(f\) 是
\(\mathbb Q_p(\eta_1,\eta_2)/\mathbb Q_p\) 的剩余次数，并按原文定义

\[
D=\frac{[\mathbb Q(\eta_1,\eta_2):\mathbb Q]}{f}.
\]

取 \(A_i>1\) 满足

\[
\log A_i>
\max\{h(\eta_i),\log p/D\}.
\]

令

\[
b'
=
\frac{b_1}{D\log A_2}
+
\frac{b_2}{D\log A_1},
\]

\[
\mathcal B
=
\max\left\{
\log b'+\log\log p+0.4,\,
10,\,
\frac{10\log p}{D}
\right\}.
\]

并令非零线性形式

\[
\Delta=\eta_1^{b_1}-\eta_2^{b_2}.
\]

则

\[
\boxed{
v_p(\Delta)
\le
\frac{
24p(p^f-1)D^4
}{
(p-1)(\log p)^4
}
\mathcal B^2
(\log A_1)(\log A_2).
}
\tag{7.4}
\]

### 7.3 参数逐项代入

取

\[
p=2,\qquad
\eta_1=25,\qquad
\eta_2=-1/7,\qquad
b_1=\varphi,\qquad
b_2=1.
\tag{7.5}
\]

两数都是二进单位。它们乘法独立：若

\[
25^u(-1/7)^v=1
\qquad(u,v\in\mathbb Z),
\]

比较 \(5\)-进与 \(7\)-进赋值即得 \(u=v=0\)。

数域为 \(\mathbb Q\)，故

\[
f=D=1.
\]

代数数的次数均为 \(1\)，高度为

\[
h(25)=\log25,\qquad
h(-1/7)=\log7.
\]

为避免高度条件中的严格端点，直接取

\[
A_1=26,\qquad A_2=8.
\tag{7.6}
\]

于是

\[
b'=\frac{\varphi}{\log8}+\frac1{\log26}<\varphi
\qquad(\varphi\ge2),
\tag{7.7}
\]

因为 \(\log26>\log8>2\)。

此时

\[
\Delta=25^\varphi+\frac17,
\qquad
v_2(\Delta)=v_2(1+7\cdot25^\varphi),
\]

因为 \(7\) 是二进单位。故式 (7.4) 给出

\[
3\varphi
\le
K\mathcal B^2,
\tag{7.8}
\]

其中

\[
K=
\frac{48(\log26)(\log8)}{(\log2)^4},
\tag{7.9}
\]

\[
\mathcal B
=
\max\left\{
\log b'+\log\log2+0.4,\,
10,\,
10\log2
\right\}.
\tag{7.10}
\]

### 7.4 显式上界 \(\varphi<60000\)

以下保守实对数界均可由

\[
\log\frac{1+y}{1-y}
=
2\sum_{j=0}^{m}\frac{y^{2j+1}}{2j+1}
+R_m,
\qquad
0<R_m<
\frac{2y^{2m+3}}{(2m+3)(1-y^2)}
\]

作有理区间运算直接验证：

\[
0.69<\log2<0.6932,
\]

\[
\log8<2.08,\qquad
\log26<3.26,
\]

\[
\log\log2+0.4<0.04,
\qquad
\log60000<11.1.
\tag{7.11}
\]

因此

\[
K
<
\frac{48\cdot3.26\cdot2.08}{0.69^4}
<
1440.
\tag{7.12}
\]

若 \(\varphi\ge60000\)，由 (7.7)、(7.10)、(7.11) 得

\[
\mathcal B<\log\varphi+0.04.
\tag{7.13}
\]

函数

\[
x\longmapsto
\frac{x}{(\log x+0.04)^2}
\]

在 \(x\ge60000\) 上严格递增，因为其导数符号为
\(\log x+0.04-2>0\)。而

\[
1440(11.14)^2
=178703.424
<180000
=3\cdot60000.
\tag{7.14}
\]

所以对所有 \(\varphi\ge60000\)，

\[
K(\log\varphi+0.04)^2
<
3\varphi,
\]

与 (7.8)、(7.13) 矛盾。故任何 (V0) 解都必须满足

\[
\boxed{
2\le\varphi\le59999.
}
\tag{7.15}
\]

这是来自显式定理常数的严格有效上界，不是经验截断。

---

## 8. 有限验证

### 8.1 完整覆盖

第 2 节排除所有偶数指数；第 4 节证明任何奇数指数解必须满足

\[
\varphi\equiv27\pmod{64}.
\]

结合 (7.15)，只需检查

\[
\varphi=27,91,\ldots,59995,
\]

共

\[
\boxed{938}
\]

个指数。

对每个指数令

\[
z_\varphi
=
(7\cdot25^\varphi+1)
\bmod 2^{3\varphi+1},
\qquad
0\le z_\varphi<2^{3\varphi+1}.
\tag{8.1}
\]

则

\[
v_2(1+7\cdot25^\varphi)=3\varphi
\]

当且仅当

\[
\boxed{z_\varphi=2^{3\varphi}.}
\tag{8.2}
\]

式 (8.2) 同时检查了“至少”和“恰好”：若赋值更大，
则 \(z_\varphi=0\)；若赋值更小，则其最低非零位低于
\(3\varphi\)。

### 8.2 完整代码

```python
#!/usr/bin/env python3
import hashlib

BOUND = 59_999
CHUNK = 128

candidates = list(range(27, BOUND + 1, 64))
assert len(candidates) == 938
assert candidates[0] == 27
assert candidates[-1] == 59_995

master = hashlib.sha256()
hits = []
high = []
histogram = {}
chunk_rows = []

for start in range(0, len(candidates), CHUNK):
    block = candidates[start:start + CHUNK]
    chunk_hash = hashlib.sha256()

    for phi in block:
        bits = 3 * phi + 1
        modulus = 1 << bits

        # 只计算题设要求的精确模幂，不构造 25**phi。
        z = (7 * pow(25, phi, modulus) + 1) % modulus

        # 规范记录格式：
        # ASCII 行 "phi:bits:lowercase_hex_residue\n"。
        record = f"{phi}:{bits}:{z:x}\n".encode("ascii")
        chunk_hash.update(record)
        master.update(record)

        if z == 0:
            # 此时只能从当前模数得知赋值 >= bits。
            # 本次完整运行中 high 为空。
            high.append(phi)
            continue

        valuation = (z & -z).bit_length() - 1
        histogram[valuation] = histogram.get(valuation, 0) + 1

        exact_hit_by_residue = (z == (1 << (3 * phi)))
        exact_hit_by_valuation = (valuation == 3 * phi)
        assert exact_hit_by_residue == exact_hit_by_valuation

        if exact_hit_by_residue:
            hits.append(phi)

    chunk_rows.append(
        (
            start,
            start + len(block) - 1,
            block[0],
            block[-1],
            len(block),
            chunk_hash.hexdigest(),
        )
    )

print("bound", BOUND)
print("candidate_count", len(candidates))
print("first_last", candidates[0], candidates[-1])
for row in chunk_rows:
    print("chunk", *row)
print("master_sha256", master.hexdigest())
print("high", high)
print("histogram", sorted(histogram.items()))
print("hits", hits)
```

### 8.3 分片、校验和与输出

每个分片含至多 \(128\) 个指数。校验和按代码中的规范 ASCII
记录逐行计算。

| 候选索引 | \(\varphi\) 范围 | 数量 | SHA-256 |
|---:|---:|---:|---|
| 0–127 | 27–8155 | 128 | `843a2eeb96b54c9e05323f3626c274d99247cb377987b09ac6d5519230b965f0` |
| 128–255 | 8219–16347 | 128 | `6b544280544d010c59aa517f5771739e1d62ed6ded5bbc45887da933973a4481` |
| 256–383 | 16411–24539 | 128 | `c52fa53153ee0a39ddea5a0af36636446d4befa50b216b3b3641a6dcd085e09c` |
| 384–511 | 24603–32731 | 128 | `a322d8e5187cb71b03463abd29f728954b706a760dea03819c1ff0a5ca350924` |
| 512–639 | 32795–40923 | 128 | `e307158f97069c227c0b240bb9a8bbbc14ac4766427511f6d938505630d9e8dd` |
| 640–767 | 40987–49115 | 128 | `23beaf1fad1ffc2e757fdd0b4c89ed2bfd52ba18bddb6310e00d3791cb25abf3` |
| 768–895 | 49179–57307 | 128 | `40323887cc91c276a7da693b3b9942d0137213d801290db54d01832c76a543fd` |
| 896–937 | 57371–59995 | 42 | `e46556ef7ad4095d97895715c9cb767a29f6473652ed15d05c867ba4cc77e0bc` |

全体规范记录的校验和为

```text
774d1c7d80da1039c14791a2a4ceb8d9d615e6b481a1310a9e326f9bf3c4af0c
```

程序输出：

```text
candidate_count 938
first_last 27 59995
high []
histogram [(9, 469), (10, 235), (11, 117), (12, 58),
           (13, 29), (14, 15), (15, 8), (16, 3),
           (17, 2), (18, 1), (21, 1)]
hits []
```

`high []` 表示没有候选在模 \(2^{3\varphi+1}\) 下变成 \(0\)，
所以表中记录的全部赋值都是精确值，不只是下界。

因此界内没有任何 (V0) 解。结合第 7 节的严格全局上界，

\[
\boxed{
v_2(1+7\cdot25^\varphi)=3\varphi,
\quad \varphi\ge2
\quad\text{无解}.
}
\tag{8.3}
\]

---

## 9. 最终分类 VA1–VA6

### 9.1 分类

本轮达到

\[
\boxed{
\mathrm{VA1}:\quad\text{指数方程无解}.
}
\]

分类依据是：

1. 初等部分严格排除偶数 \(\varphi\)，并把奇数候选压到唯一
   Hensel 固定点；
2. Bugeaud–Laurent 的显式二进线性形式界给出
   \(\varphi\le59999\)；
3. 在该严格界内，所有可能解进一步只占
   \(\varphi\equiv27\pmod{64}\) 的 \(938\) 个指数；
4. 精确模 \(2^{3\varphi+1}\) 验证无命中。

因此不是：

- VA2：没有指数解可列；
- VA3：有限验证已经完成；
- VA4：不只得到更强同余；
- VA5：显式定理、常数、参数和数值上界均已落实；
- VA6：已完成全局关闭。

### 9.2 主动审计

1. **\(-1/7\) 的定义域：**
   \(-1/7=1-8/7\in1+8\mathbb Z_2\)，二进对数确实定义。
2. **两种对数：**
   \(\log_2\) 始终表示二进对数；显式定理中的
   \(\log A_i\) 是自然实对数和高度参数。
3. **\(v_2(25-1)\)：**
   全文使用 \(v_2(24)=3\)，它正是 (V1) 中常数 \(3\) 的来源。
4. **偶数指数：**
   第 2 节独立、完整排除。
5. **“至少”与“恰好”：**
   固定点中保留 \(\varepsilon_{3\varphi-3}=1\)；
   有限验证使用模 \(2^{3\varphi+1}\)。
6. **Hensel 位观察：**
   没有从有限位样本推断随机性或统一间隔。
7. **显式性：**
   使用的是带完整常数的 Bugeaud–Laurent 显式界，不是
   “由 Baker 理论”或非有效有限性。
8. **有限搜索合法性：**
   只在证明 \(\varphi\le59999\) 后执行，并只用必要同余缩减。
9. **指数候选与原题解：**
   本轮没有指数候选；即使有，也只会是 B10–2 指数候选，
   不能自动成为原题解。

---

## 10. 对 \(\mathrm G_{10}\) 的影响

GB2 已证明

\[
\mathrm{B10\!-\!1}\text{ 无解},
\qquad
\mathrm{B10\!-\!3}\text{ 无解}.
\]

唯一剩余 B10–2 的先决条件正是 (V0)。第 8 节证明 (V0) 无解，
所以 B10–2 也无指数候选：

\[
\boxed{\mathrm{B10\!-\!2}\text{ 无解}.}
\]

于是三个 \(J=10\) 边界子室全部关闭：

\[
\boxed{
\mathrm G_{10}\text{ 无解}.
}
\]

这只关闭临界 \(G\) 模板的 \(J=10\) 状态；本文不对
\(J=1,\ldots,9\)、O、Q 或原题全局状态作任何额外结论。
