# Notation

This file records notation already stable in the current proof corpus. It is a navigation aid, not a redesign of the mathematical system. Local record notation may have a narrower scope; the defining document takes precedence.

## Original problem and concatenation

- `concat(u,v,w)` is ordinary decimal concatenation without leading zeroes.
- `a_i, b_i` are positive integers with `gcd(a_i,b_i)=1`.
- `A = concat(a_1,a_2,a_3)`, `B = concat(b_1,b_2,b_3)`.
- `alpha_i = ell(a_i)`, `beta_i = ell(b_i)`, `delta_i = alpha_i - beta_i`.
- `Delta = delta_1 + delta_2 + delta_3`, `m = max_i delta_i`.
- `q_i = a_i/b_i`, `R = A/B`.

## Common denominator and kernel

- `L = lcm(b_1,b_2,b_3)`.
- `x_i = L a_i / b_i`, `t = L A / B`.
- `G = gcd(A,B)`.
- `H = gcd(B,L)`, `B = H M`, `L = H N_L`, with `gcd(M,N_L)=1`.

## Critical-template notation

- `n = beta_2`, `T = 10^n`, `S = 10^(beta_3)`.
- `a = a_1`, `b = b_1`, `F = aT + 10a_2`, `D = bT + b_2`.
- `s = b b_2`, `N_0 = (a b_2)^2 + (b a_2)^2`.
- The critical templates are named `O`, `G`, and `Q`; these labels are not interchangeable with the `G = gcd(A,B)` notation and must be read in context.

## G-template notation

- `G_prim` denotes the primitive/core layer in the `G` template.
- `gamma` is the content/scale parameter used by the `G` branch records; `gamma=1` is a major frozen scope.
- `A1`, `A2`, `B`, `C1`, `C2`, `C3`, and `C5` are branch labels whose exact scope is defined by the linked campaign documents.
- `phi` (often written `\varphi`) is the five-adic depth parameter in the `A2` branch records.
- `F_+`, `F_{P-}`, and `F_{E-}` are high-`phi` subfamilies; `P0` and `P1` are positive-quotient families.

## Valuations and arithmetic

- `v_p(x)` is the `p`-adic valuation.
- `ord_r(10)` is the multiplicative order of `10` modulo `r` when defined.
- `N_L` is the denominator-kernel factor in the common-denominator decomposition; `N_0` is the critical quadratic-form constant.
- In the critical report, `rho` denotes the critical discriminant integer; in local campaign documents a symbol may have a narrower scope.

## Scope warning

Some historical documents use local symbols such as `m`, `M`, `R`, `q`, `r`, `k`, or `h` differently from the global report. Do not force a global identification across documents; use the local definitions and the dependency links.
