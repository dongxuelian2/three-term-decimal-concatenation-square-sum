Summary: Terminal valuation eliminates one two-adic orientation, while both recovery signs in the unique surviving orientation admit exact normal forms compatible with allocation and reconstruction.

Classification: NEW_LEMMA. Worker verification: VERDICT: CORRECT.

Let
\[
d=2^a,\qquad h=2^{2a-2},\qquad
z=(J+1)5^F+u.
\]
The terminal conditions
\[
k+1=2^Az,\qquad v_2(z)=t+2,\qquad 2a-A=t+3
\]
force
\[
v_2(k+1)=2a-1.
\]
Writing
\[
m=\frac{z}{2^{t+2}},
\]
one obtains the unique compatible orientation
\[
\boxed{s_+=2a-1,\quad m_+=m,\quad s_-=1,\quad m_-=hm-1.}
\]
Thus the opposite orientation is impossible for both recovery signs.

The odd factor \(m\) remains coupled to the unique moving quotient:
\[
m=\frac{(J+1)5^F+u}{2^{t+2}},
\qquad
qu\equiv2^{t+3}Q\pmod{5^F}.
\]
All growing two-adic and fixed quotient congruences remain mandatory.

The recovery identities imply
\[
Y=dZ.
\]
Since \(D\) and the allocation factors are odd, \(a_3\) is odd, whereas \(Y\) and \(10Y\) are even. Hence the formal half-open window
\[
Y\le a_3<10Y
\]
has the effective integer form
\[
Y+1\le a_3\le10Y-1.
\]
The lower endpoint is removed only by this derived parity argument.

Put \(\delta=a_3\).

For \(L_-\)-recovery, every allocation survivor has odd positive integers
\(\delta,M\) satisfying
\[
M>m\delta,\qquad N=hM-\delta.
\]
Then
\[
D=M(hM-\delta),
\]
\[
w_0=\frac d2(M-m\delta),
\]
\[
\mathscr R_3=(2hm-1)M-hm^2\delta,
\]
\[
Q_3=\delta\mathscr R_3,
\]
and
\[
ZH_1=\frac d2\bigl((2hm-1)M-m\delta\bigr).
\]

For \(L_+\)-recovery, every allocation survivor has odd positive integers
\(\delta,N\) satisfying
\[
\frac{hm^2\delta}{2hm-1}<N<m\delta,
\qquad M=hN-\delta.
\]
Then
\[
D=N(hN-\delta),
\]
\[
w_0=\frac d2(m\delta-N),
\]
\[
\mathscr R_3=(2hm-1)N-hm^2\delta,
\]
\[
Q_3=\delta\mathscr R_3,
\]
and
\[
ZH_1=\frac d2\bigl((2hm-1)N-m\delta\bigr).
\]

Direct substitution verifies in both signs
\[
(ZH_1)^2-w_0^2=KD,
\]
\[
Ka_3+d^2\mathscr R_3=2YH_1,
\]
and
\[
(a_3+YH_1)^2=k^2(a_3^2+d^2D).
\]
Thus allocation and the two reconstruction equations alone do not close either sign.

Exact auxiliary families realize values adjacent to both third-block endpoints, repeated and shared odd square factors, and the minimum
\[
w_0=d.
\]
They are not complete candidates because the canonical digit representations, full terminal quotient constraints, reducedness predicates, and moving congruences remain to be imposed.

The remaining obstruction is the simultaneous satisfaction of:
\[
D=(2^Ra_1)^2+a_2^2,\qquad H_1=a_1T+10a_2,
\]
the canonical digit ranges and reducedness conditions, the full moving quotient and growing two-adic congruence, and one of the two displayed sign normal forms.

Authority classes:
- PROJECT_THEOREM: PR6, SD6, GCU-2, GC2B-4.
- LOCAL_PROOF: orientation elimination, endpoint parity, sign normal forms, and compatibility mechanisms above.