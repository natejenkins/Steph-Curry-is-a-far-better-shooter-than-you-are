It's easier to first calculate the probability that he didn't hit 77 in a row on any of the 1000 days:

\(P_\textrm{failure} = (1-{p_3}^{77})^{1000} \approx (1-1000*{p_3}^{77})\)

Then the probably that he did indeed hit 77 in a row is \(P_\textrm{success} = 1 - P_\textrm{failure}\).

We are finally in a position to solve this, we can set \(P_\textrm{success}\) to 0.5, ie let's put the odds at 50% for success.  Solving the resultant equation:

\(p_3 = (0.5/1000)^{1/77} \approx 90.6\%\)
