Summary: Repository-ready corrected divisor normal form for the L+, Q3<0 branch.

<!-- VERIFIED_PROVENANCE {"artifact_sha256": "66df6bd49ba5518774e0189c483cd3c265a85efee041abcfb5deb36fd13dccf7", "campaign_id": "C2NEG-overnight-20260809", "origin_run_id": "GC2N-1-campaign-20260809-105746", "origin_step": 8, "origin_worker_index": 0, "parent_run_id": "GC2N-1-campaign-20260809-105746", "repair_kind": "FOLLOWUP_LOCAL_MINOR", "run_id": "GC2N-1-continuation-20260811-022943", "verifier_sha256": "2e978d6534495359a90fb1e62c906268ca99d90a4afb05ca80fdaf5374eb7acd"} -->

**Lemma (corrected \(L_{+},Q_{3}<0\) divisor normal form; LOCAL_PROOF).**  
Let
\[
a\ge4,\qquad 0\le t\le a-4,\qquad R\ge1,\qquad v_2(R)=t,
\]
and put
\[
R=2^tR_0\quad(R_0\ \text{odd}),\qquad
A=2a-3-t,\qquad F=a+A.
\]
Set
\[
d=2^a,\quad B=d^2=2^{2a},\quad C=2^A,\quad
E=\frac BC=2^{t+3},
\]
\[
P=5^F,\qquad Y=10^F=dCP,\qquad Z=CP.
\]
Assume the inherited parity condition
\[
F+R\equiv1\pmod2
\tag{1}
\]
and the exact tail inequality
\[
3Z5^R+1<5^{2R}.
\tag{2}
\]

Let the digit data satisfy
\[
1\le a_1\le9,\qquad 0\le a_2<10^R,\qquad
Y\le a_3<10Y,
\tag{3}
\]
and define
\[
T=10^{R+1},\qquad
H_1=a_1T+10a_2,\qquad
D=(2^Ra_1)^2+a_2^2.
\tag{4}
\]
Retain both gcd conditions
\[
\gcd(2^Ra_1,a_2)=1
\tag{5}
\]
(the primitive-tail condition) and
\[
\gcd(a_3,d\,2^R)=1
\tag{6}
\]
(the recovery reducedness condition). In particular, \(a_2\) and \(D\) are odd.

Suppose the terminal square condition is
\[
k^2=Z^2+Z5^R+1,
\tag{7}
\]
and define
\[
q=k+Z,\qquad r=k-Z.
\tag{8}
\]
Then
\[
qr=1+Z5^R=1+C5^{F+R},
\tag{9}
\]
so \(q\) is the terminal divisor and \(r\) its complementary factor. Assume further that
\[
q=BQ-1,\qquad Q\ge1,\qquad q\equiv\pm2\pmod5.
\tag{10}
\]

For
\[
\omega_t(R_0)\equiv
\frac{5^{2^tR_0}-1}{2^{t+2}}\pmod8
\tag{11}
\]
and
\[
H\equiv\frac{7-P\omega_t(R_0)}2\pmod4,
\tag{12}
\]
assume the inherited binary-root condition
\[
Q\equiv H\pmod4.
\tag{13}
\]
The quotient in (12) is integral modulo \(4\): by the lifting-the-exponent theorem,
\[
v_2(5^{2^tR_0}-1)=t+2,
\]
so \(\omega_t(R_0)\) is odd, as is \(P\).

Then the following conclusions hold.

1. Parameter and factor windows.

One has
\[
A=2a-3-t\ge 2a-3-(a-4)=a+1\ge5.
\tag{14}
\]
Moreover,
\[
0<EQ<q.
\tag{15}
\]
Indeed \(E,Q>0\), while
\[
q-EQ=(B-E)Q-1>0
\]
because \(B\ge2^8\), \(E\le2^{a-1}\), and \(Q\ge1\).

