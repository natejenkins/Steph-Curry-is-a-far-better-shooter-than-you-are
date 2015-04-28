It is a worthy exercise to try and calculate \(A_n(3)\) yourself (I failed).  The approach given in \cite{Schilling1990} is to build up the solution recursively.  Let's write out all substrings which start with a streak of 0 or more Hs, terminate upon the first occurrence of T, and satisfy \(R_n{\leq}3\):

\[T\]
\[HT\]
\[HHT\]
\[HHHT\]

For the starting substring \(T\), there are \(A_{n-1}(3)\) possible ways to satisfy \(R_n{\leq}3\), we simply tack on all valid strings of length \(n-1\) to \(T\) and end up with a valid string of length \(n\).  For \(HT\), there are \(A_{n-2}(3)\) ways, and so on.  This gives the following full recursive formula for \(A_{n-1}(3)\):

\[
A_{n}(3) = A_{n-1}(3) + A_{n-2}(3) + A_{n-3}(3) + A_{n-4}(3)
\]

and in general:

\[
A_{n}(x) = \sum_{i=0}^{x} {A_{n-i-1}(x)}
\]

