# Current Research Status

Last updated: 2026-08-13

## Global status

The original three-term decimal concatenation square-sum problem remains open. The current corpus contains rigorous foundational reductions, several closed templates or subbranches, and substantial unresolved residual systems. No complete solution or global impossibility proof is recorded.

## Proven / closed

- T1–T18: foundational integerization, denominator, valuation, digit-layer, critical-layer, and strict-layer reductions; see [`proved_results_report_v3.md`](reports/proved_results_report_v3.md).
- O1: the entire critical `O` template has no candidate, with project-internal exact machine-assisted certificates; external independent rerun remains pending.
- GA1-1: `G_prim`, `gamma=1`, `A1` is closed.
- GE2-1: the exceptional binary `A2` room is closed.
- GC3-1: primitive `gamma=1`, `C3` is closed.

## Reduced but still open

- `A2`, low `phi`: GALMB-3 gives a uniform finite-block/involution and unique finite exponent-segment structure; the moving-modulus and discrete-log residue remains.
- `A2`, high `phi`, `Fprimary-minus`: the `P0`, `P1`, and zero-quotient families are unified into an inverse–Bezout tower; the ratio-length forbidden-word obstruction remains.
- `C1` and `C2` rooms in the primitive `gamma=1` `C` system remain open.
- The critical `Q` system remains at its moving-coefficient reduction.
- All four strict-layer families still contain open infinite branches.

## Current frontier

- [`critical_G_A2_high_phi_Fprimary_minus_P0_frontier_research_20260813.md`](docs/frontiers/critical_G_A2_high_phi_Fprimary_minus_P0_frontier_research_20260813.md) records the latest high-`phi` `P0` narrowing: at most three candidate `F` values and at most six `(F,J)` pairs for fixed legal `(a,t)`, but the branch is still open.
- [`c2_negative_frontier_20260811.md`](docs/frontiers/c2_negative_frontier_20260811.md) records a clean mathematical extraction from a later C2 checkpoint: the `L+` orientation is closed and the exact `L-` residual remains. This has not replaced the v3 theorem registry.

## Recently completed

- 2026-08-13 — Narrowed the open high-`phi` `G/A2/Fprimary-minus/P0` branch without changing its open status.
- 2026-08-11 — Recorded the C2 `L+` closure and the remaining `L-` frontier as a clean research note; the original mixed run report is intentionally excluded.
- 2026-08-07 — Current global v3 report froze O1, GA1-1, GE2-1, GALMB-3, and GC3-1 in its stated project-internal proof categories.

## Scope notes

The v3 report remains the global theorem/status authority. Finite computations are kept at their stated evidence level and are not promoted to proofs. No Agent source, prompt, harness, quota record, credential, or run trace belongs in this repository.