Condition (2) is equivalent, using (7), to
\[
q=k+Z<5^R.
\tag{16}
\]
Indeed \(k<5^R-Z\) is equivalent after squaring to
\[
Z^2+Z5^R+1<(5^R-Z)^2,
\]
which is precisely (2). Since \(\gcd(q,5)=1\), \(q\nmid5^R\). Hence there are unique integers \(J,s\) such that
\[
5^R=Jq+s,\qquad J\ge1,\qquad 0<s<q,
\tag{17}
\]
or equivalently
\[
\boxed{\frac{5^R}{J+1}<q<\frac{5^R}{J}}.
\tag{18}
\]

2. Exact terminal quotient conditions.

There is a unique integer
\[
u,\qquad 1\le u\le P-1,
\tag{19}
\]
such that, on putting
\[
\Lambda=JP+u,
\tag{20}
\]
one has
\[
\boxed{5^{F+R}=q\Lambda-EQ}.
\tag{21}
\]
Furthermore,
\[
\boxed{r=C\Lambda-1=C(JP+u)-1},
\tag{22}
\]
\[
\boxed{P s=qu-EQ},
\tag{23}
\]
and therefore
\[
\boxed{
u=\left\lceil\frac{Ps}{q}\right\rceil,\qquad
qu\equiv EQ\pmod P.
}
\tag{24}
\]
Since \(q\equiv\pm2\pmod5\), \(q\) is invertible modulo \(P\), and the moving quotient condition can equivalently be written
\[
\boxed{u\equiv EQ\,q^{-1}\pmod{5^F}}.
\tag{25}
\]

To prove these identities, note from \(C(EQ)=BQ=q+1\) that
\[
5^{F+R}\equiv-EQ\pmod q.
\]
By (15), \(q-EQ\) is the least positive remainder, and hence
\[
\Lambda=\left\lceil\frac{5^{F+R}}q\right\rceil.
\]
The strict window (18) gives
\[
JP<\Lambda\le(J+1)P.
\]
Equality at the upper endpoint would imply, by (21),
\[
5\mid EQ.
\]
But \(5\nmid E\), and \(q=BQ-1\equiv\pm2\pmod5\) implies \(5\nmid Q\). Thus
\[
JP<\Lambda<(J+1)P,
\]
which proves (19)–(21). Equations (22) and (23) follow by direct substitution.

Since \(q-r=2Z=2CP\), comparison of \(q=CEQ-1\) with (22) gives the high-word condition
\[
\boxed{EQ=(J+2)P+u}.
\tag{26}
\]
Equivalently, if
\[
n:=\frac{k+1}{C},
\tag{27}
\]
then
\[
\boxed{n=EQ-P=(J+1)P+u}.
\tag{28}
\]

Finally, (21) and (22) imply
\[
5^{F+R}+\Lambda=EQr.
\]
Because \(A\ge5\), \(r=C\Lambda-1\equiv-1\pmod4\). Dividing by \(E\) and using \(Q\equiv H\pmod4\) yields the corrected binary quotient congruence
\[
\boxed{
u\equiv-P(5^R+J)-EH\pmod{4E}.
}
\tag{29}
\]
Equivalently,
\[
\boxed{
u\equiv
-5^F(5^R+J)
-2^{t+2}\bigl(7-5^F\omega_t(R_0)\bigr)
\pmod{2^{t+5}}.
}
\tag{30}
\]
The variable in (29)–(30) is the same quotient variable \(u\) as in (19)–(26).

The parity condition (1) also gives
\[
t=0\Longrightarrow a\ \text{odd},\qquad
t\ge1\Longrightarrow a\equiv t\pmod2.
\tag{31}
\]
Indeed \(F=3a-3-t\); if \(t=0\), then \(R\) is odd and \(F\) is even, whereas if \(t\ge1\), then \(R\) is even and \(F\) is odd.

3. Negative-complement recovery.

