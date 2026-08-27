# 临界 \(G\) 本原 A2 低 \(\varphi\) 任意深度统一多块终端报告

> 日期：2026-08-07  
> 适用范围：\(G_{\mathrm{prim}},\gamma=1,\mathrm{A2},a\ge3,1\le\varphi<a,\sigma\in\{+1,-1\}\)。  
> 最终分类：**GALMB-3（带精确计数修正）**。

## 0. 裁决

令

\[
\Delta=a-\varphi\ge1,\qquad
M=2^{2a},\qquad C=5^{2\varphi},\qquad
\Lambda=5^{3\Delta},\qquad B=MC.
\]

尾窗和终端窗统一为

\[
\mathcal H(a)=
\{h\ge0:2^{2a-2}\le5^{h+1},\ 5^h<2^{2a-1}\},
\]

\[
h\in\mathcal H(a),\qquad
\delta=\Delta+h,\qquad e=2a+\delta,\qquad
J\in\{1,\ldots,9\}.
\]

本轮严格证明了以下统一结论。

1. 对两个符号和任意五进深度，模 \(\Lambda\) 的 Möbius involution 都可按完整
   \(C\)-块递归，最后接一个模 \(R\mid C\) 的末块反射；每个输入块唯一决定输出块，
   没有逐位 Hensel 输出树。
2. 每个允许块状态都唯一恢复
   \((q_0,r,s_0,N_0)\) 及一条仿射族。采用最小正二进代表后，全部状态统一为
   \[
   2^\delta10^\mu=z r-\mathcal D^\sharp,\qquad
   z\ge1,\qquad 0<\mathcal D^\sharp<r,\qquad
   \gcd(\mathcal D^\sharp,r)=1.
   \]
3. 每个固定块输入状态要么为空，要么只剩一条完整有限指数同余段；没有对
   \(\mu\) 作有限采样。
4. 统一离散对数目标为
   \[
   2^{2a+h}10^{\mu+2a+\Delta}\equiv-1\pmod r.
   \]
5. 全局关闭攻击没有关闭移动模数：商恒等于原终端因子 \(q\)，Jacobi 符号自动相容，
   也没有得到统一的 \(\operatorname{ord}_r(10)\) 下界。因此不能宣称 GALMB-1 或
   GALMB-2。

同时发现，本轮任务中要求的负根逐 \(J\) 精确状态数

\[
\#=\Lambda/5
\]

并非恒真；在一个明确的端点配置中应为 \(\Lambda/5\pm1\)。这是本轮拟议命题的
修正，不是 GALS\((-)\)-3 或 GALD1\((-)\)-3 的继承错误：旧报告使用的正是不会遗漏
此端点的 floor-sum 公式。

为避免与终端因子 \(q\) 冲突，下文用 \(\nu\) 表示完整 \(C\)-块个数。

## 1. 深度分解与符号数据

唯一写成

\[
3\Delta=\nu(2\varphi)+r_0,\qquad
\nu\in\mathbb Z_{\ge0},\qquad 0<r_0\le2\varphi,
\]

其中整除时采用正余数约定

\[
\nu=\frac{3\Delta}{2\varphi}-1,\qquad r_0=2\varphi.
\]

置

\[
R=5^{r_0};\qquad \Lambda=C^\nu R.
\]

于是

\[
\begin{array}{c|c}
\nu&\text{区域}\\ \hline
0&3\Delta\le2\varphi\quad\text{（浅区）}\\
1&2\varphi<3\Delta\le4\varphi\quad\text{（第一深带）}\\
\nu\ge2&\text{全部更深带}
\end{array}
\]

且整除端点 \(r_0=2\varphi\) 被包含而没有产生零长度末块。

### 1.1 正、负公共根

正根数据为

\[
\rho_+=1,\qquad \eta_+=0.
\]

负根数据为

\[
x=\langle2C^{-1}\rangle_M,\qquad Cx=2+Mc,
\]

\[
\rho_-=Cx-1=1+Mc,\qquad \eta_-=cx.
\]

统一记 \(\rho=\rho_\sigma,\eta=\eta_\sigma\)。直接计算给出

\[
0<\rho<B,\qquad \rho^2=1+B\eta,\qquad
\rho\equiv\sigma\pmod C.
\]

原图为

\[
G_0(X,Y)=\eta+\rho(X+Y)+BXY.
\]

写

\[
(\eta_0,\alpha_0,\beta_0,\gamma_0)
=(\eta,\rho,\rho,B),
\]

则

