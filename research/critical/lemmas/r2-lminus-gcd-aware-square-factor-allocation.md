Summary: Exact gcd accounting reduces every three-mod-four prime to three local allocation types without cancelling shared factors.

Classification: NEW_LEMMA. Independent worker verification: VERDICT: CORRECT.

Let
\[
c=uv,\qquad \gcd(u,v)=1,\qquad D=MN,
\]
and suppose
\[
L-e=uM,\qquad L+e=vN.
\]
Put
\[
g=\gcd(M,N),\qquad M=gM_0,\qquad N=gN_0.
\]
Then
\[
\boxed{
\gcd(L-e,L+e)
=
g\,\gcd(u,N_0)\,\gcd(v,M_0).
}
\]
For the exchanged orientation \(L-e=vM,\ L+e=uN\),
\[
\boxed{
\gcd(L-e,L+e)
=
g\,\gcd(v,N_0)\,\gcd(u,M_0).
}
\]
These formulas retain the full two-adic and odd shared parts.

In the \(L_-\) system,
\[
M=m\delta+2e,\qquad
N=(hm-1)\delta+2he,
\]
\[
L=m(hm-1)\delta+(2hm-1)e,
\]
and
\[
\boxed{L-e=(hm-1)M,\qquad L+e=mN.}
\]
Moreover,
\[
\gcd(M,N)=\gcd(e,\delta)
\]
because \(\delta\) is odd. Hence
\[
\boxed{
\gcd(L-e,L+e)
=
g\,
\gcd\!\left(hm-1,\frac Ng\right)
\gcd\!\left(m,\frac Mg\right),
\qquad g=\gcd(e,\delta).
}
\]
All displayed quantities are odd, so the gcd has two-adic valuation zero.

Fix \(p\equiv3\pmod4\) with
\[
v_p(D)=2s>0,
\qquad \nu=v_p(\delta).
\]
Using [[lemmas/r2-global-three-mod-four-valuation-support]], every surviving local allocation has exactly one of the following forms.

1. If \(\nu\ge s\), then
   \[
   v_p(M)=v_p(N)=v_p(g)=s,
   \qquad v_p(\gcd(L-e,L+e))=s.
   \]

2. If \(\nu<s\) and \(p\mid m\), then
   \[
   v_p(M)=2s-\nu,\qquad v_p(N)=v_p(g)=\nu,
   \]
   \[
   v_p(\gcd(L-e,L+e))
   =
   \nu+\min\{v_p(m),2s-2\nu\},
   \]
   and necessarily
   \[
   v_p(m)\ge s-\nu.
   \]

3. If \(\nu<s\) and \(p\mid hm-1\), then
   \[
   v_p(N)=2s-\nu,\qquad v_p(M)=v_p(g)=\nu,
   \]
   \[
   v_p(\gcd(L-e,L+e))
   =
   \nu+\min\{v_p(hm-1),2s-2\nu\},
   \]
   and necessarily
   \[
   v_p(hm-1)\ge s-\nu.
   \]

There is no fourth deficient type: if \(\nu<s\), then \(p\mid c=m(hm-1)\), and the two coefficient factors are coprime.

Thus arbitrary allocation of \(p^{2s}\) between \(M\) and \(N\) is excluded, but all three displayed types remain algebraically compatible. The theorem does not close either support branch.

Authority classes:
- PROJECT_THEOREM: `PR6`, `SD6`, `GCU-2`, `GC2B-4`.
- LOCAL_PROOF: the gcd formulas and complete local allocation classification.