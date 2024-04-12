Instead of pruning trees if score doesn't improve (grows full trees)
- Prunes parts that don't improve score with [[L0-regularization]] added

Cost of fitting trees in [[eXtreme Gradient Boost (XGBoost)]] is same as usual [[Decision Tree(s)]] cost
- [[eXtreme Gradient Boost (XGBoost)]] includes a lot of tricks to make this efficient
- But cannot be done in parallel like [[Random Forests]]
	- Because it depends on the sum - correcting the errors (no independent trees)