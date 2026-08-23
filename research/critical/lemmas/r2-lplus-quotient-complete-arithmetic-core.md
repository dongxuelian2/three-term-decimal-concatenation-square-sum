Summary: The surviving-orientation L-plus branch has an exact quotient-complete parametrization; its sole remaining obstruction is the canonical digit-divisor system.

Classification: NEW_LEMMA. Worker verification: VERDICT: CORRECT.

Let
\[
d=2^a,\qquad h=2^{2a-2},\qquad 2a-A=t+3.
\]
Retain positive integers \(F,R,Q\), \(1\le J\le9\), and \(1\le u<5^F\). Define
\[
q=2^{2a}Q-1,\qquad
z=(J+1)5^F+u=2^{t+2}m,
\]
where \(m\) is odd. Then
\[
k=2^Az-1=2hm-1,\qquad
K=k^2-1=d^2m(hm-1).
\]

The complete quotient conditions include
\[
\frac{5^R}{J+1}<q<\frac{5^R}{J},
\]
\[
5^{F+R}=q(J5^F+u)-2^{t+3}Q,
\]
\[
qu\equiv2^{t+3}Q\pmod{5^F},
\]
and the mandatory growing congruence
\[
u\equiv-5^F(5^R+J)
-2^{t+2}\bigl(7-5^F\omega_t(R_0)\bigr)
\pmod{2^{t+5}}.
\]
The complementary factor remains
\[
r=2^A(J5^F+u)-1,\qquad qr=1+2^A5^{F+R}.
\]

The fixed parity conditions are
\[
t=0:\quad F\text{ even},\ R\text{ odd},\ a\text{ odd},
\]
\[
t\ge1:\quad F\text{ odd},\ R\text{ even},\ a\equiv t\pmod2.
\]
All fixed residues modulo \(5,8,40\) remain additional necessary conditions.

Substitution of
\[
u=2^{t+2}m-(J+1)5^F
\]
gives the two exact quotient classes
\[
qm\equiv2Q\pmod{5^F}
\]
and
\[
m\equiv-7+5^F\omega_t(R_0)
+\frac{5^F(1-5^R)}{2^{t+2}}
\pmod8.
\]
In particular, the second condition retains the information of the growing
\(2^{t+5}\)-congruence and is not replaceable by the fixed mod-\(40\) table.

For \(L_+\)-recovery, put
\[
e=\frac{ma_3-N}{2}.
\]
The exact strict interval is
\[
1\le e<
\frac{m(hm-1)a_3}{2(2hm-1)}.
\]
Conversely, for odd \(a_3>0\) and an integer \(e\) in this interval, define
\[
N=ma_3-2e,
\]
\[
M=(hm-1)a_3-2he=hN-a_3,
\]
\[
D=NM,
\]
\[
S=m(hm-1)a_3-(2hm-1)e.
\]
Then
\[
w_0=de,\qquad ZH_1=dS,
\]
\[
\mathscr R_3=m(hm-1)a_3-2(2hm-1)e>0,
\]
and no odd prime power has been cancelled. The exact shared-factor relation is
\[
\gcd(N,M)=\gcd(e,a_3).
\]

The canonical digit and endpoint conditions reduce to
\[
D=(2^Ra_1)^2+a_2^2,\qquad H_1=a_1T+10a_2,
\]
\[
H_1\mid dS,
\]
and, after setting
\[
Z=\frac{dS}{H_1},
\]
\[
d^2S<a_3H_1<10d^2S.
\]
This last inequality is equivalent to the effective third-block window.

The identities
\[
S-e=mM,\qquad S+e=(hm-1)N
\]
verify
\[
(ZH_1)^2-w_0^2=KD,
\]
\[
D-w_0^2=a_3\mathscr R_3>0,
\]
\[
Ka_3+d^2\mathscr R_3=2YH_1,
\]
and the original square reconstruction equation once \(Y=dZ\).
Thus reconstruction alone does not close this sign.

The remaining obligation is the canonical digit-divisor exclusion: prove that
no quotient-compatible \(m,a_3,e\) in the displayed interval can satisfy the
two digit representations, divisibility and endpoint inequalities, exact
digit ranges, and authorized reducedness predicates.

Authority classes:
- PROJECT_THEOREM: PR6, SD6, GCU-2, GC2B-4.
- LOCAL_PROOF: quotient substitution, L-plus parametrization, shared-factor identity, and reconstruction verification above.