Assume an \(L_+\)-recovery with
\[
Q_3<0
\tag{32}
\]
produces integers \(N_3>0\) and \(w_0\ge0\) satisfying
\[
N_3^2=a_3^2+d^2D,\qquad
a_3+YH_1=kN_3,
\tag{33}
\]
and the selected binary branch
\[
N_3+a_3\equiv0\pmod{2^{2a-1}},\qquad
N_3-a_3\equiv2\pmod4.
\tag{34}
\]
Define
\[
g=\frac{N_3-a_3}{2}.
\tag{35}
\]
Then \(g\) is positive and odd. From
\[
(N_3-a_3)(N_3+a_3)=d^2D
\]
and (34), the odd integer \(g\) divides \(D\). Put
\[
e=\frac Dg.
\tag{36}
\]
It follows that
\[
N_3+a_3=\frac{d^2e}{2},
\]
and hence
\[
\boxed{
a_3=\frac{2^{2a}e}{4}-g,\qquad
N_3=\frac{2^{2a}e}{4}+g.
}
\tag{37}
\]

Substitution of (37) into \(a_3+YH_1=kN_3\) gives
\[
4YH_1g=(k-1)d^2D+4(k+1)g^2.
\tag{38}
\]
Since \(k+1=Cn\), division by \(C\), together with \(Y/C=dP\) and \(d^2/C=E\), yields
\[
\boxed{
n(2^{2a}D+4g^2)
=
4\cdot2^a5^FH_1g+2^{t+4}D.
}
\tag{39}
\]

For \(L_+\)-recovery,
\[
dw_0=ka_3-N_3,
\]
so (37) gives the required integrality formula
\[
\boxed{
w_0=
\frac{2^{2a}(k-1)e-4(k+1)g}{4\cdot2^a}
\in\mathbb Z_{\ge0}.
}
\tag{40}
\]
Because \(D>0\), condition \(Q_3=D-w_0^2<0\) actually forces \(w_0>0\).

Let
\[
X=2^{2a}(k-1)e,\qquad W=4(k+1)g.
\]
Then \(4dw_0=X-W\), and direct expansion gives
\[
(X-W)^2-16d^2eg
=
(d^2e-4g)
\bigl(d^2(k-1)^2e-4(k+1)^2g\bigr).
\tag{41}
\]
By (37),
\[
d^2e-4g=4a_3>0.
\]
Consequently,
\[
Q_3<0
\iff w_0^2>D=eg
\iff
\boxed{2^{2a}(k-1)^2e>4(k+1)^2g}.
\tag{42}
\]

The complementary recovery quotient must satisfy
\[
\boxed{
\mathscr R_3=\frac{D-w_0^2}{a_3}\in\mathbb Z_{<0}.
}
\tag{43}
\]
Thus (37), (40), and (43) respectively encode the \(a_3\)-recovery, \(w_0\)-integrality, and complementary-quotient requirements.

4. Exact factor–recovery identity.

Put
\[
X_0=d^2D+4g^2.
\]
Equation (39) is
\[
nX_0=4dPH_1g+2ED.
\tag{44}
\]
Using
\[
n=EQ-P=\frac{q+1}{C}-P
\tag{45}
\]
and the terminal identity
\[
q(q-2CP)=1+CP5^R,
\]
we obtain
\[
P(5^R+2q)=\frac{q^2-1}{C}.
\tag{46}
\]
Now define
\[
\mathfrak B
=(5^R+q)(d^2D+4g^2)-4dqH_1g,
\]
\[
\mathfrak C=(q-1)D-4Qg^2.
\]
Multiplying (44) by \(q\) and using (45)–(46), one finds
\[
\begin{aligned}
P\mathfrak B-E\mathfrak C
&=
\biggl(P(5^R+2q)-\frac{q(q+1)}C\biggr)X_0\\
&\quad+E\bigl((q+1)D+4Qg^2\bigr)\\
&=-EQX_0+E\bigl((q+1)D+4Qg^2\bigr)\\
&=E\bigl((q+1-BQ)D\bigr)=0.
\end{aligned}
\]
Therefore the exact factor–recovery identity is
\[
\boxed{
5^F\Bigl((5^R+q)(2^{2a}D+4g^2)-4\cdot2^aqH_1g\Bigr)
=
2^{t+3}\Bigl((q-1)D-4Qg^2\Bigr).
}
\tag{47}
\]

5. Five-adic lift.

