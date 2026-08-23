Summary: The positive-complement zero-root branch is impossible by a sum-of-two-squares valuation obstruction, without recovered-pair gcd assumptions.

Classification: BRANCH_CLOSURE. Worker verification: VERDICT: CORRECT.

Assume
\[
Q_3>0,\qquad w_0=0,\qquad d=2^a,\qquad
v_2(k^2-1)=2a.
\]
Put
\[
K=k^2-1,\qquad D=(2^Ra_1)^2+a_2^2.
\]
The recovery identities for either sign reduce to
\[
D=La_3^2,\qquad \mathscr R_3=La_3,\qquad
L=\frac{K}{d^2},
\]
where \(L\) is a positive odd integer.

The terminal quotient formula has
\[
k=2^AS-1,\qquad A\ge5.
\]
Hence \(v_2(k-1)=1\). Since \(v_2(K)=2a\),
\[
k+1=2^{2a-1}s
\]
for a positive odd integer \(s\). Therefore
\[
L=\frac{(k-1)(k+1)}{2^{2a}}
=s\bigl(2^{2a-2}s-1\bigr).
\]
The two factors are coprime, and
\[
2^{2a-2}s-1\equiv3\pmod4.
\]
Thus some prime \(p\equiv3\pmod4\) occurs to an odd exponent in the second factor and hence in \(L\). Consequently
\[
v_p(D)=v_p(L)+2v_p(a_3)
\]
is odd.

But \(D=(2^Ra_1)^2+a_2^2\) is a sum of two squares. For every prime
\(p\equiv3\pmod4\), its valuation in a sum of two squares is even: if
\(p\mid x^2+y^2\), the nonresiduosity of \(-1\) modulo \(p\) forces
\(p\mid x,y\), and iteration after division by \(p^2\) proves the assertion.
This contradiction closes the branch.

Both recovery signs coincide when \(w_0=0\). The proof uses neither
\[
\gcd(a_3,D)=1
\quad\text{nor}\quad
\gcd(a_3,\mathscr R_3)=1.
\]
It includes the allowed endpoint \(a_3=Y\); the strict upper endpoint
\(a_3<10Y\) remains unchanged.

Authority classes:
- PROJECT_THEOREM: PR6, SD6, GCU-2, GC2B-4.
- LOCAL_PROOF: the factorization and sum-of-two-squares contradiction above.