\[
\alpha_0\beta_0-\gamma_0\eta_0
=\rho^2-B\eta=1,
\]

\[
\alpha_0\equiv\beta_0\equiv\sigma\pmod C,\qquad
C\mid\gamma_0.
\]

## 2. 任意深度有限块递归

标准代表唯一写成

\[
\tau=\sum_{j=0}^{\nu-1}C^ju_j+C^\nu T,\qquad
\lambda=\sum_{j=0}^{\nu-1}C^jv_j+C^\nu L,
\]

其中 \(0\le u_j,v_j<C\)，\(0\le T,L<R\)。当 \(\nu=0\) 时，和为空，
\(\tau=T,\lambda=L\)。

设第 \(j\) 层图为

\[
G_j(X,Y)=\eta_j+\alpha_jX+\beta_jY+\gamma_jXY
\]

并满足

\[
\alpha_j\beta_j-\gamma_j\eta_j=1,\qquad
\alpha_j\equiv\beta_j\equiv\sigma\pmod C,\qquad
C\mid\gamma_j.
\]

### 2.1 唯一输出块

模 \(C\) 有

\[
G_j(u_j,v_j)\equiv\eta_j+\sigma(u_j+v_j)\pmod C.
\]

定义

\[
\theta_j=\langle-\sigma\eta_j\rangle_C.
\]

于是必须且只须取

\[
v_j=\langle\theta_j-u_j\rangle_C.
\]

存在唯一 \(\epsilon_j\in\{0,1\}\) 使

\[
u_j+v_j=\theta_j+\epsilon_jC.
\]

更具体地，

\[
\begin{cases}
v_j=\theta_j-u_j,\ \epsilon_j=0,&0\le u_j\le\theta_j,\\
v_j=\theta_j+C-u_j,\ \epsilon_j=1,&\theta_j<u_j<C.
\end{cases}
\]

所以每一层只有两个进位室，而没有自由输出数字。

### 2.2 下一层公式

定义

\[
\eta_{j+1}
=\frac{\eta_j+\alpha_ju_j+\beta_jv_j+\gamma_ju_jv_j}{C},
\]

\[
\alpha_{j+1}=\alpha_j+\gamma_jv_j,\qquad
\beta_{j+1}=\beta_j+\gamma_ju_j,\qquad
\gamma_{j+1}=C\gamma_j.
\]

分子被 \(C\) 整除，因为 \(v_j\) 正是上一小节的唯一解。展开得到严格恒等式

\[
\frac{G_j(u_j+CX,v_j+CY)}C=G_{j+1}(X,Y).
\]

再计算

\[
\begin{aligned}
\alpha_{j+1}\beta_{j+1}-\gamma_{j+1}\eta_{j+1}
&=(\alpha_j+\gamma_jv_j)(\beta_j+\gamma_ju_j)\\
&\quad-\gamma_j(\eta_j+\alpha_ju_j+\beta_jv_j+\gamma_ju_jv_j)\\
&=\alpha_j\beta_j-\gamma_j\eta_j=1.
\end{aligned}
\]

由于 \(C\mid\gamma_j\)，还有

\[
\alpha_{j+1}\equiv\alpha_j\equiv\sigma\pmod C,\qquad
\beta_{j+1}\equiv\beta_j\equiv\sigma\pmod C,\qquad
C\mid\gamma_{j+1}.
\]

归纳完成全部深度。

## 3. 末块反射与严格双向等价

因为 \(R\mid C\)，末层满足

\[
G_\nu(T,L)\equiv\eta_\nu+\sigma(T+L)\pmod R.
\]

定义

\[
\Theta_\nu=\langle-\sigma\eta_\nu\rangle_R,\qquad
L=\langle\Theta_\nu-T\rangle_R,
\]

以及唯一 \(\epsilon_\nu\in\{0,1\}\) 使

\[
T+L=\Theta_\nu+\epsilon_\nu R.
\]

连续使用第 2.2 节的恒等式得到

\[
G_0(\tau,\lambda)=C^\nu G_\nu(T,L).
\]

因此

\[
G_0(\tau,\lambda)\equiv0\pmod\Lambda
\iff
G_\nu(T,L)\equiv0\pmod R.
\]

向右的每一步由标准 \(C\)-进数字唯一得到；反向将各层数字代回恒等式即可。
故上述块递归与原模 \(\Lambda\) 图严格双向等价。特别地，任意深度和两个符号
都不存在逐位 Hensel 输出树。

