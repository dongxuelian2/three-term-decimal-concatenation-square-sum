# Source repositories and consolidation provenance

This record describes the one-time consolidation into the canonical repository.
It is provenance metadata, not a mathematical result and not an upgrade of any
evidence level.

## Canonical destination

- Repository: [`dongxuelian2/three-term-decimal-concatenation-square-sum`](https://github.com/dongxuelian2/three-term-decimal-concatenation-square-sum)
- Default branch: `master`
- Pre-migration HEAD: `0188fd0badc472ebbfda9991d76f42e7b2b7f2d8`
- Migration branch: `research-corpus-cleanup`
- History-preservation merge: `b37b708f48cab716f923b0bc5d40f82597f69c27`

The migration branch started from the destination HEAD above. The
history-preservation merge has the destination history as its first parent and
`strict-layer-proof-research` `main` as its second parent.

## Consolidated source

- Repository: [`dongxuelian2/strict-layer-proof-research`](https://github.com/dongxuelian2/strict-layer-proof-research)
- Branch: `main`
- Final source HEAD: `912fb4b67419d69c8c7d805b7fd2fcadd26e9a7a`
- Full-archive branch also inspected: `codex/import-complete-archive`
- Role: strict-layer foundation, backward/global, denominator, A1, state,
  computation, and historical stage material.
- Pre-migration state: archived, clean, and not mutated by this consolidation.

The source `main` tree contains 730 tracked paths and 692 raw content groups.
The migration map accounts for all 730 current paths. Source-only content was
copied once per raw content group under the frozen archive boundary, with one
source-only computation promoted to its active A1 computation node; duplicate
paths are mapped to that representative or to an active canonical file. A
deleted source workflow is also preserved as a history-only row and file from
commit `54aba05`.

## Preservation and deletion policy

The clones used for this work were full, dedicated clones outside the Research
Agent workspace. The source commit graph is imported without squashing and is
reachable from the canonical history. The durable tag
`legacy-strict-layer-final` is intended to point at the final source HEAD after
publication.

The source repository remains archived until the final validation gates pass:
hash/accounting, link and naming checks, deterministic index regeneration,
Git object integrity, branch/tag publication, and a fresh GitHub clone. Only
then may the archived source repository be deleted. The canonical migration
map and source tag are the recovery records for that operation.
