# **Appendix:**  **Detailed Calculation**
`WARNING: Lots of math ahead. % If you aren't into that sort of thing, skip down to the last figure`

## **Flipping Coins**

Steph Curry shooting a 3-pointer has two results, either a miss or a make.  As we've already seen, his chance of making it are much higher than his chance of missing.  This is analogous to Steph flipping a (very) biased coin, heads for a make, tails for a miss.  If we were to write out this series of coin flips, we'd end up with a string of 100 \(H\)s and \(T\)s (\(H\) for heads, \(T\) for tails) in some order, likely with many more heads than tails.  If he does this 1000 different times, we want to know what the probability is that he has a streak in any run greater than 70 (I'd argue this is still newsworthy).  Let's start with a fair coin first. 

Each time I flip a fair coin there is a \(50\%\) probability for heads, let's call this probability \(p\), and likewise for tails, let's call this probability \(q\).  For the moment \(p\) and \(q\) are equal, but that won't always be the case.  A series of 5 flips might result in the following string: \(\textrm{HHTHT}\)

The probability of this occurring is simply:

\(P_5(\textrm{HHTHT}) = ppqpq = p^3q^2\)

and in general:

\(P_n(s) = p^kq^{n-k}\).

The ordering of heads and tails in a given string does not affect the probability of that string occurring, only their respective numbers and probabilities.  To calculate not only the probability of a given string with say 3 heads occurring, but of having any string of length \(n\) with exactly 3 heads, we simply need to count all the different ways to get 3 heads in a string of length \(n\) and multiply that by \(P_n(s)\).

This is given by the [binomial coefficient](http://en.wikipedia.org/wiki/Binomial_coefficient) \(\binom{n}{k}\) and we can use it to calculate the total probability of \(k\) heads in a random string of length \(n\):

\(
P_{n}(k) = \dbinom{n}{k}\,p^kq^{n-k}
\)