这里的“有限块字母表”是对固定外参数的
\(\{0,\ldots,C-1\}\) 及末块 \(\{0,\ldots,R-1\}\)；输入块字总数仍随
\(\Lambda\) 增长，不能把无输出分支误写成叶节点绝对有界。

## 4. 正反矩阵与完整 involution

定义

\[
\mathcal M_j=
\begin{pmatrix}-\alpha_j&-\eta_j\\ \gamma_j&\beta_j\end{pmatrix},\qquad
\mathcal M_j^\vee=
\begin{pmatrix}-\beta_j&-\eta_j\\ \gamma_j&\alpha_j\end{pmatrix}.
\]

由单位行列式，

\[
\mathcal M_j^\vee\mathcal M_j
=
\begin{pmatrix}
\alpha_j\beta_j-\gamma_j\eta_j&0\\0&
\alpha_j\beta_j-\gamma_j\eta_j
\end{pmatrix}=I.
\]

交换 \(u_j,v_j\) 后，\(\eta_{j+1}\) 的分子不变，
\(\alpha_{j+1},\beta_{j+1}\) 恰好交换，而 \(\gamma_{j+1}\) 不变。
因此下一层反向图仍是正向图的逆。归纳到末块，所得是原 Möbius involution
的完整双向块图，而不只是单向生成器。

## 5. 根门、固定点和奇偶门

### 5.1 根门及其保持

正根门是

\[
\tau\equiv2\text{ 或 }3\pmod5.
\]

由图方程

\[
\lambda(1+B\tau)\equiv-\tau\pmod\Lambda
\]

并在模 \(5\) 下使用 \(5\mid B\)，得到
\(\lambda\equiv-\tau\pmod5\)，故 \(2,3\) 互换。

负根门是

\[
x+M\tau\equiv2\text{ 或 }3\pmod5.
\]

负根图等价于

\[
(x+M\lambda)(\rho+B\tau)\equiv x+M\tau\pmod\Lambda.
\]

模 \(5\) 有 \(\rho\equiv-1\)，故
\(x+M\lambda\equiv-(x+M\tau)\pmod5\)，根门仍被保持。
由于 \(5\mid C\)，根门只读取 \(u_0\bmod5\)；当 \(\nu=0\) 时只读取
\(T\bmod5\)。

### 5.2 固定点

正根唯一固定点为 \(\tau=0\)，被正根门删除。

负根唯一固定点为

\[
\tau_*=\langle-xM^{-1}\rangle_\Lambda,\qquad
x+M\tau_*\equiv0\pmod\Lambda,
\]

故也被负根门删除。因此根门允许的状态在施加奇偶门前全部组成非平凡二循环。

### 5.3 奇偶门和二循环端点数

终端模 \(8\) 门统一为

\[
c_\sigma+J+\tau\equiv1\pmod2,\qquad c_+=0,\quad c_-=c.
\]

因 \(C,R\) 都是奇数，

\[
\tau\equiv\sum_{j=0}^{\nu-1}u_j+T\pmod2,
\]

\[
\tau+\lambda\equiv
\sum_{j=0}^{\nu-1}(\theta_j+\epsilon_j)
+\Theta_\nu+\epsilon_\nu\pmod2.
\]

令右端为 \(S\pmod2\)。在一个二循环 \(\{\tau,\lambda\}\) 中：

- 若 \(S=1\)，两端奇偶相反，奇偶门恰保留一端；
- 若 \(S=0\)，两端奇偶相同，按 \(c_\sigma+J+\tau\) 的值保留两端或零端。

这给出了零端、一端、两端的精确块进位判别。

## 6. 状态数：正根定值与负根端点修正

### 6.1 根门计数

由于 \(\Lambda=5^{3\Delta}\)，每个模 \(5\) 剩余类在
\(0\le\tau<\Lambda\) 中恰出现 \(\Lambda/5\) 次。两个根类故恰给

\[
\frac{2\Lambda}{5}
\]

个有向状态；两个符号都成立。

### 6.2 正根奇偶计数

正根类为 \(2,3\pmod5\)。与任意指定奇偶性联立后得到两个模 \(10\) 类，
其中一个在长度为奇数的区间 \([0,\Lambda-1]\) 中多出现一次，另一个少出现一次，
恰好抵消。因此每个固定 \(J\) 精确保留

\[
\mathcal C_{+,J}=\frac\Lambda5.
\]

### 6.3 负根的精确公式

负根的两个 \(\tau\)-剩余类为

\[
\alpha_{-,d}=\langle M^{-1}(d-x)\rangle_5,\qquad d\in\{2,3\}.
\]

