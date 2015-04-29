It's easier to first calculate the probability that he didn't hit 77 in a row on any of the 1000 days (remember we are still incorrectly assuming he only shot 77 3-pointers each day, bear with me):

\(P_\textrm{failure} = (1-{P_3}^{77})^{1000} \approx (1-1000*{P_3}^{77})\)

Then the probability that he did indeed hit 77 in a row is \(P_\textrm{success} = 1 - P_\textrm{failure}\).

We are finally in a position to solve this, we can set \(P_\textrm{success}\) to 0.5, ie let's put the odds at 50% for success.  Solving the resultant equation:

\(P_3 = (0.5/1000)^{1/77} \approx 90.6\%\)

Let's say Steph was extremely lucky that day and the likelihood of this occurrence over 1000 days was only 1% instead of 50%, in that case \(P_3\) would drop to the embarrassingly-low 86%.

TODO: INSERT IMAGE WHERE READERS CAN PLAY WITH CALCULATION