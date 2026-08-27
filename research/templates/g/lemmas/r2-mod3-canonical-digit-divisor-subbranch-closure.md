Summary: A uniform modulo-3 argument closes explicit infinite subbranches in all four quotient rows and both recovery signs.

Classification: BRANCH_CLOSURE. Independent worker verification: VERDICT: CORRECT.

Let
\[
\delta=a_3,\qquad d=2^a,\qquad h=2^{2a-2},
\]
and retain
\[
D=(2^Ra_1)^2+a_2^2,\qquad
H_1=a_1\,10^R+10a_2,\qquad
H_1\mid dS.
\]

First,
\[
\boxed{3\mid D\Longrightarrow3\mid e}
\]
for either recovery sign. If \(3\mid D\), the two squares in \(D\) force
\[
3\mid a_1,\qquad3\mid a_2.
\]
Hence \(3\mid H_1\), and \(H_1\mid dS\) with \(3\nmid d\) gives \(3\mid S\).

For \(L_+\),
\[
S-e=mM,\qquad S+e=(hm-1)N,\qquad D=MN.
\]
For \(L_-\),
\[
S-e=(hm-1)M,\qquad S+e=mN,\qquad D=MN.
\]
If \(3\mid D\), one of \(M,N\) is divisible by \(3\); the corresponding reconstruction identity then gives \(3\mid e\). No coprimality between \(M\) and \(N\) is used.

Since \(h\equiv1\pmod3\), the recovered factors satisfy
\[
\begin{array}{c|cc}
 &\text{first factor}&\text{second factor}\\ \hline
L_+&m\delta+e&(m-1)\delta+e\\
L_-&m\delta-e&(m-1)\delta-e
\end{array}
\pmod3.
\]
When \(3\nmid e\delta\), requiring both factors to be nonzero gives
\[
\boxed{
\begin{array}{c|cc}
m\bmod3&L_+:\ e\delta^{-1}&L_-:\ e\delta^{-1}\\ \hline
0&2&1\\
1&1&2\\
2&\text{impossible}&\text{impossible}
\end{array}
\pmod3.
}
\]

Therefore, for both signs,
\[
\boxed{m\equiv2\pmod3,\qquad3\nmid e\delta}
\]
is impossible. The exact open complements are
\[
\begin{aligned}
\mathcal C_+
={}&\{3\mid e\}\cup\{3\mid\delta\}\\
&{}\cup
\{3\nmid e\delta,\ (m,e\delta^{-1})\equiv(0,2),(1,1)\pmod3\},
\\
\mathcal C_-
={}&\{3\mid e\}\cup\{3\mid\delta\}\\
&{}\cup
\{3\nmid e\delta,\ (m,e\delta^{-1})\equiv(0,1),(1,2)\pmod3\}.
\end{aligned}
\]

Combining this with the verified sign-specific modulo-\(40\) table closes
\[
\boxed{
\begin{array}{c|c|c}
a\bmod2&q\bmod5&m\bmod120\\ \hline
0&2&113\\
0&-2&41\\
1&2&17\\
1&-2&89
\end{array}
\qquad\text{whenever }3\nmid e\delta.
}
\]

The result is uniform in the exact tail states, including \(t=0,1,a-4\), and retains shared-factor cases. It is a strict infinite-subbranch closure, not a proof of the full negative branch.

Authority classes:
- PROJECT_THEOREM: `PR6`, `SD6`, `GCU-2`, `GC2B-4`.
- LOCAL_PROOF: the modulo-\(3\) implication, factor tables, CRT combination, and subbranch closure.