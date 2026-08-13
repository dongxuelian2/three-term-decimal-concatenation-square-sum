Summary: The Q3=0 branch is impossible by an exact two-adic divisibility contradiction.

<!-- VERIFIED_PROVENANCE {"artifact_sha256": "a8c16340d18a7e96db2e2b2679e783b854adda53789bd7767f06e560c6524ab9", "campaign_id": "C2NEG-overnight-20260809", "origin_run_id": "GC2N-1-campaign-20260809-105746", "origin_step": 8, "origin_worker_index": 2, "parent_run_id": "GC2N-1-campaign-20260809-105746", "repair_kind": "FOLLOWUP_LOCAL_MINOR", "run_id": "GC2N-1-continuation-20260811-022943", "verifier_sha256": "39952cfe3919296ecc081c48c60589e9f0a26d97c8ed6cdba7af6678af5e5cc3"} -->

### LOCAL_PROOF

Assume the genuine negative-frontier hypotheses:

\[
a,t,R\in\mathbb Z,\qquad a\ge4,\qquad t=v_2(R),\qquad a\ge t+4,
\]

\[
A=2a-3-t,\qquad F=a+A,\qquad
Y=10^F,\qquad Z=2^A5^F,
\]

and the exact tail inequality

\[
10^{3a-4-t}\le 2^{a+R}<10^{3a-3-t}.
\]

The exact-tail normal form gives

\[
R>5a
\]

and the parity condition

\[
F+R\equiv1\pmod2,
\]

equivalently,

\[
t=0\Rightarrow a\ \text{odd},\qquad
t\ge1\Rightarrow a\equiv t\pmod2.
\]

The decimal digits satisfy

\[
1\le a_1,a_2\le9.
\]

The third block is positive and lies in the half-open digit range

\[
Y\le a_3<10Y,
\]

with the reducedness condition

\[
\gcd(a_3,2^{a+R})=1.
\]

The lower endpoint \(a_3=Y\) is impossible because \(F\ge1\), so \(2\mid Y\), whereas reducedness requires \(a_3\) odd. The upper endpoint \(a_3=10Y\) is excluded by the strict upper digit bound; it would also violate reducedness. Thus neither endpoint supplies an exceptional case.

Since \(t\le a-4\),

\[
\boxed{A=2a-3-t\ge2a-3-(a-4)=a+1\ge5.}
\]

Moreover,

\[
A\le2a-3<5a<R,
\]

so

\[
\boxed{R>A.}
\]

Let

\[
H_1=a_1 10^R+10a_2,\qquad
D=(2^Ra_1)^2+a_2^2.
\]

Both are positive. Put \(d=2^a\), \(K=k^2-1\), and take \(w_0\ge0\); allowing a signed square root merely interchanges the two recovery signs. A complete recovery means, in particular, that the displayed recovery variables are integral.

A complete recovery with sign \(\varepsilon\in\{+1,-1\}\) satisfies

\[
L_\pm=ZH_1\pm kw_0,
\]

\[
L_\varepsilon=(K/d)a_3,\qquad
L_{-\varepsilon}=d\mathscr R_3,
\]

and

\[
Q_3=D-w_0^2=a_3\mathscr R_3.
\]

Retain the inherited complete-frontier identity \(q=k+Z\), with \(k,Q\in\mathbb Z\) and \(Q\ge1\); this identity is an explicit hypothesis here, not a new conclusion of the factor-quotient lemma.

The factor-quotient character gives the terminal factor

\[
q=2^{2a}Q-1=k+Z.
\]

Hence \(q\) is odd, while \(Z\) is even, and therefore

\[
\boxed{k\ \text{is odd}.}
\]

Assume now that \(Q_3=0\). Since \(a_3>0\),

\[
\mathscr R_3=0,
\]

and consequently

\[
L_{-\varepsilon}=0.
\]

The case \(w_0=0\) is impossible already from

\[
w_0^2=D=(2^Ra_1)^2+a_2^2>0.
\]

Thus \(w_0>0\). No sign assumption on \(k\) is needed. From
\[
L_{-\varepsilon}=0
\]
one obtains directly
\[
kw_0=\varepsilon ZH_1\in\{ZH_1,-ZH_1\},
\]
for either recovery sign \(\varepsilon\in\{+1,-1\}\). Hence
\[
k^2w_0^2=Z^2H_1^2.
\]

Squaring and using \(w_0^2=D\) gives the required equality

\[
\boxed{k^2D=Z^2H_1^2.}
\]

Because \(k\) is odd and \(2^{2A}\mid Z^2\), this equality implies

\[
2^{2A}\mid D.
\]

Since \(R>A\),

\[
2^{2A}\mid (2^Ra_1)^2.
\]

Subtracting this term from \(D\) yields

\[
2^{2A}\mid a_2^2,
\]

hence

\[
2^A\mid a_2.
\]

But \(A\ge5\), so \(2^A\ge32\), whereas \(1\le a_2\le9\). This is impossible.

Therefore no complete reduced recovery on the genuine negative frontier can satisfy

\[
\boxed{Q_3=0.}
\]
