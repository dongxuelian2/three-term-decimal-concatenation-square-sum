Summary: The L-plus recovery system reduces exactly to a finite canonical third-digit progression and the same quadratic digit equation as L-minus.

Classification: NEW_LEMMA. Independent worker verification: VERDICT: CORRECT.

Retain
\[
d=2^a,\qquad h=2^{2a-2},\qquad k=2hm-1,\qquad
c=m(hm-1),
\]
\[
X_0=a_1\,10^{R-1}+a_2,\qquad
L=2^{a-t-2}5^{F+1}X_0,
\]
and
\[
D=(2^Ra_1)^2+a_2^2.
\]
Let \(\delta=a_3\). The exact \(L_+\) recovery relation is
\[
L=c\delta-ke.
\]

Consequently \(\delta\) belongs to the finite progression
\[
\mathcal I_+
=
\left\{
\delta:
10^F<\delta<10^{F+1},\
c\delta-L\in k\mathbb Z_{>0},\
\frac{c\delta}{2}<L\le c\delta-k
\right\},
\]
intersected with the inherited canonical digit, endpoint, reducedness, quotient, and reconstruction predicates. For every \(\delta\in\mathcal I_+\),
\[
e=\frac{c\delta-L}{k}
\]
is uniquely recovered.

Eliminating \(e\) from the recovered factors and using
\[
k^2-1=d^2c
\]
gives the necessary-and-sufficient quadratic criterion
\[
\boxed{
k^2D=d^2L^2+2L\delta-c\delta^2.
}
\]

Thus both recovery signs have the same canonical quadratic equation. Their only structural difference is the sign-specific finite progression and the formula recovering \(e\).

The exact third-block window remains
\[
10^F<\delta<10^{F+1}.
\]
Shared factors are retained; in particular, no pairwise coprimality of the recovered factors is imposed. The inherited scale recovery and both reconstruction equations are recovered exactly from the progression relation and quadratic criterion.

This lemma does not assert that \(\mathcal I_+\) is empty.

Authority classes:
- PROJECT_THEOREM: `GP3`, `PR6`, `SD6`, `GCU-2`, `GC2B-4`.
- LOCAL_PROOF: elimination of \(e\), the finite progression, the quadratic criterion, shared-factor preservation, and reconstruction.