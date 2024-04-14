Chi-merge: $\chi  ^2$-based [[Discretization]]
- [[Supervised Learning]]: use class information
- Bottom-up merge: find the best neighbouring intervals (those having similar distributions of classes #compsci361example low $\chi ^2$ values) to merge
- Merge performed recursively, until a predefined stopping condition

#compsci361example Given 2 nominal variables C and B with values $c\tiny {1}\normalsize,...,c\tiny {k}$ & $b\tiny {1}\normalsize,...,b\tiny {r}$ the correlation can be calculated using the $\chi ^2$ test:
$$\chi ^2 = \displaystyle\sum_{i=1}^k \displaystyle\sum_{j=1}^r \frac {(o\tiny {ij}\normalsize -e\tiny{ij}\normalsize)^2}{e\tiny {ij}}$$
- $o\tiny {ij}$ being the actual frequency of the event ($c\tiny {i}\normalsize, b\tiny {j}$)
- $e\tiny {ij}$ being the expected frequency (n is the number of instances)

$$e\tiny{ij}\normalsize = \frac {count(C = c\tiny{i}\normalsize )}{}$$

- the test measures the correlation between the 2. If there is a correlation based on this statistic.
	- this statistic goes over all possible combination of values for the 2 variables & calculates the distance between observed count vs the expected count, where the expected count is the Null Hypothesis = they are not correlated
