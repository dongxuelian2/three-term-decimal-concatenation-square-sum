Summary: Exact recovery produces incompatible five-adic congruences, closing the unit negative-complement branch.

Classification: BRANCH_CLOSURE. Worker verification: VERDICT: CORRECT.

There is no complete candidate in
\[
L_+,\qquad Q_3<0,\qquad v_5(g)=v_5(D)=0.
\]
In fact, only \(v_5(g)=0\) is needed.

Assume such a complete candidate. Set
\[
d=2^a,\quad B=d^2,\quad C=2^A,\quad
E=B/C=2^{t+3},
\]
\[
A=2a-3-t,\quad F=a+A,\quad P=5^F,\quad
Y=dCP,\quad Z=CP.
\]
The terminal factor pair and quotient normalization give
\[
q=BQ-1,\qquad q\equiv\pm2\pmod5,
\]
and a unique moving quotient \(u\), \(1\le u<P\), with
\[
K=JP+u,
\]
\[
5^{F+R}=qK-EQ,\qquad r=CK-1,\qquad
qu\equiv EQ\pmod P.
\]
Comparing the terminal factors yields
\[
EQ=K+2P.
\]
Consequently, for
\[
n=\frac{k+1}{C},
\]
one has
\[
n=K+P=EQ-P. \tag{1}
\]

The exact negative-complement recovery writes
\[
D=ge,\qquad
a_3=\frac{Be}{4}-g,\qquad
N_3=\frac{Be}{4}+g.
\]
From
\[
a_3+YH_1=kN_3
\]
one obtains
\[
n(BD+4g^2)=4dPH_1g+2ED. \tag{2}
\]
Put
\[
X_0=BD+4g^2.
\]
Reducing (2) modulo \(P\), using (1), gives
\[
QX_0\equiv2D\pmod P.
\]
Since \(BQ=q+1\), this becomes
\[
(q-1)D+4Qg^2\equiv0\pmod P. \tag{3}
\]

The complementary terminal-factor identity gives
\[
P(5^R+2q)=\frac{q^2-1}{C}.
\]
Combining it with (2) yields the opposite-sign congruence
\[
(q-1)D-4Qg^2\equiv0\pmod P. \tag{4}
\]
Subtracting (4) from (3),
\[
P\mid8Qg^2.
\]
But \(5\mid P\), \(5\nmid g\), and \(5\nmid Q\): otherwise
\[
q=BQ-1\equiv-1\pmod5,
\]
contrary to \(q\equiv\pm2\pmod5\). This is impossible.

The proof retains the moving congruence modulo \(5^F\), the strict quotient and digit windows, and the complete-candidate equations. It uses only forward recovery consequences, no bounded search, and no unsupported recovered-pair gcd.

Authority classes:
- PROJECT_THEOREM: PR6, SD6, GCU-2, GC2B-4.
- LOCAL_PROOF: the two incompatible recovery congruences above.