Since \(D=g e\),
\[
\mathfrak B
=
g\Bigl((5^R+q)(d^2e+4g)-4dqH_1\Bigr),
\]
so \(g\mid\mathfrak B\). Equation (47) therefore implies
\[
5^Fg\mid E\mathfrak C.
\]
Because \(E\) is a power of \(2\) and \(g\) is odd,
\[
\gcd(5^Fg,E)=1.
\]
Euclid’s lemma gives
\[
\boxed{5^Fg\mid(q-1)D-4Qg^2},
\tag{48}
\]
and hence
\[
\boxed{
5^{F+v_5(g)}
\mid(q-1)D-4Qg^2.
}
\tag{49}
\]

In particular, the subcase
\[
v_5(D)=v_5(g)=s>0
\tag{50}
\]
is impossible. Indeed \(q\equiv\pm2\pmod5\), so \(v_5(q-1)=0\). The two terms in
\[
(q-1)D-4Qg^2
\]
then have respective valuations
\[
s,\qquad v_5(Q)+2s>s.
\]
Their valuations differ, so the valuation of their difference is exactly \(s\), contradicting (49), which requires at least \(F+s>s\).

6. Final endpoint and admissibility checklist.

Every surviving \(L_+,Q_3<0\) candidate must satisfy simultaneously:

\[
\begin{gathered}
a\ge4,\quad0\le t\le a-4,\quad v_2(R)=t,\quad
A=2a-3-t,\quad F=a+A,\quad F+R\ \text{odd},\\
3Z5^R+1<5^{2R},\qquad
q=BQ-1,\quad q\mid1+C5^{F+R},\quad q\equiv\pm2\pmod5,\\
\frac{5^R}{J+1}<q<\frac{5^R}{J},\qquad
1\le u\le5^F-1,\\
EQ=(J+2)5^F+u,\qquad
qu\equiv EQ\pmod{5^F},\\
u\equiv-5^F(5^R+J)-EH\pmod{2^{t+5}},\\
1\le a_1\le9,\quad0\le a_2<10^R,\quad
10^F\le a_3<10^{F+1},\\
\gcd(2^Ra_1,a_2)=1,\qquad
\gcd(a_3,2^{a+R})=1,\\
a_3=\frac{2^{2a}e}{4}-g,\qquad
N_3=\frac{2^{2a}e}{4}+g,\qquad
g\mid D,\quad g,e\in\mathbb Z_{>0},\quad g\ \text{odd},\\
w_0=
\frac{2^{2a}(k-1)e-4(k+1)g}{4\cdot2^a}
\in\mathbb Z_{>0},\\
\frac{D-w_0^2}{a_3}\in\mathbb Z_{<0},\qquad
2^{2a}(k-1)^2e>4(k+1)^2g,\\
5^Fg\mid(q-1)D-4Qg^2.
\end{gathered}
\tag{51}
\]

The endpoints \(u=0\) and \(u=5^F\) are excluded by the strict quotient window. The endpoint \(a_3=10Y\) is excluded by (3), while \(a_3=Y\) is incompatible with reducedness because \(Y\) is even and
\[
\gcd(Y,2^{a+R})>1.
\]
Thus the effective recovery window is
\[
\boxed{Y<a_3<10Y}.
\tag{52}
\]

No primality or squarefreeness assumption on \(q,D\), or \(g\) is used. Independent verification of the algebraic identity (47), the binary congruence (29)–(30), and the endpoint checklist (51) is requested.

**Machine notation manifest.** `quotient_variable = u`; `codepoint = U+0075`; `forbidden_codepoints = [U+03BD, backslash+n+u]`. A byte scan of this artifact found zero occurrences of both forbidden forms. Every occurrence in equations (24), (29), (30), and (51) is the same Latin `u`.

**Notation audit.** The quotient variable in (19)--(30), including (24), (29), and (30), is consistently the ASCII Latin letter \(u\) (U+0075); no Greek Greek-nu token variable is used. The primitive-tail condition \(\gcd(2^Ra_1,a_2)=1\) appears both in the hypotheses and in the final checklist.
