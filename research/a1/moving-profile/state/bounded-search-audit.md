# 105 v3 Stage 04 — Bounded Production-Root Search Audit

Stage metadata (YAML):

    Stage ID: 105-V3-S04
    Objective: "Run a bounded exact reconnaissance after carrying the full R28 support package into the R40 production-native root search."
    Input Artifacts:
      - 105_V3_STAGE_02_R40_QUOTIENT_AND_SUPPORT_AUDIT.md
      - 105_V3_STAGE_03_SOURCE_ROOM_SUCCESSOR_AUDIT.md
      - 105_V3_R40_quotient_audit.py
      - 105_V3_R40_small_root_search.py
      - archive-by-series/90-105/105-R40-FINAL-FAILURE-REPORT.md
    Research Obligation:
      Question: "Within an explicit finite scope, do any primitive, R28-shape/support-admissible production roots reach the raw source room?"
      Why this matters: "The search separates the first source-room obstruction from the earlier primitive/support failures and supplies a reproducible continuation certificate."
      Current evidence: "R39 has a primitive/support-complete root with empty source room; R40 has raw source room but fails primitive/support."
      Expected resolution: "A bounded count and first-failure ledger, never a universal theorem."
    Method: "Enumerate primitive positive sphere packets, apply selector and exponent-image filters, solve exact production incidence for K=10^k, retain R28 shape/support gates, then apply exact integer source-room floors."
    Status: COMPUTATIONAL

## Scope

The run used the workspace Python runtime with

\[
Q_0\le300,\qquad 1\le n_3\le3,\qquad 1\le q\le4.
\]

The exact invocation was:

    python -B -c "import runpy; m=runpy.run_path('105_V3_R40_small_root_search.py'); m['run'](300,3,4)"

All arithmetic was integer-exact. The search retained primitive sphere,
selector, exponent synchronization, R40 divisibility, R28 shape, R28 support,
and the exact source-room floor/ceiling test. It did not claim global
completeness and did not execute terminal reconstruction for roots that failed
before source completion.

## Replayed counts

    PACKETS=18270
    SELECTOR_STATES=3521885
    PRODUCTION_ROOTS=7
    R40_DIV_FAILURES=0
    R28_SHAPE_ROOTS=3
    R28_SUPPORT_ROOTS=1
    ROOTS_WITH_U0_GT_1=4
    SOURCE_ROOM_ROOTS=0
    SOURCE_ROOM_ROOTS_U0_GT_1=0

The unique R28-support survivor in this scope is

\[
(P_1,P_2,P_3,Q_0)=(24,52,159,169),
\]

with

\[
(u_0,A,W,C_2,C_3,g_0,a,\mu,s)=(1,3,4,13,53,12,1,2,1),
\]

\[
(n_2,n_3,m_2,m_3,g,k)=(2,1,1,1,0,1),
\qquad
(U_{\rm lo},U_{\rm hi})=(1,0).
\]

Thus the first source-room failure in the searched support-complete corpus is
the exact integer obstruction \(U_{\rm lo}>U_{\rm hi}\).

## Result

Result metadata (YAML):

    New Result: "The bounded scope contains 7 production roots, 1 R28-support survivor, and 0 raw source-room roots."
    Evidence: "105_V3_R40_small_root_search.py, rerun with Q0<=300, n3<=3, q<=4."
    Derivation: "Enumerate primitive sphere packets, apply the synchronized selector/support filters, solve production incidence exactly, and test Ulo<=Uhi."
    Status: COMPUTATIONAL
    Remaining Gap: "No global digit-cell bound or source/support incompatibility has been proved."
    Next Action: "Search for a source-native invariant or extend the exact scope only after preserving the same first-failure predicate."

## Research State Update

    Research State Update:
      Previous State: "The source/support intersection was open after the R40 quotient audit."
      New Observation: "In the declared bounded scope, the only R28-support survivor has empty raw source room; no candidate reaches successor."
      Changed Assumption: "None globally. The result is a bounded computational certificate only."
      New Open Obligation: "Cover all digit cells by a proof-level source/support incompatibility or obtain a first support-complete source point."
      Reason: "Finite no-hit data cannot establish universal Strict A1 unliftability."
