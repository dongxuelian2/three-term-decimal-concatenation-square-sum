Summary: The authoritative omega term cancels the normalized power quotient, forcing m congruent to 1 modulo 8 and classifying the surviving close-factor residues and endpoints.

Classification: NEW_LEMMA and BRANCH_CLOSURE. Worker verification: VERDICT: CORRECT.

Let
\[
R=2^tR_0,\qquad R_0\ \text{odd},
\]
and
\[
C_t(R_0)=\frac{5^R-1}{2^{t+2}}.
\]
Then
\[
\boxed{C_t(R_0)\equiv\omega_t(R_0)\pmod8}
\]
for every \(t\ge0\), where GC2B-4 defines
\[
\omega_t(R_0)\equiv
\begin{cases}
R_0+4\binom{R_0}{2}\pmod8,&t=0,\\
3R_0\pmod8,&t=1,\\
-R_0\pmod8,&t\ge2.
\end{cases}
\]

For \(t=0\), this follows by expanding \((1+4)^{R_0}\) modulo \(32\). For \(t=1\), expand \(25^{R_0}=(1+24)^{R_0}\) modulo \(64\). For \(t\ge2\), put
\[
c_t=\frac{5^{2^t}-1}{2^{t+2}}.
\]
Since \(c_2=39\equiv-1\pmod8\) and
\[
c_{t+1}=c_t+2^{t+1}c_t^2,
\]
one has \(c_t\equiv-1\pmod8\) for every \(t\ge2\), hence
\[
C_t(R_0)\equiv R_0c_t\equiv-R_0\pmod8.
\]

Therefore the mandatory growing quotient congruence simplifies to
\[
\begin{aligned}
m
&\equiv-7+5^F\omega_t(R_0)
+\frac{5^F(1-5^R)}{2^{t+2}}\\
&\equiv-7+5^F\bigl(\omega_t(R_0)-C_t(R_0)\bigr)
\equiv1\pmod8.
\end{aligned}
\]
Thus every quotient-compatible R2 state satisfies
\[
\boxed{m\equiv1\pmod8}.
\]

For the close-factor branch \(e=1\), this is compatible with the digit-recovery condition \(m\equiv1\pmod4\), so neither recovery sign is eliminated. The sign-specific digit residues become
\[
\boxed{L_+:\delta\equiv1\pmod4,\qquad
L_-:\delta\equiv3\pmod4},
\]
where \(\delta=a_3\).

Since \(16\mid Y\),
\[
Y+1\equiv1\pmod{16},\qquad 10Y-1\equiv-1\pmod{16}.
\]
Hence the effective close-factor endpoints are classified exactly by
\[
\boxed{
\begin{array}{c|cc}
&\delta=Y+1&\delta=10Y-1\\ \hline
L_+&\text{survives}&\text{eliminated}\\
L_-&\text{eliminated}&\text{survives}.
\end{array}}
\]
Interior close-factor candidates remain possible only in the displayed sign-specific residue classes.

The conclusion holds for \(t=0\), \(t=1\), all \(t\ge2\), and the boundary \(t=a-4\), while retaining the separate parity conditions on \(F,R,a\).

Authority classes:
- PROJECT_THEOREM: GC2B-4 for the definition of \(\omega_t\), the growing quotient congruence, and the parity conditions.
- PROJECT_THEOREM: GP3, PR6, SD6, GCU-2, GC2B-4 for the quotient and digit-recovery contracts.
- LOCAL_PROOF: the computation of \(C_t(R_0)\), cancellation yielding \(m\equiv1\pmod8\), and the close-factor classification.