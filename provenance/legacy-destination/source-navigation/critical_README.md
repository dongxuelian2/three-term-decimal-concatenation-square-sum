# Three-Term Decimal Concatenation Square-Sum Problem

This repository records an ongoing mathematical proof project about whether there exist positive integers
\[
a_1,a_2,a_3,b_1,b_2,b_3
\]
with \(\gcd(a_i,b_i)=1\) for each \(i\), satisfying
\[
\left(\frac{a_1}{b_1}\right)^2+
\left(\frac{a_2}{b_2}\right)^2+
\left(\frac{a_3}{b_3}\right)^2
=
\left(
\frac{\operatorname{concat}(a_1,a_2,a_3)}
{\operatorname{concat}(b_1,b_2,b_3)}
\right)^2,
\]
where `concat` denotes ordinary decimal concatenation without leading zeroes.

The repository is a proof corpus and research index. It does not contain the Agent, harness, prompt, or run-history material used during the research.

## Current status

The global status is still open: no complete solution has been found, and the original problem has not been proved impossible.

The global authority is [`reports/proved_results_report_v3.md`](reports/proved_results_report_v3.md), with the shorter theorem registry at [`reports/proved_results_index_v3.md`](reports/proved_results_index_v3.md). The v3 record establishes T1–T18 and several branch results, including:

- the entire critical `O` template is closed by O1, as a project-internal exact machine-assisted theorem;
- `G_prim`, `gamma=1`, `A1` is closed by GA1-1;
- the exceptional binary `A2` room is closed by GE2-1;
- the low-`phi` `A2` region is reduced by GALMB-3 to a finite-state/block structure, but its moving-modulus residue remains open;
- the primitive `gamma=1`, `C3` branch is closed by GC3-1;
- `G` has substantial remaining open branches, `Q` remains open, and all four strict-layer families remain open.

The 2026-08-13 [`P0 frontier report`](docs/frontiers/critical_G_A2_high_phi_Fprimary_minus_P0_frontier_research_20260813.md) narrows, but does not close, the high-`phi` `G/A2/Fprimary-minus` `j=0` branch. The [`C2 frontier note`](docs/frontiers/c2_negative_frontier_20260811.md) records a later project-internal checkpoint that closes the `L+` orientation while leaving the `L-` residual open; it is a frontier note, not a replacement for the v3 global registry.

## Repository map

- [`reports/`](reports/) — global theorem report and quick index; start here.
- [`docs/foundations/`](docs/foundations/) — global layer and foundational campaign documents.
- [`docs/G/`](docs/G/) — `G`-template reductions and branch-specific campaigns.
- [`docs/lemmas/`](docs/lemmas/) — extracted mathematical lemma documents and terminal closure statements.
- [`docs/frontiers/`](docs/frontiers/) — current open-frontier notes and clean summaries of later partial progress.
- [`NOTATION.md`](NOTATION.md) — stable notation gathered from the current corpus.
- [`STATUS.md`](STATUS.md) — concise update dashboard.
- [`docs/dependencies.md`](docs/dependencies.md) — high-level dependency map.

## Recommended reading order

1. [`proved_results_index_v3.md`](reports/proved_results_index_v3.md)
2. [`proved_results_report_v3.md`](reports/proved_results_report_v3.md), especially the problem definition, T1–T18, status sections, and dependency table
3. [`NOTATION.md`](NOTATION.md)
4. foundational/global reductions in [`docs/foundations/`](docs/foundations/)
5. the common `G` reductions: scale divisor → primitive core/remainder → content dichotomy → terminal quotient
6. the relevant `G` branch campaign, followed by its linked lemma documents
7. the current frontier notes in [`docs/frontiers/`](docs/frontiers/)

## Status semantics

- **proved / closed** — a complete proof or a stated project-internal exact certificate is supplied in the linked document; machine-assisted closure is not presented as third-party reproduction.
- **reduced / classified** — a rigorous structural reduction or classification is established, but the remaining residual is not closed.
- **finite observation** — a bounded computation or experiment; it is not a global proof.
- **open** — no complete proof or counterexample is recorded.
- **frozen** — a result or status is treated as the current versioned baseline.
- **superseded / withdrawn** — retained only for history when a later document replaces or corrects its scope.

## Updating the corpus

For a substantive mathematical milestone, update the proof document first, then the theorem index, [`STATUS.md`](STATUS.md), and the global report if needed. See [`PROOF_UPDATE_WORKFLOW.md`](PROOF_UPDATE_WORKFLOW.md).

## Disclaimer

This repository contains an ongoing mathematical proof project. Results marked as proved or closed are intended to have complete proofs in the linked documents; other branches may remain provisional or open. The repository does not claim that the original problem has been solved.
