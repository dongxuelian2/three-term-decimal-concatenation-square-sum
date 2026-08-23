Summary: The exact negative-complement identity forces a five-adic lift, excluding the subcase \(v_5(D)=v_5(g)>0\).

Classification: LOCAL_PROOF from the corrected \(L_+,Q_3<0\) factor–recovery identity. Independent worker verification: VERDICT: CORRECT.

Assume
\[
PB=EC,
\qquad P=5^F,\qquad E=2^{t+3},
\]
where
\[
B=(5^R+q)(d^2D+4g^2)-4dqH_1g,
\]
\[
C=(q-1)D-4Qg^2,
\]
and \(g\mid D\) is positive and odd.

Writing \(D=gD_0\) shows
\[
B=g\bigl((5^R+q)(d^2D_0+4g)-4dqH_1\bigr),
\]
so \(g\mid B\). Hence \(5^Fg\mid PB=EC\). Since \(E\) is a power of \(2\) and \(g\) is odd,
\[
\gcd(5^Fg,E)=1.
\]
Euclid's lemma therefore gives
\[
\boxed{5^Fg\mid C}
\]
and, in particular,
\[
\boxed{5^{F+v_5(g)}\mid (q-1)D-4Qg^2.}
\]

For nonzero \(C\), put
\[
\delta=v_5(D),\qquad \gamma=v_5(g),\qquad
\alpha=v_5(q-1),\qquad \kappa=v_5(Q).
\]
The two terms of \(C\) have valuations
\[
\alpha+\delta,\qquad \kappa+2\gamma.
\]
If these valuations differ, then
\[
v_5(C)=\min(\alpha+\delta,\kappa+2\gamma).
\]
If they are equal to \(h\), then the normalized terms must cancel to the additional order required by
\[
v_5(C)\ge F+\gamma.
\]
The zero case \(C=0\) is covered by \(v_5(0)=+\infty\); the exact identity also gives \(B=0\iff C=0\).

On the actual negative frontier,
\[
q\equiv\pm2\pmod5,
\]
so \(v_5(q-1)=0\). If
\[
v_5(D)=v_5(g)=s>0,
\]
then the two term-valuations are
\[
s,\qquad v_5(Q)+2s>s.
\]
Thus \(v_5(C)=s\), whereas the lift requires
\[
v_5(C)\ge F+s.
\]
Since the frontier has \(F\ge1\), this is impossible. Therefore
\[
\boxed{v_5(D)=v_5(g)>0\quad\Longrightarrow\quad\text{no }L_+,Q_3<0\text{ recovery}.}
\]

No primality or squarefreeness assumption on \(q,D\), or \(g\) is used.