令目标奇偶性

\[
p_{-,J}=\langle1-c-J\rangle_2.
\]

对 \(d=2,3\)，令 \(\beta_{d,J}\in\{0,\ldots,9\}\) 是 CRT 唯一解

\[
\beta_{d,J}\equiv\alpha_{-,d}\pmod5,\qquad
\beta_{d,J}\equiv p_{-,J}\pmod2.
\]

定义

\[
F(X;\beta)=
\begin{cases}
0,&X<\beta,\\
\left\lfloor\dfrac{X-\beta}{10}\right\rfloor+1,&X\ge\beta.
\end{cases}
\]

则精确计数是

\[
\boxed{\mathcal C_{-,J}=
F(\Lambda-1;\beta_{2,J})+F(\Lambda-1;\beta_{3,J}).}
\]

写 \(K=\Lambda/5\)。化简 floor-sum 得

\[
\mathcal C_{-,J}=
\begin{cases}
K,&\{\alpha_{-,2},\alpha_{-,3}\}\ne\{0,4\},\\
K+(-1)^{p_{-,J}},&\{\alpha_{-,2},\alpha_{-,3}\}=\{0,4\}.
\end{cases}
\]

所以“负根对每个 \(J\) 恒为 \(\Lambda/5\)”是假的。范围内的反例为

\[
a=5,\quad\varphi=1,\quad\Delta=4,\quad
M=1024,\quad C=25,\quad x=82,\quad c=2,
\]

\[
\Lambda=244140625,\qquad K=48828125,\qquad
\{\alpha_{-,2},\alpha_{-,3}\}=\{0,4\}.
\]

此时 \(J=1\) 给 \(K+1=48828126\)，\(J=2\) 给
\(K-1=48828124\)。

若 \(J=1,\ldots,9\)，两个符号合计为

\[
\sum_{\sigma,J}\mathcal C_{\sigma,J}=
\begin{cases}
18\Lambda/5,&\text{非端点配置},\\
18\Lambda/5+(-1)^c,&\text{端点配置 }\{0,4\}.
\end{cases}
\]

这也说明任务中要求的总数 \(18\Lambda/5\) 不是无条件定理。

## 7. 统一终端恢复

从块字恢复 \(0\le\tau,\lambda<\Lambda\)，定义

\[
V=J\Lambda+\tau,\qquad
r=\rho+BV,\qquad
q_0=\rho+B\lambda,
\]

\[
s_0=\frac{G_0(\tau,\lambda)}\Lambda,\qquad
N_0=Jq_0+s_0.
\]

第 3 节的精确展开立即给

\[
s_0=\frac{G_\nu(T,L)}R.
\]

根门删除唯一零点，且原正整数表达式的各项非负，故 \(s_0>0\)。更直接地，

\[
q_0r=1+B\Lambda N_0.
\]

证明如下：使用 \(\rho^2=1+B\eta\) 展开左边，按
\(V=J\Lambda+\tau\) 收集，括号内恰为
\(J\Lambda q_0+G_0(\tau,\lambda)=\Lambda N_0\)。

又有

\[
JB\Lambda<r<(J+1)B\Lambda,\qquad 0<q_0<B\Lambda.
\]

令 \(R_\tau=\rho+B\tau=r-JB\Lambda\)，则

\[
0<R_\tau<B\Lambda,
\qquad q_0R_\tau=1+B\Lambda s_0.
\]

根门删除唯一的 \(s_0=0\) 状态；又由
\(q_0R_\tau<B\Lambda q_0\) 得 \(s_0<q_0\)。另一方面，
\(q_0<B\Lambda\) 与乘积恒等式给

\[
1+B\Lambda N_0=q_0r<B\Lambda r.
\]

所以

\[
0<s_0<q_0,\qquad 0<N_0<r.
\]

若 \(d\mid N_0,r\)，则由乘积恒等式 \(d\mid q_0r-B\Lambda N_0=1\)，故

\[
\gcd(N_0,r)=1.
\]

全部仿射恢复为

\[
q=q_0+B\Lambda y,\qquad
s=s_0+(\rho+B\tau)y,\qquad
N=N_0+ry,\qquad y\in\mathbb Z_{\ge0}.
\]

代回即满足原终端方程；反向对 \(q\) 作模 \(B\Lambda\) 的标准除法，所得余数必须
为 \(q_0\)，商即唯一的 \(y\)，其余两式由乘积关系和线性终端方程强制得到。
故该恢复与原终端状态严格双向。

