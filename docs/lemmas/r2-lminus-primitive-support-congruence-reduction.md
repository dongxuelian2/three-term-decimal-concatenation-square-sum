Summary: The primitive-support L-minus branch is reduced to all-prime support conditions and a strengthened progression modulo 4k.

Classification: BRANCH_CLOSURE. Independent worker verification: VERDICT: CORRECT.

Retain
\[
M=m\delta+2e,\qquad
N=(hm-1)\delta+2he=hM-\delta,
\]
\[
D=MN,\qquad
c=m(hm-1),\qquad
k=2hm-1,\qquad
L=c\delta+ke.
\]
Assume
\[
B=1,
\]
so \(D\) has no prime divisor congruent to \(3\pmod4\).

Both \(M,N\) are positive odd divisors of \(D\). Thus every prime divisor of either factor is \(1\pmod4\), giving
\[
M\equiv N\equiv1\pmod4.
\]
Since \(4\mid h\) and \(N=hM-\delta\),
\[
\boxed{\delta\equiv3\pmod4.}
\]

In the inherited tail states \(4\mid L\). Combining
\[
L=c\delta+ke
\]
with \(M\equiv1\pmod4\) then gives
\[
\boxed{m\equiv e\equiv1\pmod4.}
\]

For every prime \(p\equiv3\pmod4\), the exact surviving configurations satisfy:

1. If \(p\mid\delta\), then \(p\nmid e\).

2. If \(p\mid e\), then
   \[
   p\nmid\delta,\qquad p\nmid m(hm-1).
   \]

3. If \(p\nmid e\delta\), then
   \[
   e\delta^{-1}\not\equiv-\frac m2,
   \qquad
   e\delta^{-1}\not\equiv-\frac m2+(2h)^{-1}
   \pmod p.
   \]

The finite progression is consequently refined to
\[
\boxed{
10^F<\delta<10^{F+1},\qquad
\delta\equiv-d^2L\pmod k,\qquad
\delta\equiv3\pmod4,
}
\]
which is one residue class modulo \(4k\).

This does not close \(B=1\). Reconstruction-level examples show that primitive support, the square equation, and a sum-of-two-squares representation can coexist; the remaining canonical scale, quotient, digit, endpoint, reducedness, and reconstruction conditions are essential.

Authority classes:
- FOUNDATIONAL_THEOREM: `FOUND-NT-QR-01`.
- PROJECT_THEOREM: `PR6`, `SD6`, `GCU-2`, `GC2B-4`.
- LOCAL_PROOF: support congruences, all-prime exclusions, and progression refinement.