Summary: The positive-complement allocation is verified for both recovery signs and both two-adic orientations, retaining all repeated odd square factors.

Classification: MINOR_REPAIR. Worker verification: VERDICT: CORRECT.

Let
\[
d=2^a,\qquad P=ZH_1,\qquad K=k^2-1,
\]
and suppose
\[
w_0>0,\qquad w_0^2=P^2-KD,\qquad Q_3=D-w_0^2>0,
\]
with
\[
A\ge5,\qquad t\ge0,\qquad 2a-A=t+3.
\]
Thus \(a\ge4\). Put
\[
C=P-w_0,\qquad E=P+w_0.
\]
Then
\[
0<C<E,\qquad CE=KD,\qquad E-C=2w_0<2\sqrt D.
\]

Write
\[
k-1=2^{s_-}m_-,\qquad k+1=2^{s_+}m_+,
\]
where \(m_\pm\) are odd. Then
\[
s_-+s_+=2a,\qquad \{s_-,s_+\}=\{1,2a-1\},
\qquad K=d^2m_-m_+.
\]

For either recovery sign, the recovery identity and \(D\) odd imply
\[
v_2(C)=v_2(E)=a.
\]
Moreover, every full odd prime power dividing \(m_-\) enters the recovery factor paired with \(m_-\), and every full odd prime power dividing \(m_+\) enters the complementary factor paired with \(m_+\). This remains valid for repeated prime powers and primes shared with \(D\), \(K\), or \(ZH_1\); no coprimality of these quantities is assumed.

For \(L_-\)-recovery there exist positive integers \(M,N\) with \(MN=D\) such that
\[
C=d\,m_-M,\qquad E=d\,m_+N,
\]
and
\[
a_3=\frac{2^{s_+}M-2^{s_-}N}{2},
\]
\[
\mathscr R_3=
\frac{2^{s_+}m_+^2N-2^{s_-}m_-^2M}{2}.
\]
Consequently,
\[
2^{s_+}M>2^{s_-}N
\]
and
\[
2^{s_+}m_+^2N>2^{s_-}m_-^2M.
\]
The close-factor equations are
\[
d(m_-M+m_+N)=2ZH_1,
\]
\[
0<d(m_+N-m_-M)<2\sqrt D.
\]

For \(L_+\)-recovery the allocation is exchanged:
\[
C=d\,m_+M,\qquad E=d\,m_-N,\qquad MN=D,
\]
and
\[
a_3=\frac{2^{s_+}N-2^{s_-}M}{2},
\]
\[
\mathscr R_3=
\frac{2^{s_+}m_+^2M-2^{s_-}m_-^2N}{2}.
\]
Consequently,
\[
2^{s_+}N>2^{s_-}M
\]
and
\[
2^{s_+}m_+^2M>2^{s_-}m_-^2N.
\]
The close-factor equations are
\[
d(m_+M+m_-N)=2ZH_1,
\]
\[
0<d(m_-N-m_+M)<2\sqrt D.
\]

Neither pair of odd square factors may be cancelled. In particular, one may not assume
\[
\gcd(D,ZH_1)=1
\]
or replace either relevant gcd by \(d\).

Every surviving R2 state must additionally satisfy
\[
D=(2^Ra_1)^2+a_2^2,\qquad H_1=a_1T+10a_2,
\]
\[
w_0^2=Z^2H_1^2-KD,\qquad Q_3=a_3\mathscr R_3>0,
\]
\[
Ka_3+d^2\mathscr R_3=2YH_1,
\]
\[
(a_3+YH_1)^2=k^2(a_3^2+d^2D),
\]
the true third-block window and digit reducedness, and the terminal quotient system
\[
q=2^{2a}Q-1,\qquad 1\le J\le9,\qquad 1\le u<5^F,
\]
\[
\frac{5^R}{J+1}<q<\frac{5^R}{J},
\]
\[
5^{F+R}=q(J5^F+u)-2^{t+3}Q,
\]
\[
k=2^A((J+1)5^F+u)-1,
\]
\[
v_2((J+1)5^F+u)=t+2,
\]
\[
qu\equiv2^{t+3}Q\pmod{5^F},
\]
together with every fixed congruence from [[lemmas/quotient-fixed-residues]]. The fixed congruences supplement rather than replace the moving class modulo \(5^F\).

This theorem repairs the allocation defect but does not close R2.

Authority classes:
- PROJECT_THEOREM: PR6, SD6, GCU-2, GC2B-4.
- LOCAL_PROOF: the orientation-safe allocation and positivity formulas above.