## 8. 最小正二进代表与统一正缺陷

真实指数满足

\[
N=2^e10^\mu,\qquad e=2a+\delta,\qquad
\delta=\Delta+h,\qquad \mu\ge0.
\]

所以 \(M\mid N\)。又 \(r\equiv1\pmod M\)，故
\(y\equiv-N_0\pmod M\)。定义

\[
A^\sharp=1+\langle N_0-1\rangle_M\in\{1,\ldots,M\}.
\]

则 \(A^\sharp\equiv N_0\pmod M\)，且全部非负 \(y\) 唯一写成

\[
y=Mz-A^\sharp,\qquad z\in\mathbb Z_{\ge1}.
\]

若 \(A^\sharp<M\)，最小 \(z=1\) 给 \(y=M-A^\sharp>0\)；若
\(A^\sharp=M\)，则 \(z=1\) 恰给 \(y=0\)。

定义

\[
\mathcal D^\sharp=\frac{A^\sharp r-N_0}{M}.
\]

分子由同余关系被 \(M\) 整除。由于 \(A^\sharp\ge1\) 且
\(0<N_0<r\)，

\[
\boxed{\mathcal D^\sharp>0.}
\]

最小正代表还给出严格上界。由 \(A^\sharp\le M\) 与 \(N_0>0\)，

\[
A^\sharp r-N_0<Mr,
\]

故

\[
\boxed{0<\mathcal D^\sharp<r.}
\]

将 \(y=Mz-A^\sharp\) 代入 \(N=N_0+ry=M2^\delta10^\mu\)，得到

\[
\boxed{2^\delta10^\mu=z r-\mathcal D^\sharp,\qquad z\ge1.}
\]

反向由该式定义 \(y=Mz-A^\sharp\)，端点字典保证 \(y\ge0\)，再恢复
\(N=M2^\delta10^\mu\)。所以核心正规形与仿射终端状态严格双向。

特别地，\(\mathcal D^\sharp=0\)、\(\mathcal D^\sharp\ge r\) 和
\(r-\mathcal D^\sharp\le0\) 都不可能。

## 9. 下降坐标的规范等价

若旧坐标使用 \(A\)，并取

\[
A'=A+kM,\qquad z'=z+k,\qquad
\mathcal D'=\frac{A'r-N_0}{M}=\mathcal D+kr,
\]

则

\[
z'r-\mathcal D'=zr-\mathcal D.
\]

因此零至 \(M-1\) 代表、未约化正代表、正缺陷和有符号缺陷只是同一仿射类的
不同规范。

逐报告核对如下。

| 旧报告 | 旧坐标 | 到 \(A^\sharp\) 的变换 | 裁决 |
|---|---|---|---|
| GALS\((+)\)-3 | \(A=J+1\) | 已是最小正代表 | 严格相同 |
| GALS\((-)\)-3 | 正但可未约化的 \(A=J+\epsilon+s_*\) | 取 \(k=(A^\sharp-A)/M\)，同时 \(z^\sharp=z+k\) | 仿射等价 |
| GALD1\((+)\)-3 | \(A\in\{0,\ldots,M-1\}\) | \(A>0\) 不变；\(A=0\) 时 \(A^\sharp=M,k=1\) | 原零/负缺陷是规范选择 |
| GALD1\((-)\)-3 | 正但可未约化的 \(A=J+\epsilon+\Sigma\) | 同负浅区约化 | 仿射等价 |

四行的端点也完全一致。GALS\((+)\)-3 中
\(2\le J+1\le10<M\)，所以无需平移。对两个使用未约化正代表的负根报告，
唯一写 \(A=A^\sharp+tM\) 后，旧下端
\(z\ge\lceil A/M\rceil=t+1\) 恰变成
\(z^\sharp=z-t\ge1\)。GALD1\((+)\)-3 的唯一特殊端是旧
\(A=0,z\ge0\)；取 \(k=1\) 后变成
\(A^\sharp=M,z^\sharp=z+1\ge1\)，且
\(\mathcal D^\sharp=\mathcal D+r>0\)。

在 \(\nu=0,1\) 时，块递归分别就是旧浅区和第一深带公式；上述坐标变换后严格
退化为本轮 \((A^\sharp,\mathcal D^\sharp,z)\)。因此这里得到的是统一加强，不能把
相容恒等式伪报为继承错误。

## 10. 缺陷互素性与商恒等式

由

\[
M\mathcal D^\sharp=A^\sharp r-N_0
\]

