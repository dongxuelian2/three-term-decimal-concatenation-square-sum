# 105 v3 Research-State Reconstruction Report

> Recovery date: 2026-08-21 (Asia/Shanghai)  
> Repository: `https://github.com/dongxuelian2/strict-layer-proof-research`  
> Recovered checkout: commit `ff3c281` (`Import complete strict-layer proof archive`)  
> Scope: 105 continuation, Strict Layer (A_1)-only  
> Evidence rule: an archived assertion is not inherited as a theorem until its later audit and failure reports are checked.

## 1. Research State

### 1.1 Current research goal

The parent problem is to decide whether there exist positive decimal blocks

\[
\gcd(a_i,b_i)=1,
\qquad
\left(\frac{a_1}{b_1}\right)^2+
\left(\frac{a_2}{b_2}\right)^2+
\left(\frac{a_3}{b_3}\right)^2
=
\left(\frac{\operatorname{concat}(a_1,a_2,a_3)}
{\operatorname{concat}(b_1,b_2,b_3)}\right)^2,
\]

with no leading zero in any block. The global parent problem is still **OPEN**:
the archive does not prove either existence or nonexistence.

The 105 continuation is narrower. It asks whether the faithful source-completed
Strict (A_1) branch has a legal lift to actual decimal blocks. The active
decision is therefore

\[
\boxed{\text{Strict }A_1\text{ unliftability, or a full Strict }A_1\text{ witness}.}
\]

### 1.2 Strict (A_1) definition recovered from the archive

The label `Strict Layer — (A_1)-only` is a branch label, not a relaxed
projection. A faithful state must retain all of the following:

1. a positive primitive sphere packet
   \[
   \pi=(P_1,P_2,P_3,Q_0),\qquad
   P_1^2+P_2^2+P_3^2=Q_0^2,qquad
   \gcd(P_1,P_2,P_3,Q_0)=1;
   \]
2. the exact Smith/support selectors and the moving decimal profile;
3. the source affine section: a positive integer common radial scale \(U\),
   coprimality, source congruences, and the actual digit rooms;
4. the powers-of-ten exponent image and the actual word placement;
5. the exact MASTER, denominator window, successor, and terminal predicates;
6. reverse reconstruction to the original (a_i,b_i), including individual
   reducedness.

The canonical source decomposition recovered in R1--R2 is

\[
\mathbf a=U\mathbf C_x,
\qquad \gcd(C_1,C_2,C_3)=1,
\]

where \(U\) is intrinsic common numerator content, not an optional projective
scale. Ambient sphere, Gaussian, determinant, Smith, or valuation statements
are not Strict (A_1) results unless the same source section is restored.

### 1.3 Frozen exact state

The following formulas are the current interface. They are frozen inputs, not
new derivations in this recovery report.

#### Primitive sphere and selectors

\[
M_0=u_0AW,
\qquad g_0=\gcd(M_0,P_1),
\qquad M_0=g_0a,
\qquad P_1=g_0\mu s,
\qquad \gcd(a,\mu s)=1,
\]

\[
P_2=u_0WC_2,
\qquad P_3=u_0AC_3.
\]

The primitive packet and these selectors are necessary but not sufficient for
a source lift.

#### Smith/support and residual denominator shell

With \(T_3=Q_0-P_3\) and \(Y=10^{n_3}\),

\[
\lambda_z=\frac{Y}{\gcd(Y,WT_3)},
\qquad
\Lambda=\operatorname{lcm}(\mu,\lambda_z)=\mu\tau,
\]

and, after the exact compatibility gates,

\[
z=\Lambda q,
\qquad
\gcd(q,F)=1,
\qquad
F=\operatorname{rad}(R_1C_2C_3).
\]

For a fixed architecture, the denominator residual interval is

\[
Q_-\le q\le Q_+,
\qquad
Q_{\rm master}=\left\lfloor\frac{Q_0-1}{b_1D}\right\rfloor,
\qquad
Q_*=\min(Q_+,Q_{\rm master}).
\]

