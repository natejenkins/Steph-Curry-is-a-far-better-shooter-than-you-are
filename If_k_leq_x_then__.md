If \(k\leq x\) then all strings are valid and \(C_n^{(k)}(x) = \binom{n}{k}\).  If \(x\lt k\) and \(k = n\), \(C_n^{(k)}(x) = 0\), no strings are valid.  For \(C_n^{(k)}(3)\) with \(x\lt{k}\lt{n}\), we can write out:

\[
C_n^{(k)}(3) = C_{n-1}^{(k)}(3) + C_{n-2}^{(k-1)}(3) + C_{n-3}^{(k-2)}(3) + C_{n-4}^{(k-3)}(3)
\]