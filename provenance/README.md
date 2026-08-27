# Provenance and migration records

This directory is the authoritative migration ledger for the consolidation of
the canonical corpus and the archived strict-layer source. It records source
paths, hashes, duplicate relationships, dispositions, aliases, and unresolved
references without changing the mathematical claims in the research files.

- [`MIGRATION_MAP.tsv`](MIGRATION_MAP.tsv) accounts for every source path at the
  final source `main` commit, plus the deleted workflow recovered from history.
- [`ALIASES.tsv`](ALIASES.tsv) is generated from the migration map and resolves
  historical source and pre-migration destination paths.
- [`SOURCE_REPOSITORIES.md`](SOURCE_REPOSITORIES.md) records repository roles,
  commits, refs, and the preservation policy.
- [`UNRESOLVED_MIGRATION.md`](UNRESOLVED_MIGRATION.md) records references that
  were known to the source export but whose original bytes were unavailable.

The old destination manifests remain under
[`legacy-destination/`](legacy-destination/) as historical audit material. They
are not a competing canonical index. Regenerate the deterministic navigation
and alias files with:

```text
python tools/update-research-index.py
```