以及 \(\gcd(N_0,r)=\gcd(M,r)=1\)，若素数同时整除
\(\mathcal D^\sharp,r\)，便会整除 \(N_0\)，矛盾。因此

\[
\gcd(\mathcal D^\sharp,r)=1.
\]

把 \(N_0=A^\sharp r-M\mathcal D^\sharp\) 代入
\(q_0r=1+B\Lambda N_0\)，得

\[
MB\Lambda\mathcal D^\sharp
=1+r(A^\sharp B\Lambda-q_0).
\]

定义

\[
\ell^\sharp=A^\sharp B\Lambda-q_0.
\]

因 \(A^\sharp\ge1\) 且 \(0<q_0<B\Lambda\)，

\[
0<\ell^\sharp<MB\Lambda,\qquad
MB\Lambda\mathcal D^\sharp=1+\ell^\sharp r.
\]

还可读出

\[
\ell^\sharp\equiv-1\pmod M,\qquad
\ell^\sharp\equiv-\sigma\pmod C,\qquad
v_2(\ell^\sharp)=v_5(\ell^\sharp)=0.
\]

这些是方便的数字信息，但不是独立关闭门：商恒等式由终端乘积恒等式与缺陷定义
互相代入即得；\(A^\sharp\) 在模 \(M\) 约化处发生锯齿跳变，故
\(\ell^\sharp\) 对块进位没有统一单调性。

## 11. 统一离散对数和完整有限指数段

核心方程模 \(r\) 给

\[
10^\mu\equiv-2^{-\delta}\mathcal D^\sharp\pmod r.
\]

由上一节

\[
\mathcal D^\sharp\equiv(MB\Lambda)^{-1}\pmod r.
\]

又

\[
MB\Lambda=M^2C\Lambda
=2^{4a}5^{2\varphi+3\Delta}
=2^{4a}5^{2a+\Delta},
\]

所以两个符号、全部深度共有

\[
\boxed{2^{2a+h}10^{\mu+2a+\Delta}\equiv-1\pmod r.}
\]

令 \(P_r=\operatorname{ord}_r(10)\)。若目标不在
\(\langle10\rangle\subseteq(\mathbb Z/r\mathbb Z)^\times\)，整个块状态删除；若在，
全部指数位于唯一类

\[
\mu\equiv\mu_0\pmod{P_r},\qquad 0\le\mu_0<P_r.
\]

对每个指数，

\[
z=\frac{\mathcal D^\sharp+2^\delta10^\mu}{r}
\]

唯一恢复。

### 11.1 精确下端

\(z\ge1\) 等价于

\[
2^\delta10^\mu\ge r-\mathcal D^\sharp.
\]

第 8 节已证 \(0<\mathcal D^\sharp<r\)，所以右端总是正整数。定义

\[
D_{\min}=r-\mathcal D^\sharp\in\{1,\ldots,r-1\},
\]

\[
\mu_{\min}=\min\{v\in\mathbb Z_{\ge0}:2^\delta10^v\ge D_{\min}\}.
\]

这与 \(z\ge1\) 严格双向，并完整保留 \(z=1\) 和 \(\mu=0\)。

### 11.2 保留严格端点的整数上端

继承大小门

\[
20\cdot10^m<194029\,\mathfrak Z^2Y,\qquad
\mathfrak Z=\frac{B\Lambda}{2},\qquad Y=10^{3a},\qquad
m=e+\mu.
\]

令

\[
H=194029\,\mathfrak Z^2Y,\qquad
Q_\mu=\left\lfloor\frac{H-1}{20\cdot10^e}\right\rfloor.
\]

若 \(Q_\mu<1\)，状态为空；否则定义纯整数上端

\[
\mu_{\max}=\max\{v\in\mathbb Z_{\ge0}:10^v\le Q_\mu\}.
\]

\(H-1\) 恰好保留了原严格不等号。

### 11.3 唯一完整指数段

若离散对数存在，定义

\[
t_{\min}=\max\left(0,
\left\lceil\frac{\mu_{\min}-\mu_0}{P_r}\right\rceil\right),
\qquad
t_{\max}=
\left\lfloor\frac{\mu_{\max}-\mu_0}{P_r}\right\rfloor.
\]

全部指数恰为

\[
\boxed{\mu=\mu_0+tP_r,\qquad
t_{\min}\le t\le t_{\max}.}
\]

若 \(t_{\min}>t_{\max}\)，状态为空。否则每个 \(\mu\) 依次唯一恢复
\(z,y,q,s,N\)。因此任意深度的每个固定块输入状态至多对应一条完整有限指数段，
而不是若干采样点。

