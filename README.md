# Three-Term Decimal Concatenation Square-Sum Problem

This is the canonical repository for the project. It is a proof corpus, not the
Research Agent, its runtime, or its run history.

## Problem

For positive integers `a_i,b_i` with `gcd(a_i,b_i)=1`, let `concat` be ordinary
decimal concatenation without leading zeroes. The question is whether

\[
\sum_{i=1}^{3}\left(\frac{a_i}{b_i}\right)^2
=
\left(\frac{\operatorname{concat}(a_1,a_2,a_3)}
{\operatorname{concat}(b_1,b_2,b_3)}\right)^2
\]

can hold. The global problem remains open. The theorem record is
[`research/foundations/results/theorem-index.md`](research/foundations/results/theorem-index.md),
and the detailed report is
[`research/foundations/results/proved-results.md`](research/foundations/results/proved-results.md).

## Canonical research tree

Directory hierarchy expresses mathematical containment; filenames express local
mathematical meaning. Proof maturity and historical workflow are metadata, not
parallel mathematical trees.

- [`research/foundations/`](research/foundations/) — definitions, theorem records, and foundational reductions.
- [`research/exact-lift/`](research/exact-lift/) — the common exact-lift and recovery framework.
- [`research/denominator-structure/`](research/denominator-structure/) — denominator and DD reductions.
- [`research/a1/`](research/a1/) — the A1 branch, with forward, backward, J2, and moving-profile subproblems.
- [`research/templates/g/`](research/templates/g/) — the critical G-template branches and their lemmas.
- [`TREE.md`](TREE.md) and [`INDEX.md`](INDEX.md) — deterministic navigation generated from this tree.

Results, reusable failures, incomplete attempts, computations, and literature
audits belong near the node they concern. A failure is scope-qualified negative
knowledge about a route; it is not automatically a proof that the original
problem has no solution.

## Historical names and provenance

Campaign, round, strict-layer, and numbered-series names are historical aliases,
not active canonical names. The source-only material is preserved byte-for-byte
under [`research/archive/strict-layer-proof-research/`](research/archive/strict-layer-proof-research/).
That directory is an intentionally frozen archival boundary; its old names are
kept so that provenance remains recoverable. The migration map, source commits,
hashes, relationships, and aliases live under [`provenance/`](provenance/).
Git retains the complete source commit graph, including the imported source
history and the `legacy-strict-layer-final` tag.

## Updating the corpus

For a new mathematical result, update the closest canonical node, then update
the theorem/status record and links. Keep local notation scoped to its defining
document; see [`NOTATION.md`](NOTATION.md) and
[`PROOF_UPDATE_WORKFLOW.md`](PROOF_UPDATE_WORKFLOW.md).

Regenerate navigation with:

```text
python tools/update-research-index.py
```

The generator is deterministic and uses no database, embedding service, or
agent runtime.
