Summary: Full recovery yields a unit-width interval only when the complementary quotient is positive; the nonpositive L-plus cases remain separate.

All statements below are LOCAL_PROOF from the displayed PR6/SD6 recovery identities. Worker verification: VERDICT: CORRECT.

Assume
\[
u=2^R,\quad d=2^a,\quad Y=10^F,\quad Z=2^A5^F,\quad F=a+A,
\]
so
\[
\boxed{dZ=Y}.
\]
Let
\[
H_1=a_1T+10a_2,\qquad
\mathcal R=(ua_1)^2+a_2^2,\qquad K=k^2-1,
\]
\[
w_0^2=Z^2H_1^2-K\mathcal R,\qquad
L_\pm=ZH_1\pm kw_0.
\]
For a valid recovery sign \(\varepsilon\),
\[
L_\varepsilon=(K/d)a_3,\qquad
L_{-\varepsilon}=d\mathscr R_3,
\]
\[
Q_3:=\mathcal R-w_0^2=a_3\mathscr R_3,
\qquad
Ka_3+d^2\mathscr R_3=2YH_1.
\]

Define
\[
\Xi=\frac{Z^2H_1^2}{\mathcal R}.
\]
Then
\[
Q_3=\mathcal R(k^2-\Xi),
\]
while \(w_0^2\ge0\) gives
\[
k^2\le\Xi+1.
\]
Hence
\[
\boxed{
\begin{array}{c|c}
Q_3>0&\sqrt\Xi<k\le\sqrt{\Xi+1},\\
Q_3=0&k=\sqrt\Xi,\\
Q_3<0&k<\sqrt\Xi.
\end{array}}
\]
The first interval has length
\[
\sqrt{\Xi+1}-\sqrt\Xi<1.
\]

Consequently:

- Every \(L_-\)-recovery has \(Q_3>0\), so the unit-width mechanism applies.
- An \(L_+\)-recovery has the unit-width conclusion only when \(Q_3>0\).
- If an \(L_+\)-recovery has \(Q_3=0\), then \(L_-=0\) and only \(L_+\) can recover.
- If an \(L_+\)-recovery has \(Q_3<0\), then \(L_-<0\) and only the one-sided bound \(k<\sqrt\Xi\) remains.

The recovery equation also gives
\[
\boxed{Ka_3=YH_1+\varepsilon dkw_0}.
\]
Thus
\[
L_+\text{-recovery}\Rightarrow Ka_3\ge YH_1,
\]
\[
L_-\text{-recovery}\Rightarrow Ka_3\le YH_1.
\]
Using \(Y\le a_3<10Y\),
\[
L_+\text{-recovery}\Rightarrow K>H_1/10,
\]
and
\[
L_-\text{-recovery}\Rightarrow K\le H_1.
\]
Since \(F\ge1\), the allowed geometric endpoint \(a_3=Y\) fails
\(\gcd(a_3,du)=1\); therefore a complete \(L_-\)-recovery actually has
\[
K<H_1.
\]
The endpoint \(a_3=10Y\) remains strictly excluded.

For every \(Q_3>0\) recovery, if the inherited terminal identity
\[
qr=1+Z5^R,\qquad r=k-Z
\]
is retained, then
\[
\boxed{\sqrt\Xi-Z<r\le\sqrt{\Xi+1}-Z}.
\]
This interval has length less than one, so at most one integer \(r\) survives; after \(r\) is fixed,
\[
q=\frac{1+Z5^R}{r}
\]
is determined exactly.

A further sign-independent identity is
\[
\boxed{(a_3+YH_1)^2=k^2(a_3^2+d^2\mathcal R)}.
\]
Therefore
\[
a_3^2+d^2\mathcal R=N_3^2,\qquad
a_3+YH_1=kN_3
\]
for an integer \(N_3>0\).

The unit-width argument must not be extended to \(L_+\)-recovery with
\(Q_3\le0\). Exact auxiliary recovery data exist with
\[
L_-<0,\qquad Q_3<0,\qquad\mathscr R_3<0.
\]
Such auxiliary data do not satisfy the inherited terminal factor identity and are not complete candidates, but they rigorously refute the sign collapse.