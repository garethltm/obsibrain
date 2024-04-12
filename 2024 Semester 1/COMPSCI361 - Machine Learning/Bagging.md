using [[Bootstrapping]] samples for [[Ensemble(s)]] learning - Bootstrap Aggregating
- Generate several bootstrap samples of examples ($x\tiny {i}, \normalsize y\tiny{i}$)
- Fit a [[classifier(s)]] to each bootstrap sample
	- Train a [[classifier(s)]] on each of the samples
- At test time, average the predictions

[[Ensemble(s)]] won't make sense if the trees are the same