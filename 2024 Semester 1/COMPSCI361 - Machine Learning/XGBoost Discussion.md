Instead of pruning trees if score doesn't improve (grows full trees)
- Prunes parts that don't improve score with [[L0-regularization]] added

Cost of fitting trees in [[eXtreme Gradient Boost (XGBoost)]] is same as usual [[Decision Tree(s)]] cost
- [[eXtreme Gradient Boost (XGBoost)]] includes a lot of tricks to make this efficient
- But cannot be done in parallel like [[Random Forests]]
	- Because it depends on the sum - correcting the errors (no independent trees)

In [[eXtreme Gradient Boost (XGBoost)]], it's the residuals that act like weights in [[AdaBoost]]
- Focuses on decreasing error in examples with large residuals

## How do you maintain efficiency if not using squared error?
- For non-quadratic losses like logistic, there is no closed-form solution
- Approximates non-quadratic losses with 2nd-order Taylor expansion
	- Maintains least squares efficiency for other losses (by approximating with quadratic)