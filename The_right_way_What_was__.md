# **The right way**

What was so wrong about the above calculation?  The article mentioned that Steph didn't shoot until he missed, he shot 100 3-pointers, made 77 in a row, and 94 out of 100.  Limiting the calculation to a total of 77 shots means that if he misses the first attempt it is game-over, yet in reality he could start his streak on any shot up to and including his 24th.  To calculate this properly we first need to talk about flipping coins.

## **Streaks of Heads**

Each time I flip a fair coin there is a \(50\%\) probability for heads, let's call this probability \(p\), and likewise for tails, let's call this probability \(q\).  For the moment \(p\) and \(q\) are equal, but that won't always be the case.  A string of 5 flips might result in the following:

\(\textrm{HHTHT}\)

The probability of this string occurring is simply:

\(P_5(\textrm{HHTHT}) = ppqpq = p^3q^2\)

and in general:

\(P_n(s) = p^kq^{n-k}\)

Since I can re-arrange the powers of \(p\) and \(q\) however I like, you can see that the ordering of heads and tails in a given string does not affect the probability of that string occurring, only their respective numbers and probabilities.  To calculate not only the probability of a given string with say 3 heads occurring, but of having any string of length \(n\) with exactly 3 heads, we simply need to count all the different ways to get 3 heads in a string of length \(n\) and multiply that by \(P_n(s)\).

This is given by the [binomial coefficient](http://en.wikipedia.org/wiki/Binomial_coefficient) \(\binom{n}{k}\) and we can use it to calculate the total probability of \(k\) heads in a random string of length \(n\)

\(P_{n}(k) = \binom{n}{k}p^kq^{n-k}\)

