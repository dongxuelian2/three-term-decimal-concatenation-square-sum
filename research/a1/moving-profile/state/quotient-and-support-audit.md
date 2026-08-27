# 105 v3 Stage 02 — R40 Quotient / R28 Support Audit

```yaml
Stage ID: 105-V3-S02
Objective: "Determine whether R40-DIV creates information beyond the already frozen R28 TC1 support package."
Input Artifacts:
  - archive-by-series/90-105/105-R28-stage-archive.md
  - archive-by-series/90-105/105-R28-TC1-derivation.md
  - archive-by-series/90-105/105-R39-production-native-root-system.md
  - archive-by-series/90-105/105-R40-FINAL-FAILURE-REPORT.md
  - 105_V3_R40_quotient_audit.py
  - 105_V3_R40_small_root_search.py
Research Obligation:
  Question: "Does the R40 production-native divisibility gate yield a new source/primitive/support contradiction?"
  Why this matters: "If yes, it could close the only R40 object; if no, the continuation must attack the source fibre itself rather than repeat TC1 support algebra."
  Current evidence: "R28 already contains the same divisibility and a stronger support package; R40's actual-source counterexample satisfies the weak quotient system but fails primitivity and Lambda-support."
  Expected resolution: "Classify the quotient as a recovered normal form or identify a genuinely new invariant."
Method: "Exact symbolic substitution plus bounded integer reconnaissance with primitive sphere, selector, exponent, R28 shape/support, and source-room filters."
Status: CLOSED_AS_NO_NEW_INFORMATION
```

## 1. Exact quotient equivalence

Set

\[
H=W+A10^{m_3},\qquad X=10^{m_2+m_3},\qquad
Y=10^{n_3},\qquad K=10^k,
\]

\[
T=C_3+YC_2,\qquad
a_0=\frac{AW}{g_0}.
\]

R28's already-proved support divisibility is \(u_0\mid H\). The primitive
gcd argument also gives \(u_0\mid a\), and the frozen identity

\[
u_0AW=g_0a
\]

then gives

\[
\frac a{u_0}=\frac{AW}{g_0}=a_0.
\]

Write \(\ell=H/u_0\). The R40 production equation

\[
(\mu H+aX)Q_0
=
\mu g_0a(XKs+T)
\]

divides by \(u_0\) to become

\[
\boxed{(\mu\ell+a_0X)Q_0
=
\mu AW(XKs+T).}
\tag{Q}
\]

Using (P_1=g_0\mu s), equation (Q) is equivalent to

\[
\boxed{
\mu\bigl(Q_0\ell-AW(C_3+YC_2)\bigr)
=
a_0X(KP_1-Q_0).
}
\tag{MU-CORE}
\]

This is the R28 \(\mu\)-core, with \(X=10^{m+n+g}\). Therefore:

```text
R40_DIV_INFORMATION_GAIN_OVER_R28 = 0
R40_QUOTIENT_NORMAL_FORM = R28_MU_CORE
```

The associated R28 facts remain active and must be carried together:

\[
(u_0,A)=1,
\qquad
\gcd(u_0,W)=\gcd(u_0,10^{n+g}),
\]

