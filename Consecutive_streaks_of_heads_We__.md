## **Consecutive streaks of heads**

We can now calculate the chances of getting \(k\) heads in \(n\) flips, but what we really want to know is the probability of having a run of consecutive heads longer than some value \(x\).  There is an excellent resource \cite{Schilling1990} that elaborates on how to do this, with the basic idea being the following:

Let \(F_n(x)=P(R_n{\leq}x)\) be the probability of the longest run of \(n\) flips of a fair coin being less than or equal to \(x\).  Then the probability we are looking after, that of having a run greater than \(x\), is simply \(1 - F_n(x)\).  To give a concrete example, assume we are looking for \(F_n(3)\) and let \(A_n(x)\) be the number of different strings of length \(n\) containing a run no longer than \(x\).  In this case:

\[
F_n(3) = \frac{1}{2^n}A_n(3)
\]