The master-refined terminal predicate recovered in R30/R35 is

\[
\boxed{\exists U\in\mathcal U_0\;\exists q\in[Q_-,Q_*]\cap\mathbb Z_{>0}
\quad \gcd(q,FU)=1.}
\tag{TP}
\]

Here \(\mathcal U_0\) is not merely a real interval: it includes the exact
source digit room, the periodic source selector, all completed-source gates,
and \(\gcd(U,V_0)=1\).

#### Source interval and successor

On regular source strata,

\[
L=\max\left(\frac{10^{n_2-1}}{C_2},\frac{10^{n_3-1}}{C_3}\right),
\qquad
R_{\rm src}=\min\left(\frac{10^{n_2}}{C_2},\frac{10^{n_3}}{C_3}\right).
\]

With native period \(M_U=\operatorname{lcm}(P_0,V_0)\), the authoritative
successor is formed from the integer edge

\[
U_{\rm lo}=\lceil\max(L,1)\rceil,
\qquad
U_{\min}=U_{\rm lo}+\min_r[r-U_{\rm lo}]_{M_U},
\]

and source nonemptiness is \(U_{\min}<R_{\rm src}\), with the documented
strict-floor correction on decorated open strata. The raw \(L\)-based modular
delay is not the authoritative successor formula.

The corrected simultaneous source/denominator/master locus is

\[
\boxed{
\mathscr T=
\{\mathcal U_0\ne\varnothing,
Q_-≤Q_+,
Q_-b_1D<Q_0\}.
}
\tag{SIM}
\]

#### Production-native root system

After exponent synchronization, R39 freezes

\[
L_{\rm src}=a10^{n_2+n_3},
\]

\[
B_{\rm src}=\mu(W+A10^{m_3})+a10^{m_2+m_3},
\]

\[
C_{\rm src}=\mu g_0a(C_3+10^{n_3}C_2),
\qquad
L_{\rm src}P_1=B_{\rm src}Q_0-C_{\rm src},
\]

with the primitive sphere equation. R39 proves \(B_{\rm src}<L_{\rm src}\),
so the linear \(\mathcal A_N=0\) branch is globally extinct, while the
quadratic branch is not empty in the ambient production system.

R28 already proves the same support-divisibility theorem in the TC1 chart,
with \(m_3=n+g\):

\[
u_0\mid W+A10^{n+g},
\qquad
(u_0,A)=1,
\qquad
\gcd(u_0,W)=\gcd(u_0,10^{n+g}),
\]

