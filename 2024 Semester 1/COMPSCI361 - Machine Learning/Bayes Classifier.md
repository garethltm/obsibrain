

## Bayes Optimal Classifier
#### What is the most probable [[classification]] of a new instance given the [[training data]]?
Simply adding [[Maximum A Posteriori (MAP) Hypothesis]] ($h\tiny {MAP}$)
#compsci361example 
H = {$h\tiny {1}$, $h\tiny {2}$, $h\tiny {3}$}, where $P(h\tiny {1}\normalsize |D)$ = 0.4, $P(h\tiny {2}\normalsize |D)$ = $P(h\tiny {3}\normalsize |D)$ = 0.3
$h\tiny {MAP}$ = $h\tiny {1}$ the maximum currently
Consider a new instance x encountered, which is classified positive $h\tiny {1}$ and negative by $h\tiny {2}\normalsize ,h\tiny {3}$
- here we can say that we can get a better prediction if we weight the evidence of all the hypothesis - taking the average
###### Taking all hypothesis into account
- The [[probability]] that x is positive is 0.4
- The [[probability]] that x is negative is 0.6
- most probable [[classification]] $\not =$ [[classification]] generated by [[Maximum A Posteriori (MAP) Hypothesis]] (the most likely hypothesis that you get if you maximise the posterior distribution for all possible hypothesis)
	- don't really have to use [[Maximum A Posteriori (MAP) Hypothesis]] if you only care about the best
