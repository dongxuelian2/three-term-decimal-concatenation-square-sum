Summary: Canonical digit recovery imposes sign-specific mod-16 conditions, closes the close-factor subbranch when the quotient fixes \(m\equiv3\pmod4\), and classifies the effective endpoint corners.

Classification: BRANCH_CLOSURE. Worker verification: VERDICT: CORRECT.

Let \(\delta=a_3\). In either quotient-complete R2 recovery core,
\[
D=(2^Ra_1)^2+a_2^2,\qquad \gcd(a_2,2^Rq)=1.
\]
The canonical interval for \(a_2\) forces \(R\ge2\). Hence \(a_2\) is odd and
\[
D\equiv a_2^2\pmod{16},\qquad D\equiv1\pmod8.
\]
Since \(a\ge4\),
\[
h=2^{2a-2}\equiv0\pmod{16}.
\]

For \(L_-\),
\[
M=m\delta+2e,\qquad N=hM-\delta,
\]
and therefore
\[
\boxed{a_2^2\equiv-m\delta^2-2e\delta\pmod{16}}.
\]
For \(L_+\),
\[
N=m\delta-2e,\qquad M=hN-\delta,
\]
and therefore
\[
\boxed{a_2^2\equiv-m\delta^2+2e\delta\pmod{16}}.
\]

Modulo \(8\), these become
\[
\boxed{
\begin{aligned}
L_-:&\quad e\delta\equiv-\frac{m+1}{2}\pmod4,\\
L_+:&\quad e\delta\equiv \frac{m+1}{2}\pmod4.
\end{aligned}}
\]
In either sign,
\[
e\text{ odd}\iff m\equiv1\pmod4,\qquad
e\text{ even}\iff m\equiv3\pmod4.
\]

Because \(w_0=de\), the close-factor boundary \(w_0=d\) is exactly \(e=1\).
Consequently,
\[
\boxed{w_0=d\Longrightarrow m\equiv1\pmod4}.
\]
Thus every quotient state whose mandatory growing congruence fixes
\[
m\equiv3\ \text{or}\ 7\pmod8
\]
has no canonical \(w_0=d\) candidate for either recovery sign.

Write
\[
H_1=10(a_1\,10^{R-1}+a_2)=2B.
\]
Then \(B\) is odd. From \(H_1\mid dS\), one obtains \(B\mid S\), and therefore
\[
Y=\frac{d^2S}{H_1}
=2^{2a-1}\frac SB.
\]
In particular \(16\mid Y\), so
\[
Y+1\equiv1\pmod{16},\qquad
10Y-1\equiv-1\pmod{16}.
\]

Combining these endpoint residues with \(e=1\) gives
\[
\boxed{
\begin{array}{c|cc}
&\delta=Y+1&\delta=10Y-1\\ \hline
L_+&m\equiv1\pmod8&m\equiv5\pmod8\\
L_-&m\equiv5\pmod8&m\equiv1\pmod8.
\end{array}}
\]
All other values of the mandatory growing \(m\bmod8\) class close the corresponding close-factor endpoint corner.

The strict factor-window endpoints cannot occur under \(q\equiv\pm2\pmod5\). Likewise, either forbidden quotient endpoint \(u=0\) or \(u=5^F\) would imply \(5^F\mid Q\), hence \(q\equiv-1\pmod5\), contradicting \(q\equiv\pm2\pmod5\).

Shared factors do not yield recovered-pair coprimality. In particular, neither
\[
\gcd(M,N)=1
\quad\text{nor}\quad
\gcd(e,\delta)=1
\]
follows from the authorized canonical contract.

This lemma closes only the stated \(e=1\) residue subbranch and incompatible endpoint corners. Both full recovery signs remain open.

Authority classes:
- PROJECT_THEOREM: GP3, PR6, SD6, GCU-2, GC2B-4.
- LOCAL_PROOF: the mod-\(16\) reductions, close-factor obstruction, endpoint-corner classification, and strict-boundary exclusions above.