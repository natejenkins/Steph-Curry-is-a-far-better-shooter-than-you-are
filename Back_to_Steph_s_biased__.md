## Back to Steph's biased coin

We are finally getting close to our answer.  Streaks of biased coins not only involve counting the number of strings with runs less than \(x\), we also have to calculate the probability of the full string occurring.  Just as before, let's look at the specific case of \(x=3\).  Let \(C_n^{(k)}(x)\) be the number of strings with exactly \(k\) heads where the longest run is less than \(x\).  Then we can write out:

\[
F_n(x) = \sum_{k=0}^{n}{C_n^{(k)}(x)p^kq^{n-k}}
\]