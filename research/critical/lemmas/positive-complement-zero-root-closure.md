Summary: The Q3>0, w0=0 branch is impossible by D=L a3^2 and reducedness.

<!-- VERIFIED_PROVENANCE {"artifact_sha256": "b3639288f8dd7767939098d3e305df7db48417a31b0811aca3de2a82067156eb", "campaign_id": "C2NEG-overnight-20260809", "origin_run_id": "GC2N-1-campaign-20260809-105746", "origin_step": 8, "origin_worker_index": 3, "parent_run_id": "GC2N-1-campaign-20260809-105746", "promotion_kind": "PREVIOUSLY_VERIFIED_NO_NEW_CALL", "run_id": "GC2N-1-continuation-20260811-022943", "verifier_sha256": "c85a47e04934cc9892701264ca9074b3e535f1a39b3049623b1be0ab75b33d82"} -->

Let
\[
d=2^a,\qquad P_0=ZH_1,\qquad K=k^2-1.
\]
Since \(w_0=0\), one has \(Q_3=D>0\) and
\[
P_0^2=KD.
\]
In particular \(P_0>0\) and \(K>0\).

The exact two-adic allocation gives
\[
v_2(K)=2a.
\]
Hence
\[
L:=\frac{K}{d^2}
\]
is a positive odd integer. Indeed, writing
\[
N=(J+1)5^F+u,
\]
the terminal factor formula gives
\[
k+1=2^AN,\qquad v_2(k-1)=1,\qquad v_2(N)=t+2,
\]
so
\[
2a=v_2(K)=A+t+3,
\]
and
\[
L=\frac{k-1}{2}\,\frac{N}{2^{t+2}}.
\]

Now \(Y=dZ\), so the recovery formulas imply
\[
Ka_3=YH_1=dZH_1=dP_0.
\]
Since
\[
\mathscr R_3=\frac{P_0}{d},
\]
we obtain
\[
Ka_3=d^2\mathscr R_3.
\]
Dividing by \(d^2\) yields the decisive identity
\[
\boxed{\mathscr R_3=L a_3.}
\]
Moreover,
\[
P_0^2=d^2\mathscr R_3^2=d^2LD,
\]
whence
\[
\mathscr R_3^2=LD.
\]
Substituting \(\mathscr R_3=La_3\) and cancelling \(L>0\) gives
\[
\boxed{D=L a_3^2.}
\]

Thus the recovered pair is never reduced:
\[
\gcd(a_3,\mathscr R_3)
=\gcd(a_3,La_3)
=a_3.
\]
Consequently, the retained reducedness requirement
\[
\gcd(a_3,\mathscr R_3)=1
\]
forces \(a_3=1\). Equivalently, if reducedness is expressed through \(\gcd(a_3,D)=1\), then \(D=La_3^2\) gives the same conclusion.

This contradicts even the weak upstream lower bound \(a_3\ge Y\). Indeed, \(1\le u<5^F\) implies \(F\ge1\), so
\[
Y=10^F\ge10.
\]

The endpoints are therefore accounted for exactly:

- The upstream-allowed endpoint \(a_3=Y\) satisfies
  \[
  \mathscr R_3=LY,\qquad \gcd(a_3,\mathscr R_3)=Y>1,
  \]
  so it fails reducedness. It is also incompatible with the required odd digit condition because \(Y\) is even.
- The endpoint \(a_3=10Y\) is excluded by the strict window \(a_3<10Y\); if inserted formally, it would likewise fail reducedness.
- When \(w_0=0\), \(X_+=X_-=P_0\), and for either recovery sign
  \[
  a_3=
  \frac{d\bigl((k+1)P_0-(k-1)P_0\bigr)}{2K}
  =\frac{dP_0}{K}.
  \]
  The complementary positivity inequality reduces to \(2P_0>0\). Hence the two signs give precisely the same recovery and cannot avoid the common-factor obstruction.

Therefore the entire \(Q_3>0,\ w_0=0\) subcase is uniformly contradictory. The terminal quotient congruences and odd-prime allocation are not needed beyond the exact valuation \(v_2(K)=2a\); no residual divisibility case remains.
