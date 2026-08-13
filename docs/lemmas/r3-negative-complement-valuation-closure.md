Summary: Both alternatives in the verified unequal five-adic classification are impossible, closing R3.

Classification: BRANCH_CLOSURE. Worker verification: VERDICT: CORRECT.

There is no complete candidate in
\[
L_+,\qquad Q_3<0,\qquad v_5(g)<v_5(D).
\]

Assume such a candidate. Retain
\[
D=(2^Ra_1)^2+a_2^2,\qquad \gcd(2^Ra_1,a_2)=1,
\]
the strict digit windows, the moving quotient modulo \(5^F\), and both original equations. Put
\[
B=2^{2a},\quad C=2^A,\quad E=2^{t+3},\quad
P=5^F,\quad A=2a-3-t,\quad F=a+A,
\]
and
\[
c=2^{2a-2}.
\]
The canonical negative-complement identities are
\[
D=ge,\qquad a_3=ce-g,\qquad N_3=ce+g,
\]
and
\[
a_3+YH_1=kN_3,\qquad H_1=a_1\,10^{R+1}+10a_2.
\]
Hence
\[
YH_1=(k-1)ce+(k+1)g. \tag{1}
\]

Because \(2^Ra_1\) is even and coprime to \(a_2\), \(a_2\) is odd. Thus \(D\), \(g\), and \(e\) are odd. Also
\[
v_2(H_1)=1. \tag{2}
\]

The verified classification [[lemmas/negative-complement-unequal-five-adic-classification]] leaves exactly two alternatives.

First suppose
\[
v_5(e)=v_5(g)=h<F
\]
with normalized cancellation
\[
P\mid(q-1)e-4Qg. \tag{3}
\]
Since \(P\mid Y\), equation (1), \(k\equiv q\pmod P\), and
\[
q+1=2^{2a}Q=4cQ
\]
give
\[
P\mid(q-1)e+4Qg. \tag{4}
\]
Adding and subtracting (3) and (4) yields
\[
P\mid2(q-1)e,\qquad P\mid8Qg.
\]
Here \(5\nmid q-1\) because \(q\equiv\pm2\pmod5\), and \(5\nmid Q\), since otherwise \(q\equiv-1\pmod5\). Therefore
\[
P\mid e,\qquad P\mid g,
\]
contradicting \(v_5(e)=v_5(g)=h<F\).

Now suppose
\[
\min(v_5(e),v_5(g))\ge F.
\]
Let
\[
n=EQ-P.
\]
Then \(n\) is odd, and the terminal identities give
\[
k+1=Cn,\qquad v_2(k+1)=A,
\]
while
\[
k-1=Cn-2
\]
has
\[
v_2(k-1)=1.
\]
Thus the two terms on the right side of (1) have valuations
\[
v_2((k-1)ce)=2a-1,\qquad
v_2((k+1)g)=A.
\]
Since
\[
2a-1-A=t+2>0,
\]
their sum has valuation \(A\). But
\[
Y=10^F,\qquad v_2(H_1)=1,
\]
so
\[
v_2(YH_1)=F+1=a+A+1>A,
\]
contradicting (1).

The two alternatives are disjoint and exhaustive. Hence R3 is closed. No recovered-pair gcd, bounded computation, fixed-residue replacement, or reverse reconstruction is used.

Authority classes:
- PROJECT_THEOREM: PR6, SD6, GCU-2, GC2B-4.
- LOCAL_PROOF: the two contradictions above.