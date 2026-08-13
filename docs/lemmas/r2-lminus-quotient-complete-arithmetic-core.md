Summary: The surviving-orientation L-minus branch has a quotient-complete, parity-complete, reconstruction-complete parametrization whose remaining obstruction is the canonical digit-divisor exclusion.

Classification: NEW_LEMMA. Worker verification: VERDICT: CORRECT.

Let
\[
t\ge0,\qquad R=2^tR_0,\qquad R_0\ \text{odd},
\]
and
\[
A\ge5,\qquad 2a-A=t+3,\qquad
d=2^a,\qquad h=2^{2a-2},\qquad E=2^{t+3}.
\]
Retain
\[
1\le J\le9,\qquad 1\le u<5^F,
\]
and define
\[
q=d^2Q-1,\qquad q\equiv\pm2\pmod5,
\]
with
\[
\frac{5^R}{J+1}<q<\frac{5^R}{J}.
\]

The complete quotient conditions are
\[
5^{F+R}=q(J5^F+u)-EQ,
\]
\[
qu\equiv EQ\pmod{5^F},
\]
and
\[
u\equiv-5^F(5^R+J)
-2^{t+2}\bigl(7-5^F\omega_t(R_0)\bigr)
\pmod{2^{t+5}}.
\]
The complementary factor is retained:
\[
r=2^A(J5^F+u)-1,\qquad
qr=1+2^A5^{F+R}.
\]

Write
\[
z=(J+1)5^F+u=2^{t+2}m,
\]
where \(m\) is odd. Then
\[
k=2^Az-1=2hm-1,\qquad
K=k^2-1=d^2m(hm-1).
\]
The moving and growing quotient congruences become
\[
qm\equiv2Q\pmod{5^F}
\]
and
\[
m\equiv-7+5^F\omega_t(R_0)
+\frac{5^F(1-5^R)}{2^{t+2}}
\pmod8.
\]
All fixed residues modulo \(5,8,40\) remain additional necessary conditions and do not replace either displayed moving condition.

The separate parity conditions are
\[
t=0:\qquad F\text{ even},\quad R\text{ odd},\quad a\text{ odd},
\]
and
\[
t\ge1:\qquad F\text{ odd},\quad R\text{ even},\quad a\equiv t\pmod2.
\]

For \(L_-\)-recovery let \(\delta=a_3\) be odd. The inequality
\[
M>m\delta
\]
is equivalent to a unique integer
\[
e=\frac{M-m\delta}{2}\ge1.
\]
Conversely, for every odd \(\delta>0\) and \(e\ge1\), define
\[
M=m\delta+2e,
\]
\[
N=(hm-1)\delta+2he=hM-\delta,
\]
\[
D=MN,
\]
and
\[
S=m(hm-1)\delta+(2hm-1)e.
\]
Then
\[
w_0=de,\qquad ZH_1=dS,
\]
\[
\mathscr R_3
=m(hm-1)\delta+2(2hm-1)e>0,
\qquad
Q_3=\delta\mathscr R_3.
\]

No prime-power cancellation is permitted. The exact shared-factor identity is
\[
\gcd(M,N)=\gcd(e,\delta).
\]
This is an identity, not an authorization to impose a recovered-pair coprimality condition.

The remaining digit-divisor and scale conditions are
\[
D=(2^Ra_1)^2+a_2^2,\qquad
H_1=a_1T+10a_2,
\]
\[
H_1\mid dS,\qquad
Z=\frac{dS}{H_1},\qquad
Y=dZ,
\]
and
\[
d^2S<\delta H_1<10d^2S.
\]
The last inequality is equivalent to the effective third-block window
\[
Y+1\le\delta\le10Y-1.
\]

All exact canonical digit requirements and original authorized reducedness predicates remain separate conjuncts. They cannot be replaced by
\[
\gcd(M,N)=1,
\quad \gcd(D,ZH_1)=1,
\quad \gcd(a_3,D)=1,
\quad\text{or}\quad
\gcd(a_3,\mathscr R_3)=1.
\]

The identities
\[
S-e=(hm-1)M,\qquad S+e=mN
\]
give
\[
(ZH_1)^2-w_0^2=KD.
\]
Direct expansion also gives
\[
D-w_0^2=\delta\mathscr R_3=Q_3,
\]
\[
K\delta+d^2\mathscr R_3=2YH_1,
\]
and
\[
(\delta+YH_1)^2
=k^2(\delta^2+d^2D).
\]
Thus the core retains both reconstruction equations and does not itself close the branch.

The remaining obligation is the canonical \(L_-\) digit-divisor exclusion for quotient-compatible triples \((m,\delta,e)\) with \(e\ge1\).

Authority classes:
- PROJECT_THEOREM: PR6, SD6, GCU-2, GC2B-4.
- LOCAL_PROOF: quotient substitution, \(L_-\) parametrization, shared-factor identity, endpoint equivalence, and reconstruction identities above.