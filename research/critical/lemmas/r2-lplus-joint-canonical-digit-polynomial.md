Summary: The L-plus progression coupled to the same canonical digits yields an exact quadratic digit identity and a sum-of-two-squares norm sieve, but no branch closure yet.

Classification: NEW_LEMMA. Worker verification: VERDICT: CORRECT.

In the canonical \(L_+\) residual retain
\[
D=(2^Ra_1)^2+a_2^2,\qquad
H_1=a_1\,10^R+10a_2,
\]
\[
L=\frac{10^FH_1}{2^{2a}},\qquad
C=m(hm-1)\delta,\qquad k=2hm-1,
\]
\[
e=\frac{C-L}{k},\qquad
1\le e<\frac{C}{2k}.
\]
Define
\[
N=m\delta-2e,\qquad
M=(hm-1)\delta-2he.
\]
Then
\[
D=NM
\]
and
\[
k^2D=(2L+m\delta)
\bigl(2hL-(hm-1)\delta\bigr).
\]

The simultaneous canonical equations imply
\[
\boxed{
5^{2R}D=(H_1-10a_2)^2+5^{2R}a_2^2.
}
\]
Equivalently, writing
\[
B=a_1\,10^{R-1}+a_2
\]
and eliminating \(a_2=B-10^{R-1}a_1\), a candidate must satisfy the exact quadratic digit equation
\[
\boxed{
(4^R+10^{2R-2})a_1^2
-2B10^{R-1}a_1+B^2-D=0.
}
\]

Consequently, for every prime \(p\equiv3\pmod4\),
\[
\boxed{v_p(D)=v_p(M)+v_p(N)\ \text{is even}.}
\]
This condition concerns the total valuation and remains valid when \(M,N\) share factors. No factorwise coprimality is assumed.

All complete quotient conditions, canonical digit intervals, strict recovery windows, authorized reducedness predicates, and reconstruction equations remain mandatory. The identities above do not themselves close \(L_+\).

Authority classes:
- PROJECT_THEOREM: GP3, PR6, SD6, GCU-2, GC2B-4 for the inherited quotient, recovery, and digit contracts.
- LOCAL_PROOF: the coupled digit polynomial and total-valuation norm sieve.