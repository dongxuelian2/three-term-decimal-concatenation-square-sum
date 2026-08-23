Summary: Positive-complement recovery is equivalent to an exact close conjugate-factor pair coupled to the terminal quotient, two-adic allocation, recovery window, and reducedness conditions.

Classification: LOCAL_PROOF from [[lemmas/recovery-sign-normal-form]] and [[lemmas/factor-quotient-character]]. Independent worker verification: VERDICT: CORRECT.

On the negative frontier put
\[
d=2^a,\qquad Z=2^A5^F,\qquad Y=10^F=dZ,
\]
\[
D=(2^Ra_1)^2+a_2^2,\qquad P_0=ZH_1,\qquad K=k^2-1.
\]
Assume
\[
w_0^2=P_0^2-KD,\qquad Q_3=D-w_0^2>0.
\]
Define
\[
X=P_0-w_0,\qquad X'=P_0+w_0.
\]
Then
\[
\boxed{XX'=KD,\qquad X+X'=2P_0,\qquad 0\le X'-X<2\sqrt D,}
\]
and \(X,X'>0\).

For \(\varepsilon\in\{\pm1\}\), let \(X_\varepsilon=P_0+\varepsilon w_0\). The recovery factors satisfy
\[
P_0+\varepsilon kw_0
=\frac{(k+1)X_\varepsilon-(k-1)X_{-\varepsilon}}2,
\]
\[
P_0-\varepsilon kw_0
=\frac{(k+1)X_{-\varepsilon}-(k-1)X_\varepsilon}2.
\]
Thus recovery with sign \(\varepsilon\) requires
\[
\boxed{
a_3=
\frac{d\bigl((k+1)X_\varepsilon-(k-1)X_{-\varepsilon}\bigr)}
{2K}
}
\]
to be an odd integer satisfying
\[
\boxed{Y<a_3<10Y,}
\]
and requires the complementary positivity condition
\[
\boxed{(k+1)X_{-\varepsilon}>(k-1)X_\varepsilon.}
\]
The geometric lower endpoint \(a_3=Y\) is allowed upstream but fails reducedness on this frontier; \(a_3=10Y\) fails the strict upper window.

The terminal quotient data are
\[
q=2^{2a}Q-1,
\]
\[
5^{F+R}=q(J5^F+u)-2^{t+3}Q,\qquad 1\le u<5^F,
\]
\[
k=2^A\bigl((J+1)5^F+u\bigr)-1,
\]
with the full moving and binary congruences inherited from [[lemmas/factor-quotient-character]]. Since \(A\ge5\),
\[
v_2(k-1)=1,
\]
and the exact condition \(v_2(k^2-1)=2a\) is equivalent to
\[
\boxed{
v_2\bigl((J+1)5^F+u\bigr)=t+2.
}
\]

If \(w_0=0\), then \(X=X'=P_0\), both recovery signs coincide, and
\[
\boxed{
a_3=\frac{dP_0}{K}=\frac{YH_1}{K},
\qquad
\mathscr R_3=\frac{P_0}{d}.
}
\]
This case remains subject to integrality, the strict recovered window, and reducedness; it cannot be discarded merely from \(Q_3>0\).

The factor-pair formulation does not itself close the branch. The unresolved issue is control of the odd-prime allocation in
\[
XX'=(k^2-1)D
\]
together with the moving quotient class modulo \(5^F\).