\[
A\mid g_1^*Q_0,
\qquad
W^{(10')}\mid g_1^*Q_0,
\qquad
C_3\text{ odd},
\qquad
(\mu,C_2C_3)=1.
\]

The quotient is useful as a clean interface, but it is not a new obstruction.

## 2. Exact packet audit

`105_V3_R40_quotient_audit.py` rechecked the two authoritative packets using
integer arithmetic.

### R39 production root

\[
(P_1,P_2,P_3,Q_0)=(48,436,75,445),
\]

\[
(u_0,A,W,g_0,a,\mu,s)=(1,3,4,12,1,2,2),
\]

\[
(H,X,Y,K,T,L,B,C)=(34,100,10,10,1115,1000,168,26760).
\]

The audit confirms sphere, incidence, primitive packet, selector normalization,
exponent synchronization, R40-DIV, and (MU-CORE). The source interval remains

\[
U_{\rm lo}=1>0=U_{\rm hi}.
\]

Status: `PROVED/REPLAYED`; first downstream failure: `SOURCE_INTEGER_ROOM_EMPTY`.

### R40 actual-source counterexample

\[
(P_1,P_2,P_3,Q_0)=(150,1450,225,1475),
\]

\[
(u_0,A,W,C_2,C_3,g_0,a,\mu,s)=(1,3,2,725,75,6,1,25,1).
\]

\[
(n_2,n_3,m_2,m_3,g,k)=(3,2,2,2,0,1).
\]

The audit confirms sphere, incidence, selectors, exponent synchronization,
R40-DIV and (MU-CORE). But

\[
\gcd(P_1,P_2,P_3,Q_0)=25,
\qquad
\gcd(\Lambda,C_2C_3)=25,
\]

so this is not a primitive/support-complete Strict (A_1) state. It is a
counterexample only to the weaker claim that actual (U), selectors, exponent
synchronization, incidence and sphere automatically imply a lift.

Status: `COMPUTATIONAL/EXACT COUNTEREXAMPLE`; first mandatory failure:
`PRIMITIVITY`, with independent `LAMBDA_SUPPORT` failure.

## 3. Bounded source-root reconnaissance

The new exact script searched:

```yaml
Scope:
  Primitive sphere packets: "Q0 <= 300"
  n3: "1..3"
  residual q: "1..4"
  Arithmetic: "Python integers only"
  Root condition: "exact production incidence solved for K=10^k"
  Retained filters: "primitive packet, selector, exponent synchronization, R28 shape/support gates"
  Not claimed: "global completeness; full R30 terminal predicate for all architectures"
```

Observed exact counts:

```text
PACKETS=18270
SELECTOR_STATES=3521885
PRODUCTION_ROOTS=7
R40_DIV_FAILURES=0
R28_SHAPE_ROOTS=3
R28_SUPPORT_ROOTS=1
ROOTS_WITH_U0_GT_1=4
SOURCE_ROOM_ROOTS=0
SOURCE_ROOM_ROOTS_U0_GT_1=0
```

The single R28-support survivor in this bounded run is

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

This is a bounded observation only. It shows that the first support-admissible
root need not be the R39 packet, while the source-room failure remains the first
failure in this small scope.

## 4. Result and remaining gap

```yaml
New Result: "R40-DIV is a recovered R28 support theorem in production coordinates; its quotient is exactly the R28 MU-CORE."
Evidence: "Symbolic equivalence plus exact packet replay and bounded search."
Derivation: "Set H, X, Y, T, a0 and ell; use u0|H, u0|a, u0AW=g0a, and P1=g0 mu s to transform the R40 equation into MU-CORE."
Status: PROVED_AS_EQUIVALENCE; COMPUTATIONAL_FOR_COUNTS
Remaining Gap: "No global theorem relates the R28 support-admissible production-root locus to source-room nonemptiness, and no global digit-cell bound is available."
Next Action: "Keep the full R28 support package active and attack the source-room intersection or a global digit-complexity bound; do not repeat R40-DIV algebra."
```

## 5. Research State Update

```yaml
Research State Update:
  Previous State: "R40-DIV was provisionally treated as a new R40 theorem."
  New Observation: "R28 already proves the same divisibility and stronger support allocations; R40 only re-expresses and audits them in the production-native root system."
  Changed Assumption: "R40-DIV is not an independent information source. The active state must include R28 C3-odd, shape, mu-support, A/W allocation, and MU-CORE constraints."
  New Open Obligation: "Prove or refute the intersection of the R28-support-admissible negative quadratic production-root locus with the nonempty completed source fibre and successor/MASTER predicates."
  Reason: "The exact quotient identity saturates at R28; the bounded audit finds no source-room root but cannot globalize."
```
