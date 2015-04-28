# **The right way**

What was so wrong about the wrong way?  The article mentioned that Steph didn't shoot until he missed, he shot 100 3-pointers, made 77 in a row, and 94 out of 100.  Limiting the calculation to a total of 77 shots means that if he misses the first attempt it is game-over, yet in reality he could start his streak on any shot up to and including his 24th.  To calculate this properly we first need to talk about flipping coins.

## **Streaks of Heads**

Each time I flip a fair coin there is a \(50\%\) probability for heads, let's call this probability \(p\), and likewise for tails, let's call this probability \(q\).  For the moment \(p\) and \(q\) are equal, but that won't always be the case.  A string of 5 flips might result in the following:

\(\textrm{HHTHT}\)

The probability of this occurring is simply:

\(ppqpq = p^3q^2\)

i.e., the probability of getting \(x\) number of heads in a string of coin flips only depends on the probability of getting heads on a single coin flip and the total number of coin flips (you can calculate \(q\) from \(p\)).  The ordering of heads and tails doesn't matter at all, only the number.  

How about if we are only interested in the number of heads and not the exact way they came about?  In that case we need to add up all the probabilities for all strings with the desired number of heads, which involves the [binomial coefficient](http://en.wikipedia.org/wiki/Binomial_coefficient) \(\binom{n}{k}\):

\(P_{N}(k) = \binom{n}{k}p^kq^{N-k}\)