## 12. 共轭和差的统一字典

定义

\[
\mathscr L=\lambda+\Lambda y,\qquad
q=\rho+B\mathscr L,\qquad
r=\rho+BV.
\]

于是

\[
q-r=B(\mathscr L-V),\qquad
q+r=2\rho+B(\mathscr L+V).
\]

若 \(q=r\)，则 \(\lambda\equiv\tau\pmod\Lambda\)，故来自原 involution 的固定点；
第 5.2 节已证明该点被根门删除。因此允许状态均有 \(q\ne r\)。

根门给 \(\lambda-\tau\not\equiv0\pmod5\)，故

\[
v_5(q-r)=v_5(B)=2\varphi.
\]

又 \(q,r\equiv\rho\equiv1\pmod M\)，所以

\[
v_2(q+r)=1,\qquad v_5(q+r)=0.
\]

为求差的二进赋值，写

\[
q=1+MD_L,\qquad r=1+MD_V,
\]

其中

\[
D_L=c_\sigma+C\mathscr L,\qquad
D_V=c_\sigma+CV.
\]

奇偶门恰使 \(D_V\) 为奇数。又 \(M\mid N\) 且
\(qr=1+B\Lambda N\)，故 \(qr\equiv1\pmod{M^2}\)。展开并除以 \(M\) 得

\[
D_L+D_V+MD_LD_V\equiv0\pmod M.
\]

因 \(4\mid M\)，模 \(4\) 得 \(D_L+D_V\equiv0\pmod4\)。所以
\(D_L\) 也是奇数且 \(D_L-D_V\equiv2\pmod4\)。因此

\[
\boxed{v_2(q-r)=2a+1,\qquad v_5(q-r)=2\varphi,}
\]

\[
\boxed{v_2(q+r)=1,\qquad v_5(q+r)=0.}
\]

证明没有使用 \(\nu=0,1\)，故覆盖所有更深块消去。

若 \(z\ge2\)，则 \(y=Mz-A^\sharp\ge M>J\)，从而
\(\mathscr L>V\) 且 \(q>r\)。所以 \(q<r\) 只可能出现在最小 \(z=1\)。特别地，
\(A^\sharp=M,z=1\) 给 \(y=0\)，此时 \(q<r\)。和差平方路线代回后仍只是
\(qr=1+B\Lambda N\) 的重写，没有新增独立约束。

## 13. 全局关闭攻击及失败原因

### 13.1 商 \(\mathcal Q\) 恰是 \(q\)

定义

\[
\mathcal Q=
\frac{2^{2a+h}10^{\mu+2a+\Delta}+1}{r}.
\]

注意

\[
2^{2a+h}10^{\mu+2a+\Delta}=B\Lambda N.
\]

由 \(qr=1+B\Lambda N\)，立刻得到

\[
\boxed{\mathcal Q=q.}
\]

另一方面用核心正规形与商恒等式也得

\[
\mathcal Q=MB\Lambda z-\ell^\sharp=q.
\]

所以 \(\mathcal Q\) 的二进、五进数字和大小窗口只是原终端因子的信息回代：

\[
q\equiv1\pmod M,\qquad q\equiv\sigma\pmod C,\qquad
v_2(q)=v_5(q)=0.
\]

它不是新的关闭门。

### 13.2 窗口和严格大小门

窗口

\[
JB\Lambda<r<(J+1)B\Lambda
\]

与第 11 节大小门确实使每个固定状态的指数段有限，但参数 \(a,\Delta\) 仍无绝对
上界，窗口长度仍为 \(B\Lambda\)。没有得到 GALMB-2 所需的绝对有限边界。

### 13.3 阶与固定外部素数

\(r\) 随块字移动。目前没有只从该窗口和
\(r\equiv1\pmod M, r\equiv\sigma\pmod C\) 推出

\[
\operatorname{ord}_r(10)>\mu_{\max}-\mu_{\min}
\]

的定理。故不能统一把每状态进一步压成一个指数或空集。

同样，任取固定素数 \(p\nmid10B\)，允许的 \(\tau\) 是若干模 \(10\) 等差类；当
\(\Lambda\) 增长后，这些等差类模 \(p\) 遍历全部剩余类，而
\(r=\rho+B(J\Lambda+\tau)\) 对 \(\tau\) 是可逆仿射函数。因此仅靠固定外部素数的
剩余类覆盖不能统一删除全部块字。

### 13.4 Jacobi 与高次剩余

允许状态有

