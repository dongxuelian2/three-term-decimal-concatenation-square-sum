# Canonical Mathematical Corpus

Generated corpus navigation and provenance metadata for the unified mathematical corpus.

## Canonical navigation

- Global v3 index: [reports/global/proved_results_index_v3.md](reports/global/proved_results_index_v3.md)
- Global v3 report: [reports/global/proved_results_report_v3.md](reports/global/proved_results_report_v3.md)
- Critical source frontier: [research/critical/frontiers/critical_G_A2_high_phi_Fprimary_minus_P0_frontier_research_20260813.md](research/critical/frontiers/critical_G_A2_high_phi_Fprimary_minus_P0_frontier_research_20260813.md)
- Strict source status: [reports/strict/current_research_status_v3.md](reports/strict/current_research_status_v3.md)
- Strict current foundation document: [research/strict/foundation/strict_layer_unified_exact_lift_campaign.md](research/strict/foundation/strict_layer_unified_exact_lift_campaign.md)
- Strict 105 continuation report: [research/strict/campaigns/105/local/105_V3_CONTINUATION_REPORT.md](research/strict/campaigns/105/local/105_V3_CONTINUATION_REPORT.md)
- Source equivalence: [manifests/SOURCE_EQUIVALENCE_MANIFEST.tsv](manifests/SOURCE_EQUIVALENCE_MANIFEST.tsv)
- Public migration manifest: [manifests/MIGRATION_MANIFEST.tsv](manifests/MIGRATION_MANIFEST.tsv)

## Mathematical boundary

- GLOBAL_PROBLEM=OPEN
- STRICT_A1=OPEN
- 105_CONTINUATION=OPEN

Critical and strict source scopes remain distinct. Closed sub-results and bounded searches stay scope-qualified; no corpus navigation promotes them to global closure.

The two source-repository copies of each v3 proved-results document have one canonical global physical target under `reports/global`. This is provenance consolidation, not a ranking of critical over strict or strict over critical.

## Provenance and safety

Source-backed files are copied byte-for-byte. Canonical hashes normalize only CRLF/CR line endings to LF for equivalence checks. The exact-text aliases, the global v3 source pair, and the strict initial historical pair are recorded in `SOURCE_EQUIVALENCE_MANIFEST.tsv`.

The source README/STATUS reference to the locally present but remote-missing critical P0 frontier is represented by the corpus frontier target and the token `LEGACY_REMOTE_BROKEN_REFERENCE_REPAIRED_BY_MIGRATION`. This repairs corpus navigation only; it does not alter either source repository.
