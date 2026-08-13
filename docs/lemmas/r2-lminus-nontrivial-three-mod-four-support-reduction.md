Summary: In the L-minus branch with nontrivial three-mod-four support, a valuation-deficient subbranch is closed and the exact surviving digit divisibility is identified.

Classification: BRANCH_CLOSURE. Independent worker verification: VERDICT: CORRECT.

Assume the \(L_-\) finite-digit system and define
\[
B=\prod_{\substack{p\mid D\\p\equiv3(4)}}p^{s_p},
\qquad
s_p=\frac{v_p(D)}2.
\]
By [[lemmas/r2-global-three-mod-four-valuation-support]],
\[
B\mid L,\qquad B\mid e,\qquad B\mid c\delta.
\]

Therefore the complete valuation-deficient subbranch
\[
\boxed{
B>1,\qquad
\exists p\equiv3\pmod4,\ p\mid D:
\quad v_p(c\delta)<\frac{v_p(D)}2
}
\]
is empty.

Define
\[
C_B=\frac{B}{\gcd(B,c)}
=
\prod_{\substack{p\mid D\\p\equiv3(4)}}
p^{\max\{s_p-v_p(c),0\}}.
\]
Every surviving \(B>1\) candidate satisfies
\[
\boxed{C_B\mid\delta.}
\]

Together with the finite-progression congruence
\[
\delta\equiv-d^2L\pmod k,
\]
this gives one compatible residue class modulo
\[
\operatorname{lcm}(k,C_B).
\]
The modulus is strictly strengthened exactly when
\[
C_B/\gcd(C_B,k)>1.
\]

No descent by \(B\) is authorized. The exact unresolved complement is
\[
\boxed{
B>1,\qquad
v_p(\delta)\ge
\max\left\{0,\frac{v_p(D)}2-v_p(c)\right\}
\quad
\text{for every }p\equiv3\pmod4,\ p\mid D.
}
\]
In particular, the coefficient-supported subbranch \(B\mid c\) remains open.

Authority classes:
- FOUNDATIONAL_THEOREM: `FOUND-NT-QR-01`.
- PROJECT_THEOREM: `PR6`, `SD6`, `GCU-2`, `GC2B-4`.
- LOCAL_PROOF: valuation-deficient closure, \(C_B\mid\delta\), CRT refinement, and descent audit.