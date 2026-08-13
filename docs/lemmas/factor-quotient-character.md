Summary: The factor window admits an exact quotient variable u constrained simultaneously modulo a growing power of two and modulo \(5^F\).

All statements below are LOCAL_PROOF from the GC2B-4 negative frontier, using FOUND-NT-JAC-01/02/03 and FOUND-NT-QR-02 only where stated.

Let
\[
B=2^{2a},\qquad C=2^A,\qquad E=B/C=2^{t+3},
\qquad N=F+R,
\]
write
\[
q=BQ-1,
\]
and let
\[
H\equiv\frac{7-5^F\omega_t(R_0)}2\pmod4,
\qquad Q\equiv H\pmod4.
\]
Assume
\[
q\mid1+C5^N,\qquad
\frac{5^R}{J+1}<q<\frac{5^R}{J}.
\]

There are unique integers \(s,K,u\) satisfying
\[
5^R=Jq+s,\qquad0<s<q,
\]
\[
K=J5^F+u,\qquad1\le u\le5^F-1,
\]
and
\[
\boxed{5^N=qK-EQ.}
\]
The complementary factor is
\[
\boxed{
r=\frac{1+C5^N}{q}=CK-1=C(J5^F+u)-1.
}
\]
Moreover,
\[
\boxed{5^Fs=qu-EQ,}
\]
\[
\boxed{
u=\left\lceil\frac{5^Fs}{q}\right\rceil,
}
\]
\[
\boxed{
qu\equiv EQ\pmod{5^F},
}
\]
and
\[
\boxed{
u\equiv-5^F(5^R+J)-EH\pmod{4E}.
}
\]
Equivalently,
\[
\boxed{
u\equiv
-5^F(5^R+J)
-2^{t+2}\bigl(7-5^F\omega_t(R_0)\bigr)
\pmod{2^{t+5}}.
}
\]

Proof of the quotient identities: since \(C(EQ)=BQ=q+1\),
\[
5^N\equiv-EQ\pmod q.
\]
Also \(0<EQ<q\), so \(q-EQ\) is the least nonnegative remainder. Hence
\[
K=\left\lceil\frac{5^N}{q}\right\rceil.
\]
The strict \(q\)-window gives
\[
J5^F<K\le(J+1)5^F.
\]
Equality at the upper endpoint would imply \(5\mid EQ\), while
\(q\equiv\pm2\pmod5\) implies \(5\nmid Q\); therefore
\[
J5^F<K<(J+1)5^F.
\]
Substitution yields the displayed formulas for \(r\), \(s\), and \(u\).

For the binary congruence, the identities imply
\[
5^N+K=EQr.
\]
Since \(A\ge5\),
\[
r=CK-1\equiv-1\pmod4.
\]
Thus
\[
\frac{5^N+K}{E}=Qr\equiv-H\pmod4,
\]
which gives the stated congruence modulo \(4E=2^{t+5}\).

The composite-safe Jacobi calculation applied to
\[
2^A5^N\equiv-1\pmod q
\]
uses
\[
q\equiv7\pmod8,\qquad q\equiv\pm2\pmod5,
\]
and yields
\[
\boxed{F+R\text{ is odd}.}
\]
Consequently,
\[
t=0\Rightarrow a\text{ odd},\qquad
t\ge1\Rightarrow a\equiv t\pmod2.
\]

No step assumes that \(q\) is prime or squarefree. The unresolved arithmetic obstruction is the moving inverse
\[
u\equiv EQ(BQ-1)^{-1}\pmod{5^F},
\]
which must also satisfy the binary residue modulo \(2^{t+5}\) and
\(1\le u<5^F\). The two moduli are coprime, so CRT alone gives no contradiction.

Worker verification: VERDICT: CORRECT.