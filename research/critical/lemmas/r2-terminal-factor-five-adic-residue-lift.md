Summary: Terminal-factor allocation leaves exactly four sign-specific classes modulo 40 and excludes all other classes compatible with m congruent to 1 modulo 8.

Classification: BRANCH_CLOSURE and DIAGNOSTIC. Independent worker verification: VERDICT: CORRECT.

Retain
\[
qr=1+2^A5^{F+R},\qquad
q=2^{2a}Q-1,\qquad
q\equiv\pm2\pmod5,
\]
together with
\[
m\equiv1\pmod8.
\]
Exact reduction of the quotient identities modulo \(5\), followed by CRT with the mod-\(8\) condition, gives the complete surviving table
\[
\boxed{
\begin{array}{c|c|c}
 &q\equiv2\pmod5&q\equiv-2\pmod5\\ \hline
a\text{ even}&m\equiv33\pmod{40}&m\equiv1\pmod{40}\\
a\text{ odd}&m\equiv17\pmod{40}&m\equiv9\pmod{40}.
\end{array}}
\]
Consequently, after allowing either sign,
\[
\boxed{
\begin{aligned}
a\text{ even}:&\quad m\equiv1,33\pmod{40},\\
a\text{ odd}:&\quad m\equiv9,17\pmod{40}.
\end{aligned}}
\]
Thus the following infinite collections are excluded:
\[
\boxed{
\begin{aligned}
a\text{ even}:&\quad m\equiv9,17,25\pmod{40},\\
a\text{ odd}:&\quad m\equiv1,25,33\pmod{40}.
\end{aligned}}
\]

This strictly strengthens [[lemmas/r2-terminal-divisor-mod40-subbranch-closure]] and is uniform for
\[
0\le t\le a-4.
\]

For every fixed \(n\le F\), each lift modulo \(5^n\) of a surviving sign-specific class is locally compatible with the terminal-factor and quotient congruences. In particular, moduli \(25,125,200,1000\) introduce no further exclusion beyond the table above. These local lifts are not integral candidates and do not include canonical digit, scale, endpoint, reducedness, or reconstruction conditions.

Authority classes:
- PROJECT_THEOREM: `PR6`, `SD6`, `GCU-2`, `GC2B-4` for the inherited quotient and factor contracts.
- LOCAL_PROOF: the sign-specific table, CRT closure, prime-power lift bijection, and limitation statement.