Summary: The negative-branch tail subsystem has an exact ceiling normal form, at most one candidate for each t>=1, at most two for t=0, and admits unbounded t and a.

All statements below are LOCAL_PROOF from the GC2B-4 frontier.

Let
\[
L=\log_2 10,\qquad c=3L-1,
\qquad y(a,t)=ca-L(t+4).
\]
Unique factorization gives \(L\notin\mathbb Q\), while
\[
3<L<10/3.
\]
The exact tail inequality
\[
10^{3a-4-t}\le2^{a+R}<10^{3a-3-t}
\]
is equivalent, for integral \(R\), to
\[
\boxed{y(a,t)<R<y(a,t)+L.}
\]
Neither endpoint can be integral. In particular, equality at the original lower endpoint is impossible.

Every tail solution satisfies
\[
\boxed{5a<R<9a.}
\]

The condition \(v_2(R)=t\) is
\[
R\equiv2^t\pmod{2^{t+1}}.
\]
The parity condition \(F+R\) odd is equivalent to
\[
t=0\Rightarrow a\text{ odd},\qquad
t\ge1\Rightarrow a\equiv t\pmod2.
\]

Put
\[
M_t=2^{t+1},\qquad b_t=2^t,
\]
and let
\[
r_t=b_t+M_t\left\lceil\frac{y(a,t)-b_t}{M_t}\right\rceil.
\]
For \(t\ge1\), since \(M_t\ge4>L\), there is at most one possible \(R\). The exact criterion is
\[
a\ge t+4,\qquad a\equiv t\pmod2,\qquad
R=r_t<y(a,t)+L.
\]
For \(t=0\), admissibility requires \(a\ge5\) odd, and the only possibilities are
\[
R=r_0,\qquad
R=r_0+2\ \text{if }r_0+2<y(a,0)+L.
\]

Equivalently, writing
\[
R=2^t+2^{t+1}h,\qquad h\ge0,
\]
all subsystem solutions are parametrized bijectively by
\[
\boxed{
0<ca-L(t+3)-2^t-2^{t+1}h<L
}
\]
together with
\[
a\ge t+4,\qquad
a\equiv
\begin{cases}
1\pmod2,&t=0,\\
t\pmod2,&t\ge1.
\end{cases}
\]

For each fixed \(t\), restricting \(a\) to the required parity class turns the boxed condition into an irrational rotation modulo \(2^{t+1}\). Density of irrational rotations proves that every fixed \(t\) occurs for infinitely many \(a\). Thus this subsystem alone gives no absolute bound on \(t\) or \(a\).

The same density argument shows that even for fixed \(t=1\), admissibility is not periodic in \(a\) modulo any fixed integer. Exact valuation also intrinsically uses the growing modulus \(2^{t+1}\). Hence this subsystem has no exact fixed-modulus residue description independent of \(a\).

Boundary audit:
- \(a=4\) is empty by parity.
- \(t=0\) requires \(a\) odd.
- \(t=1\) requires \(a\) odd.
- The endpoint \(t=a-4\) occurs exactly at
\[
(a,t,R)=(5,1,30),(6,2,36),(7,3,40),(8,4,48).
\]

Worker verification: VERDICT: CORRECT.