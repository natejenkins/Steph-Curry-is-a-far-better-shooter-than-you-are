## **Consecutive streaks of heads**

what if we are not interested in the number of heads in a given number of flips, but instead the longest streak of heads.  It's quite a bit more complicated to calculate.  Let's call this streak \(x\).  The idea is the same, we need to find all the strings that have a longest streak of \(x\), find the probability for each of those strings to occur, and add them up.  You should take a moment to convince yourself this is non-trivial and then have a look at an excellent resource: \cite{Schilling1990}. 

The idea is the following:

First consider a fair coin, \(p=q=0.5\).  If we knew how many strings of length \(N\) had a longest streak of \(x\), let's call this , we could calculate the probability directly:

\[
P_N(x) = (\textrm{number of strings with max streak x})/{2^N}
\]

As is often the case, the calculation is simplified by calculating something slightly different, instead of the probability of having a max streak of length \(x\), let's calculate the probability of having a max streak \(R_n\lex\)