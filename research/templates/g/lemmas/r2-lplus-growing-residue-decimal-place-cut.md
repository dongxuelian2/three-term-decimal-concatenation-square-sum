Summary: Every canonical L-plus survivor has m congruent to 1 modulo 8, satisfies F at least 2a+1, and obeys an explicit scale inequality coupling the quotient to the canonical decimal block.

Classification: NEW_LEMMA. Worker verification: VERDICT: CORRECT.

In the quotient-complete \(L_+\) branch put
\[
g=m(hm-1),\qquad C=g\delta,\qquad
k=2hm-1,\qquad
L=\frac{10^FH_1}{d^2},
\]
where
\[
d=2^a,\qquad h=2^{2a-2},\qquad \delta=a_3.
\]
Then
\[
e=\frac{C-L}{k},\qquad
1\le e<\frac{C}{2k}.
\]
The integrality condition is equivalent to
\[
\delta\equiv-4hL\pmod{k}.
\]
Since \(4h=d^2\), this may also be written
\[
\boxed{\delta\equiv-10^FH_1\pmod{k}}.
\]

Define
\[
N=m\delta-2e,\qquad
M=(hm-1)\delta-2he=hN-\delta.
\]
Then
\[
2L+m\delta=kN,\qquad
2hL-(hm-1)\delta=kM,
\]
and the canonical product equation is
\[
\boxed{
k^2D=(2L+m\delta)
\bigl(2hL-(hm-1)\delta\bigr)
}
\]
with
\[
D=NM=(2^Ra_1)^2+a_2^2.
\]

By [[lemmas/r2-authoritative-growing-residue-close-factor-classification]],
\[
\boxed{m\equiv1\pmod8}.
\]
The canonical mod-\(8\) digit condition gives
\[
e\delta\equiv1\pmod4.
\]
Thus \(e\) is odd and
\[
e-m\delta\equiv0\pmod4.
\]

The identity
\[
L=hmN+e-m\delta
\]
therefore implies \(4\mid L\). Writing
\[
H_1=2B,\qquad B\ \text{odd},
\]
one has
\[
L=2^{F+1-2a}5^FB.
\]
Consequently
\[
\boxed{F\ge2a+1}.
\]
More precisely, if
\[
\lambda=F+1-2a,
\]
then \(\lambda\ge2\), and
\[
\begin{cases}
v_2(e-m\delta)=\lambda,&2\le\lambda<2a-2,\\
e\equiv m\delta\pmod{2^{2a-2}},&\lambda\ge2a-2.
\end{cases}
\]
The separate parity conditions strengthen this to
\[
t=0:\quad F\ge2a+2,
\qquad
t\ge1:\quad F\ge2a+1.
\]

The effective third-block interval is
\[
\boxed{10^F+1\le\delta\le10^{F+1}-1,\qquad \delta\ \text{odd}}.
\]
The strict \(L_+\) scale inequality yields
\[
\boxed{d^2m(hm-1)<2H_1}.
\]
Combining this with
\[
m>\frac{(J+1)5^F}{2^{t+2}},
\qquad
2^{t+2}=\frac{2h}{2^A},
\]
gives
\[
\boxed{
2^A(J+1)5^F<1+\sqrt{1+2H_1}
}.
\]
Using the canonical decimal bound \(H_1<10^{R+1}\), every survivor satisfies
\[
\boxed{
\bigl(2^A(J+1)5^F-1\bigr)^2
<1+2\cdot10^{R+1}.
}
\]

The \(e=1\), \(\delta=10^{F+1}-1\) endpoint is impossible, while the \(e=1\), \(\delta=10^F+1\) endpoint remains compatible.

All moving congruences modulo \(5^F\), fixed residues, strict quotient windows, separate parity conditions, canonical digit ranges, authorized reducedness predicates, and both reconstruction equations remain mandatory. No recovered-pair coprimality or factor cancellation is used.

Authority classes:
- PROJECT_THEOREM: GP3, PR6, SD6, GCU-2, GC2B-4.
- LOCAL_PROOF: the progression, valuation, decimal-place inequality, and residual reduction above.