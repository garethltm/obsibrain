## Null Hypothesis
1. Perform a 10-fold [[Cross-Validation (CV)]]
2. Assume samples follow a t-distribution with k-1 degrees of freedom (here, k = 10)
3. Use t-test (or Student's t-test)
4. Null Hypothesis: $M\tiny 1$ & $M\tiny 2$ are the same
	- models are performing the same
5. If we can reject null hypothesis, then
	- we can conclude that the difference between $M\tiny 1$ & $M\tiny 2$ is statistically significant
	- we choose the model with lower error rate

## t-test
- if only 1 test set is available: pairwise comparison (we apply both models to the same test set)
	- For the ith round of 10-fold [[Cross-Validation (CV)]], the same cross partitioning is used to obtain $err(M\tiny 1\normalsize )\tiny i$ and $err(M\tiny 2\normalsize )\tiny i$
	- Average over (at least) 10 rounds to get $\overline {err}(M\tiny 1\normalsize )$ & $\overline {err}(M\tiny 2\normalsize )$ 
		- we get the mean error of model 1 & model 2
	- t-test computes t-statistic with k-1 degrees of freedom: ![[IMG_22E65146B328-1.jpeg]]
- where:![[IMG_98969FEBD02F-1.jpeg]]

## Statistical Significance
- Are $M\tiny 1$ & $M\tiny 2$ significantly different?
- Comput