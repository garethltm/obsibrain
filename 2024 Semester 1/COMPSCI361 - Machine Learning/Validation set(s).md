- is a sample of data held back from training your model that is used to give an estimate of model skill while tuning model’s [[hyperparameter(s)]].

## [[2024 Semester 1/COMPSCI361 - Machine Learning/Overfitting|Overfitting]] to the [[Validation set(s)]]
- [[Validation Error]] usually has [[Optimization Bias]] than [[training error]]
	- Might optimize over 20 values of depth, instead of millions+ of possible trees
- But we can still cause [[2024 Semester 1/COMPSCI361 - Machine Learning/Overfitting|Overfitting]] to the [[Validation Error]] (common in practice)
	- [[Validation Error]] is only an unbiased approximation if you use it once
	- Once you start optimizing it, you start 