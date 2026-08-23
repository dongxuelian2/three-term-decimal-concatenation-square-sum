# C2 Negative Frontier Note

This document is a clean mathematical extraction from the 2026-08-11 C2 checkpoint. Internal campaign identifiers, provider/quota information, harness paths, usage counters, and run-history material have been omitted. The mathematical status is preserved at the evidence level stated by the source: these are project-internal verified reductions, not a global closure of the C2 branch.

## Outcome

The `L+` orientation of the former `R2` residual is closed. The remaining mathematical frontier is the `L-` orientation with `Q3 > 0` and `w0 > 0`.

## Closed branches

- `C0`: `Q3 = 0`.
- `R1`: `Q3 > 0`, `w0 = 0`.
- `R3`: `L+`, `Q3 < 0`, `v5(g) < v5(D)`.
- `R4`: `L+`, `Q3 < 0`, `v5(g) = v5(D) = 0`.
- `R2 / L+`: Archimedean dominance gives
  `Lambda > C*10^(F+1)`, contradicting the recovery inequality
  `Lambda <= C*delta-k < C*10^(F+1)`.

## Remaining `R2 / L-` system

All remaining states satisfy

```text
L^2-cD=e^2>0,
delta=(L-ke)/c,
D=(2^R*a1)^2+a2^2,
10^F<delta<10^(F+1),
M=m*delta+2e,
N=(hm-1)*delta+2he=hM-delta,
L-e=(hm-1)M,
L+e=mN.
```

Let

```text
B = product over p=3 (mod 4) of p^(v_p(D)/2).
```

### Nontrivial support, `B > 1`

The verified divisibility reductions are

```text
B divides L,
B divides e,
B divides c*delta,
C_B=B/gcd(B,c) divides delta.
```

The coefficient-supported residual `B divides c=m(hm-1)` remains. The exact gcd-aware allocation and the `p divides hm-1` valuation trichotomy narrow this residual but do not close it.

### Primitive support, `B = 1`

The verified congruence reductions are

```text
M and N have only 1 (mod 4) prime support,
delta = 3 (mod 4),
m = e = 1 (mod 4),
m = 1 (mod 8),
delta lies in exactly two classes modulo 8hk.
```

The remaining obstruction is the intersection of those dyadic classes with the canonical quadratic digit equation, quotient rows, moving five-adic congruence, strict endpoints, reducedness, scale recovery, and both reconstruction equations. The dyadic refinement does not by itself prove emptiness.

## Evidence boundary

The rejected local incompatibility argument involving `p divides m` is not promoted as a theorem. The C2 branch therefore remains open; this note records a narrowed frontier rather than a completed proof.
