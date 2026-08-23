Summary: The full three-mod-four square part of the canonical norm D divides the recovery parameter e, with exact recovered-factor valuation profiles.

Classification: NEW_LEMMA. Independent worker verification: VERDICT: CORRECT.

For either recovery sign, let
\[
D=(2^Ra_1)^2+a_2^2,
\qquad
L^2-cD=e^2.
\]
Fix a prime \(p\equiv3\pmod4\) and write
\[
v_p(D)=2s.
\]
The sum-of-two-squares valuation formula gives
\[
s=\min\{v_p(a_1),v_p(a_2)\}.
\]
Hence \(p^s\mid X_0\), so \(p^s\mid L\).

If \(v_p(e)<s\), then
\[
v_p(L^2-e^2)=2v_p(e)<2s,
\]
whereas
\[
L^2-e^2=cD
\]
has valuation at least \(2s\), a contradiction. Therefore
\[
\boxed{v_p(e)\ge s.}
\]

Define
\[
B=\prod_{\substack{p\mid D\\p\equiv3(4)}}p^{v_p(D)/2}.
\]
Then
\[
\boxed{B\mid L,\qquad B\mid e,\qquad B\mid c\delta.}
\]

For the recovered factors \(D=MN\), put
\[
u_p=v_p(\delta),\qquad q_p=v_p(e),\qquad q_p\ge s.
\]
If \(u_p\ge s\), then
\[
v_p(M)=v_p(N)=s,\qquad \min\{q_p,u_p\}=s.
\]
If \(u_p<s\), then \(p\mid c=m(hm-1)\), and exactly one of \(m,hm-1\) is divisible by \(p\). For the \(L_-\) orientation:

- if \(p\mid m\), then
  \[
  v_p(N)=u_p,\qquad v_p(M)=2s-u_p;
  \]
- if \(p\mid hm-1\), then
  \[
  v_p(M)=u_p,\qquad v_p(N)=2s-u_p.
  \]

The analogous sign-swapped recovered-factor formulas hold for \(L_+\).

The half-valuation bound is sharp at the reconstruction level. It does not imply \(v_p(e)\ge v_p(D)\), and division by \(B\) is not a canonical descent: digit windows, endpoints, and reducedness need not survive scaling.

Authority classes:
- FOUNDATIONAL_THEOREM: `FOUND-NT-QR-01` for the nonresidue of \(-1\) at primes \(p\equiv3\pmod4\).
- PROJECT_THEOREM: `PR6`, `SD6`, `GCU-2`, `GC2B-4`.
- LOCAL_PROOF: the valuation comparison, global product divisibilities, and recovered-factor profiles.