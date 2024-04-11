- is a **sample of data** held back from training your model that is used to give an estimate of model skill while tuning model’s [[hyperparameter(s)]].

## [[overfit(ting)|overfit(ting)]] to the [[Validation set(s)]]
- [[Validation Error]] usually has [[Optimization Bias]] than [[training error]]
	- Might optimize over 20 values of depth, instead of millions+ of possible trees
- But we can still cause [[overfit(ting)|overfit(ting)]] to the [[Validation Error]] (common in practice)
	- [[Validation Error]] is only an unbiased approximation if you use it once
	- Once you start optimizing it, you start to cause [[overfit(ting)|overfit(ting)]] to the [[Validation set(s)]]
- This is most important when the [[Validation set(s)]] is small
	- The [[Optimization Bias]] decreases as the number of validation examples increases
- Goal: to do well on the test set (new data), NOT the [[Validation set(s)]] (where we already know the labels)