Summary: The L-minus recovery system reduces exactly to a finite canonical third-digit progression and one quadratic digit equation.

Classification: NEW_LEMMA. Independent worker verification: VERDICT: CORRECT.

Retain
\[
d=2^a,\qquad h=2^{2a-2},\qquad k=2hm-1,\qquad
c=m(hm-1),
\]
\[
P=5^{F+1},\qquad
X_0=a_1\,10^{R-1}+a_2,\qquad
L=2^{a-t-2}PX_0,
\]
and
\[
D=(2^Ra_1)^2+a_2^2.
\]
Let \(\delta=a_3\). The exact \(L_-\) recovery identities are
\[
L=c\delta+ke,\qquad L^2-cD=e^2.
\]

Consequently \(\delta\) must lie in the finite progression
\[
\mathcal I=
\left\{
\delta:
10^F<\delta<10^{F+1},\
L-c\delta\in k\mathbb Z_{>0}
\right\},
\]
intersected with the inherited endpoint, reducedness, and canonical digit predicates. For each \(\delta\in\mathcal I\),
\[
e=\frac{L-c\delta}{k}
\]
is uniquely determined.

Using
\[
k^2-1=d^2c,
\]
the square equation is equivalent to
\[
\boxed{
k^2D=d^2L^2+2L\delta-c\delta^2.
}
\]

Indeed, substituting \(ke=L-c\delta\) into \(L^2-cD=e^2\), multiplying by \(k^2\), and using \(k^2-1=d^2c\) gives the displayed equation. Reversing these steps recovers the square equation and \(e\).

Thus the complete remaining \(L_-\) arithmetic obstruction is an integral exclusion problem over the finite progression \(\mathcal I\):
\[
k^2\bigl((2^Ra_1)^2+a_2^2\bigr)
=
d^2\bigl(2^{a-t-2}5^{F+1}X_0\bigr)^2
+2\bigl(2^{a-t-2}5^{F+1}X_0\bigr)\delta
-c\delta^2.
\]
The dependent corrected residue modulo \(5^{F+1}\) is already contained in this formulation and is not an additional obstruction.

This lemma does not claim that the progression is empty. Strict digit windows, authorized reducedness, quotient filters, endpoints, and both original reconstruction equations remain mandatory external intersections.

Authority classes:
- PROJECT_THEOREM: `PR6`, `SD6`, `GCU-2`, `GC2B-4`.
- LOCAL_PROOF: elimination of \(e\), the finite progression, and the quadratic criterion.