and the associated allocations \(A\mid g_1^*Q_0\) and
\(W^{(10')}\mid g_1^*Q_0\), together with \(C_3\) odd and the \(\mu\)-core.
R40 rederives the same divisibility in the production-native coordinates and
uses it as its finite-cell enumeration gate; it is a **reinforcement/recovery,
not a newly discovered independent theorem**.

The shared theorem is

\[
\boxed{u_0\mid W+A10^{m_3}.}
\tag{R40-DIV}
\]

This makes every fixed \((n_2,n_3)\) digit cell finite, but does **not** bound
the set of digit cells globally.

### 1.4 Frozen assumptions

The following are the assumptions that may be used in continuation, subject to
the stated scope:

- exact integer arithmetic only for theorem-level claims;
- primitive sphere coordinates and source selectors retain their full gcd
  conditions;
- \(U\) remains an absolute source variable and may not be quotiented out;
- the actual decimal cut is part of the object, not a final replay step;
- \(q\) is eliminated only through the exact finite interval and coprimality
  predicate (TP);
- \(Q_-\le Q_+\) is required before the corrected simultaneous partition;
- successor residues begin at the integer edge \(U_{\rm lo}\);
- finite search output is a bounded certificate or regression, never a universal
  nonexistence proof;
- historical File Library references with no mounted bytes are ledger
  cross-checks, not newly recomputed hashes.

### 1.5 Closed results

The following are the strongest currently closed items. “Closed” means closed
only in the scope stated; none alone closes the global parent problem.

| ID | Result | Status | Scope |
|---|---|---|---|
| T1--T18 | Sphere, denominator, digit-gap, critical/strict-layer necessary structure | `PROVED` | parent arithmetic interface |
| DD | DD branch | `PROVED EMPTY` | Strict-layer decomposition |
| R1 | Source-affine-section loss is the common obstruction | `PROVED` | architecture diagnosis |
| R2 | Source section internalization in the canonical source-completed chart | `PROVED` | canonical chart only |
| R3 | finite source-completed valuation atlas | `PROVED` | atlas/cell semantics, not global extinction |
| R6 | complementary sphere-master discriminant square class | `PROVED`; universal obstruction `DISPROVED` | moving profiles |
| R7/R7B/R7C/R7D | exceptional square locus, oriented root divisibility, source divisor/determinant gates | `PROVED` as reductions; no global extinction | specified source-completed loci |
| R27 | decimal capacity and Gaussian split restrictions | `PROVED` | primitive packet-only necessary locus |
| R30 | exact \(q\)-elimination and Möbius terminal count | `PROVED` | fixed architecture |
| R35 | master-refined terminal predicate and unit-branch non-kill lemma | `PROVED` | fixed completed profile |
| R36 | corrected simultaneous partition and canonical successor | `PROVED` | completed profile / decorated strata |
| R37 | corrected gcd-normalized generator and bounded-search audit | `PROVED` | searched cells; no global extinction |
| R38 | NRDG/factor-allocation saturation; stronger radial divisibility `DISPROVED` | `PROVED` identities / `DISPROVED` stronger conjecture | production root locus |
| R39 | exponent image saturation and \(B_{\rm src}<L_{\rm src}\) | `PROVED` | source-native production system |
| R28/R40-DIV | \(u_0\mid W+A10^{m_3}\) plus R28 shape/support allocations | `PROVED` / re-derived in R40 coordinates | TC1/production root interface |
| R40 cells | \((n_2,n_3)=(2,1)\) and \((3,1)\) exact selector/production extinction | `COMPUTATIONAL` exact finite enumeration | those two full digit cells |

### 1.6 Open results

- `Strict_A1_UNLIFTABILITY_PROVED = NO`.
- `FULL_STRICT_A1_WITNESS_FOUND = NO`.
- No global bound on \((n_2,n_3)\), \(Q_0\), \(U\), or the equivalent global
  complexity parameter is proved.
- The corrected simultaneous locus (SIM) is neither proved empty nor shown
  nonempty.
- The R40 unresolved object is
  \[
  \boxed{\text{source-native negative quadratic production roots}
  \cap\{\mathcal U_0\ne\varnothing\}.}
  \]
- Full primitive/support compatibility of the residual production root system
  is still open; the weak “actual \(U\)+selector+exponent synchronization+
  incidence+sphere” overflow claim is false by an exact counterexample.
- No terminal pair has been reconstructed to original decimal blocks.

### 1.7 Current first failure

There are two distinct first-failure records and they must not be merged:

1. **Production-root route (R39):** the first exact exponent-synchronized root
   \[
   (P_1,P_2,P_3,Q_0)=(48,436,75,445)
   \]
   passes selector normalization, primitive sphere, shape, support and
   \(Λ\)-recovery, but its source interval is empty:
   \[
   U_{\rm lo}=1>0=U_{\rm hi}.
   \]
2. **Actual-source route (R40):** the deepest exact source-side packet found is
   \[
   (P_1,P_2,P_3,Q_0)=(150,1450,225,1475).
   \]
   It passes actual \(U\), digit rooms, exponent synchronization, incidence,
   sphere and selector checks, but its first mandatory failure is
   \[
   \gcd(150,1450,225,1475)=25\ne1,
   \]
   with an independent support failure
   \(\gcd(\Lambda,C_2C_3)=25\ne1\). It is therefore not a Strict (A_1)
   witness.

The active first-failure boundary is consequently the source/primitive/support
intersection, not a generic square, Gaussian, Smith, or valuation identity.

### 1.8 Current highest-value attack

Attack the single source-completed incidence left by R40:

1. use (R40-DIV) to make \(u_0\) finite inside each fixed digit cell;
2. keep primitive sphere, \(\Lambda\)-support, exact source \(U\), successor and
   MASTER cutoff in one synchronized predicate;
3. prove a global cell bound or a source-native contradiction, or produce the
   first genuine simultaneous point and run terminal reconstruction;
4. if a simultaneous point exists, continue through (TP), denominator successor
   consistency, and reverse root reconstruction;
5. if not, record the missing global invariant rather than promoting finite
   cell no-hits to a theorem.

Routes explicitly retired by the current state: raw denominator-square overload,
factor allocation into (Q_0\pm P_1), NRDG-only valuation, generic Gaussian
representation counting, and a source-free ambient square obstruction.

## 2. Artifact Inventory

### 2.1 Stage files

The imported 105 archive contains the following primary stage files. R1--R25
are the pre-terminal architecture and gate rounds; R26--R40 are the terminal
continuation rounds.

```yaml
Artifact:
  Location: archive-by-series/90-105/105_R1_Common_Obstruction_Reconstruction.md
  Status: FROZEN / ARCHIVED
  Reliability: source-state reconstruction; theorem claims scoped in text
  Used For: common obstruction and master-object definition
Artifact:
  Location: archive-by-series/90-105/105_R2_Source_Section_Internalization.md
  Status: FROZEN / ARCHIVED
  Reliability: canonical-chart theorem with explicit qualifiers
  Used For: source fibre, actual cut, common-U semantics
Artifact:
  Location: archive-by-series/90-105/105_R3_Source_Completed_Valuation_Atlas.md
  Status: FROZEN / ARCHIVED
  Reliability: source-completed cell atlas; not global closure
  Used For: valuation cells and branch labels
Artifact:
  Location: archive-by-series/90-105/105_R4_Source_Completed_Fixed_Incidence_Extraction.md
  Status: FROZEN / ARCHIVED
  Reliability: fixed-incidence reductions with exceptional-locus qualifiers
  Used For: moving-profile incidence
Artifact:
  Location: archive-by-series/90-105/105_R5_Outer_Depth_Source_Selector_Fixedness.md and 105_R5C_Moving_Base_Full_Source_Decision.md
  Status: FROZEN / ARCHIVED
  Reliability: R5C explicitly retains the moving-base failure
  Used For: source selector and square/master gate history
Artifact:
  Location: archive-by-series/90-105/105_R6_General_Moving_Profile_Sphere_Master_Lift.md
  Status: FROZEN / ARCHIVED
  Reliability: canonical discriminant reduction; no universal obstruction
  Used For: sphere/master square locus
Artifact:
  Location: archive-by-series/90-105/105_R7_Exceptional_Square_Locus_Source_Intersection.md, 105_R7B_Oriented_Root_Divisibility.md, 105_R7C_Prescribed_Source_Divisor_Gate.md, 105_R7D_Determinant_Packet_Source_GCD_Firewall.md
  Status: FROZEN / ARCHIVED
  Reliability: scoped reductions and source gates
  Used For: exceptional square, source divisor and support structure
Artifact:
  Location: archive-by-series/90-105/105_R8_Common_U_Integer_Source_Fibre.md through 105_R25_Positive_Carrier_Excess_Divisor.md
  Status: FROZEN / ARCHIVED
  Reliability: each file carries its own saturation/negative-result boundary
  Used For: common-U fibre, master phases, carrier/support and terminal-gate history
Artifact:
  Location: archive-by-series/90-105/105-R26-stage-archive.md
  Status: FROZEN / ARCHIVED; later claims narrowed by R27 and R40
  Reliability: packet-level finite predicate only; early global-sounding verdicts not inherited
  Used For: fixed primitive-packet lift wrapper
Artifact:
  Location: archive-by-series/90-105/105-R27-stage-archive.md
  Status: FROZEN / ARCHIVED
  Reliability: exact-capacity and Gaussian necessary reductions; infinite survivor family retained
  Used For: packet-only exceptional-locus restriction
Artifact:
  Location: archive-by-series/90-105/105-R28-stage-archive.md and companions
  Status: FROZEN / ARCHIVED
  Reliability: frozen historical input; companion-byte availability is ledger-dependent
  Used For: TC1/radial support gate
Artifact:
  Location: archive-by-series/90-105/105-R29-stage-archive.md
  Status: FROZEN / ARCHIVED
  Reliability: exact Smith/tail pass with a counterexample to the stronger collision conjecture
  Used For: post-radial support saturation boundary
Artifact:
  Location: archive-by-series/90-105/105-R30-stage-archive.md
  Status: FROZEN / ARCHIVED
  Reliability: exact q-elimination and 540000-case verifier; no global extinction
  Used For: terminal predicate (TP) and successor input
Artifact:
  Location: archive-by-series/90-105/105-R31-stage-archive.md
  Status: FROZEN / ARCHIVED
  Reliability: bounded q1/forced-scale analysis; no global source theorem
  Used For: unit chamber history
Artifact:
  Location: archive-by-series/90-105/105-R32-stage-archive.md through 105-R34-stage-archive.md
  Status: FROZEN / ARCHIVED
  Reliability: exact local/unit/master/source-word saturations; no global lift decision
  Used For: master/source-word collision interface
Artifact:
  Location: archive-by-series/90-105/105-R35-stage-archive.md
  Status: FROZEN / ARCHIVED
  Reliability: terminal predicate saturation; extinction explicitly not proved
  Used For: master-refined q window and unit-branch boundary
Artifact:
  Location: archive-by-series/90-105/105-R36-stage-archive.md
  Status: FROZEN / ARCHIVED
  Reliability: corrected simultaneous partition and integer-edge successor
  Used For: source successor consistency
Artifact:
  Location: archive-by-series/90-105/105-R37-stage-archive.md
  Status: FROZEN / ARCHIVED
  Reliability: corrected gcd normalization; bounded searches are reconnaissance
  Used For: selector-consistent normalized root interface
Artifact:
  Location: archive-by-series/90-105/105-R38-stage-archive.md
  Status: FROZEN / ARCHIVED
  Reliability: exact NRDG identities; proposed stronger factor allocation falsified
  Used For: retire factor-allocation route
Artifact:
  Location: archive-by-series/90-105/105-R39-stage-archive.md
  Status: FROZEN / ARCHIVED
  Reliability: exponent-image saturation and production-native root system
  Used For: current production root interface and first failure
Artifact:
  Location: archive-by-series/90-105/105-R40-FINAL-FAILURE-REPORT.md
  Status: FINAL FAILURE REPORT
  Reliability: authoritative latest global status
  Used For: current first failure, exact counterexample, and next attack
```

### 2.2 Theorem / lemma artifacts

```yaml
Artifact:
  Location: 00-foundation/proved_results_index_v3.md
  Status: FROZEN INDEX
  Reliability: audited summary; detailed reports are authoritative for proofs
  Used For: T1-T18 and proof-grade/computational status boundary
Artifact:
  Location: archive-by-series/90-105/105_R6_General_Moving_Profile_Sphere_Master_Lift.md
  Status: PROVED REDUCTION / UNIVERSAL OBSTRUCTION OPEN
  Reliability: source-qualified square-class identity
  Used For: sphere/master discriminant
Artifact:
  Location: archive-by-series/90-105/105_R7B_Oriented_Root_Divisibility.md
  Status: PROVED SCOPED LEMMA
  Reliability: source-completed oriented divisibility only
  Used For: root selector gate
Artifact:
  Location: archive-by-series/90-105/105-R30-q-elimination-derivation.md
  Status: PROVED
  Reliability: exact integer/Möbius equivalence on fixed architecture
  Used For: eliminate residual q without dropping coprimality
Artifact:
  Location: archive-by-series/90-105/105-R36-unit-canonical-successor-derivation.md
  Status: PROVED SCOPED
  Reliability: integer-edge successor with decorated-branch qualifier
  Used For: source successor
Artifact:
  Location: archive-by-series/90-105/105-R39-exponent-synchronization-derivation.md
  Status: PROVED
  Reliability: prescribed-q exponent image; not source-fibre extinction
  Used For: deterministic (m_2,m_3,g,k)
Artifact:
  Location: archive-by-series/90-105/105-R39-production-native-root-system.md
  Status: PROVED SYSTEM
  Reliability: exact incidence/sphere system and branch sign result
  Used For: R40 continuation
Artifact:
  Location: archive-by-series/90-105/105-R40-FINAL-FAILURE-REPORT.md
  Status: PROVED R40-DIV + bounded-cell results
  Reliability: latest audit; global finiteness explicitly denied
  Used For: active obligation
```

### 2.3 Computation artifacts

```yaml
Artifact:
  Location: archive-by-series/90-105/105_R2_q1_transport_certificate.py and .txt
  Status: COMPUTATIONAL CERTIFICATE
  Reliability: exact script/certificate; scoped to its transport test
  Used For: q1 source transport regression
Artifact:
  Location: archive-by-series/90-105/105_R15_phase_offensive.py; 105_R16_master_complement.py; 105_R17_post_d_source_excess.py
  Status: COMPUTATIONAL / STRUCTURE DISCOVERY
  Reliability: use only with accompanying stage reports and manifests
  Used For: phase/master/support searches
Artifact:
  Location: archive-by-series/90-105/r27_recon.py; r29_support_core.py; r32_unit_digit.py; r36_sourcefirst_unit_shell.py; r39_verify.py
  Status: COMPUTATIONAL ARTIFACTS
  Reliability: exact-integer implementations; finite outputs do not globalize
  Used For: R27/R29/R32/R36/R39 replay and regression
Artifact:
  Location: archive-by-series/90-105/verify_transfer_first_failure.py; verify_r11_quotient.py; verify_r13_carrier_image.py; verification_output.txt
  Status: COMPUTATIONAL AUDIT
  Reliability: verification logs/claims are scope-limited
  Used For: transfer, quotient and carrier checks
Artifact:
  Location: archive-by-series/90-105/*execution.log and *SHA256-MANIFEST.txt
  Status: PROVENANCE / COMPUTATION LOG
  Reliability: local artifacts are byte-hashed; historical references may be ledger cross-checks
  Used For: reproducibility and artifact integrity
Artifact:
  Location: archive-by-series/90-105/*Artifacts.zip and *bundle.zip
  Status: PACKAGED COMPUTATION ARTIFACTS
  Reliability: inspect manifest before treating a bundled claim as available
  Used For: frozen companions, registries and reruns
```

### 2.4 Proof and failure artifacts

```yaml
Artifact:
  Location: archive-by-series/90-105/105-R39-SOURCE-EXPONENT-IMAGE-SATURATION-CERTIFICATE.md
  Status: PROOF / SATURATION CERTIFICATE
  Reliability: proves exponent-image removal, not A1 extinction
  Used For: retire ambient exponent freedom
Artifact:
  Location: archive-by-series/90-105/105-R39-FIRST-EXPONENT-SYNCHRONIZED-ROOT.md
  Status: EXACT ROOT CERTIFICATE
  Reliability: genuine production root, not a full source lift
  Used For: first failure witness
Artifact:
  Location: archive-by-series/90-105/105-R40-FINAL-FAILURE-REPORT.md
  Status: FAILURE REPORT
  Reliability: latest authoritative negative boundary
  Used For: no-closure declaration and next obligation
Artifact:
  Location: 00-foundation/provenance/MISSING_ARTIFACTS_2026-08-16.md
  Status: PROVENANCE WARNING
  Reliability: authoritative for missing referenced bytes
  Used For: prevent fabricated replays
```

### 2.5 Literature artifacts

```yaml
Artifact:
  Location: archive-by-series/65-bridge-and-provenance/source_audit.md
  Status: EXISTING HISTORICAL EXTERNAL-THEOREM AUDIT; NOT AN ACTIVE 105 DEPENDENCY
  Reliability: source audit only; claims must not be silently imported into 105
  Used For: provenance warning and applicability boundary
Artifact:
  Location: 105-specific literature artifact
  Status: NOT FOUND IN RECOVERED CHECKOUT
  Reliability: none
  Used For: no external theorem may be inherited from the archive by default
```

## 3. Knowledge Boundary

### PROVED

- The exact sphere/master, source-section, Smith/support, successor, and
  production-root reductions listed above, with their scope qualifiers.
- R40-DIV and finiteness inside a fixed digit/exponent cell.
- The R28 support package accompanying R40-DIV: \(C_3\) odd, decimal-only
  common support of \((u_0,W)\), and the stated \(A/W\) allocations.
- Exact finite-cell extinction for the two enumerated R40 cells.

### COMPUTATIONAL

- All finite no-hit counts, including R40's two cells, R36's bounded source-first
  shell, and R37's expanded stress lanes.
- The existence of raw or production-normalized roots that fail a downstream
  gate.
- Hash/manifests and replay logs as evidence of what was run, not as universal
  mathematical conclusions.

### HEURISTIC / RESEARCH DIRECTION

- A global source/master synchronization obstruction may exist.
- The source-native negative quadratic locus may have empty intersection with
  \(\mathcal U_0\).
- A global bound on digit complexity may be discoverable from the source-native
  divisibility and primitive/support constraints.

### DISPROVED OR RETIRED

- R26's early packet-level language cannot be promoted to global Strict-A1
  extinction; R27/R40 retain infinite/global scope.
- Exponent synchronization alone implies extinction: falsified by the R39 root.
- Weak actual-\(U\)+selector+incidence+sphere synchronization automatically
  lifts: falsified by the R40 packet ((150,1450,225,1475)).
- Strong universal factor allocation into (Q_0\pm P_1), NRDG-only closure,
  generic Gaussian representation counting, and raw denominator-square overload.

### OPEN

No statement in the open list may be used as a premise in the next stage:

- global Strict-A1 unliftability or existence;
- global digit-cell bound;
- nonempty/empty corrected simultaneous locus;
- source-compatible primitive/support root;
- terminal pair and root reconstruction.

## 4. Initial Research-State Update

```yaml
Research State Update:
  Previous State: "Unknown to the new agent; only repository assets available."
  New Observation: "R40 is the latest authoritative boundary: R40-DIV is proved and two complete digit cells are extinct, but global digit complexity remains unbounded and no full Strict-A1 witness exists."
  Changed Assumption: "Do not inherit R26's early global-sounding terminal language or treat exponent synchronization / finite no-hit as global closure."
  New Open Obligation: "Decide the source-native negative quadratic production-root locus intersected with the completed source fibre U_0, while retaining primitive/support, successor and MASTER conditions."
  Reason: "R39 supplies a genuine exponent-synchronized ambient root; R40 supplies a genuine actual-source counterexample to weak lifting and identifies the first mandatory failures."
```

## 5. Recovery verdict

The project is not closed. The correct hand-off state is:

\[
\boxed{
\text{Strict }A_1\text{ remains OPEN; the current bottleneck is source-completed}
\text{ primitive/support/root incidence, not ambient square arithmetic.}
}
\]

The next continuation may use the frozen formulas above, but must either prove a
global theorem covering all digit cells or produce a fully source-completed
terminal pair. A finite extension of the current searches is not enough.
