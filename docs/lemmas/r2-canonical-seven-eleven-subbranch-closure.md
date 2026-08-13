Summary: Canonical recovery modulo 7 and 11 closes additional explicit infinite subbranches in both recovery signs.

Classification: BRANCH_CLOSURE. Independent worker verification: VERDICT: CORRECT.

Let
\[
d=2^a,\qquad h=2^{2a-2},\qquad \delta=a_3,
\]
and retain
\[
D=(2^Ra_1)^2+a_2^2,\qquad
H_1=a_1\,10^R+10a_2,\qquad H_1\mid dS.
\]

For each \(p\in\{7,11\}\), every complete candidate of either recovery sign satisfies
\[
\boxed{p\mid D\Longrightarrow p\mid e.}
\]
Indeed, \(p\equiv3\pmod4\). Thus \(p\mid D\) forces
\[
p\mid a_1,\qquad p\mid a_2,
\]
hence \(p\mid H_1\), then \(p\mid S\). The exact sign-specific reconstruction identities and \(D=MN\) then imply \(p\mid e\), without assuming \(\gcd(M,N)=1\).

Suppose \(p\nmid e\delta\), put
\[
x_p=e\delta^{-1}\pmod p,\qquad
c_p(a)=(2h)^{-1}\pmod p.
\]
Neither recovered factor may vanish modulo \(p\). Therefore the following classes are impossible:
\[
\boxed{
\begin{aligned}
L_+:\quad&
x_p\equiv \frac m2
\quad\text{or}\quad
x_p\equiv\frac m2-c_p(a)\pmod p,\\
L_-:\quad&
x_p\equiv-\frac m2
\quad\text{or}\quad
x_p\equiv-\frac m2+c_p(a)\pmod p.
\end{aligned}
}
\]
The two forbidden classes are distinct.

The coefficients are
\[
\begin{array}{c|ccc}
a\bmod3&0&1&2\\ \hline
c_7(a)&2&4&1
\end{array}
\]
and
\[
\begin{array}{c|ccccc}
a\bmod5&0&1&2&3&4\\ \hline
c_{11}(a)&2&6&7&10&8.
\end{array}
\]

Let
\[
\mathcal F_{+,p}(m,a)
=
\left\{\frac m2,\frac m2-c_p(a)\right\},
\qquad
\mathcal F_{-,p}(m,a)
=
\left\{-\frac m2,-\frac m2+c_p(a)\right\}.
\]
The exact residual complements are
\[
\boxed{
\mathcal C_\pm^{(7,11)}
=
\mathcal C_\pm
\cap
\bigcap_{p\in\{7,11\}}
\left(
\{p\mid e\delta\}
\cup
\{e\delta^{-1}\notin\mathcal F_{\pm,p}(m,a)\}
\right).
}
\]

These closures are uniform in all four quotient rows and retain shared-factor states. They do not exhaust either complement and do not assert the existence of integral candidates in the surviving residue classes.

Authority classes:
- PROJECT_THEOREM: `PR6`, `SD6`, `GCU-2`, `GC2B-4`.
- LOCAL_PROOF: the \(p\mid D\Rightarrow p\mid e\) implication, forbidden residue classes, coefficient tables, and exact complements.