\[
r\equiv1\pmod8,\qquad r\equiv\pm1\pmod5.
\]

所以

\[
\left(\frac{-1}{r}\right)=
\left(\frac2r\right)=
\left(\frac5r\right)=1
\]

（按 Jacobi 符号解释）。统一目标中的固定 \(2,5,-1\) 因子自动相容，未产生只依赖
\((a,\Delta,h)\) 的二次剩余障碍。没有发现可脱离移动块字而成立的更高次剩余障碍。

因此剩余障碍精确位于移动模数 \(r\)、目标在
\(\langle10\rangle\) 中的成员性及 \(\operatorname{ord}_r(10)\)，而不再位于五进深度。

## 14. 主动端点审计

| 项目 | 审计结果 |
|---|---|
| \(\nu=0\) | 空和约定后直接成为末块反射，等于 GALS\((\pm)\)-3 |
| \(\nu=1\) | 一个完整 \(C\)-块加末块，等于 GALD1\((\pm)\)-3 |
| \(\nu\ge2\) | 归纳式不变，覆盖全部更深带 |
| \(r_0=2\varphi\) | \(R=C\)，仍是非零末块，无整除端点漏洞 |
| 首块、中间块、末块为零 | 标准余数公式仍唯一；无除以数字步骤 |
| 任一输出块为零 | 对应 \(u_j=\theta_j\) 或末块 \(T=\Theta_\nu\)，递归正常 |
| 任一平移数字为零 | 两室在端点退化但 \(v_j=\langle-u_j\rangle_C\) 仍唯一 |
| 块固定坐标 | 只表示局部数字相同；全局固定点仍由第 5.2 节唯一确定 |
| 正、负固定点 | 均被各自根门删除 |
| 根门保持 | 第 5.1 节对两个符号直接证明 |
| 奇偶门 0/1/2 端 | 由块进位和 \(S=\tau+\lambda\pmod2\) 精确判定 |
| \(A^\sharp=M\) | \(z=1\iff y=0\)，不遗漏仿射初端 |
| \(y=0,z=1\) | 被正代表规范完整保留 |
| \(\mathcal D^\sharp=0\) | 由 \(0<N_0<r\) 排除 |
| \(\mathcal D^\sharp\ge r\) | 由 \(A^\sharp\le M\) 与 \(N_0>0\) 排除 |
| \(r-\mathcal D^\sharp\le0\) | 同上排除；实际恒有 \(1\le r-\mathcal D^\sharp\le r-1\) |
| \(\mu=0\) | 由精确整数下端和离散对数类决定，不作先验删除 |
| \(q=r\) | 只来自已删除固定点 |
| \(q<r\) | 只可能在 \(z=1\)；\(A^\sharp=M,z=1\) 确实给负差 |
| 深块和差赋值 | 第 12 节证明不依赖块数 |
| 严格大小端点 | 用 \(H-1\) 保持原严格不等号 |
| 状态计数 | 负根有端点 \(\pm1\) 修正，不能写成恒定 \(\Lambda/5\) |
| 全局关闭 | 没有把多块正规形误报为低 \(\varphi\) 无解 |

此外，对最小更深例 \(a=3,\varphi=1\)（此时 \(\nu=2\)）进行了完整
\(\tau\)-状态精确整数回归：两个符号合计核对了施加根门和九个奇偶门后的
\(56\,250\) 个有向状态，包括块输出唯一性、单位行列式、反向 involution、
末块商、\(s_0,N_0\) 区间、互素性、严格界
\(0<\mathcal D^\sharp<r\)、商恒等式及 \(z=1,2,3\) 的四个和差赋值，
均与上述符号证明一致。该回归只是审计，不是定理成立的证明来源。

## 15. 最终结果分类

本轮得到

\[
\boxed{\text{GALMB-3：任意低 }\varphi\text{、任意深度、两个符号的统一多块终端定理。}}
\]

准确内容是

\[
\boxed{
\text{有限块字母递归}
\; +\;
\text{统一正缺陷二进下降}
\; +\;
\text{每块状态唯一有限指数段}.}
\]

五进深度已完全被有限块递归吸收；开放部分只剩移动 \(r\) 的离散对数成员性和
\(\operatorname{ord}_r(10)\)。没有得到无候选、绝对有限边界或周期证书，因此不生成
独立生成器、验证器或规范证书，也不进入高 \(\varphi\) 的
\(\mathcal F_{P-}\)、B、C、\(\gamma>1\)、非本原 C2/C5、Q 或严格层。
