- The [[Decision Tree(s)]] depth is called a [[hyperparameter(s)]]
	- [[hyperparameter(s)]] control how complex our model is
	- We can't train a [[hyperparameter(s)]]
		- You can always fit [[training data]] better by making the model more complicated
	- We validate a [[hyperparameter(s)]] using a validation score

## Choosing [[hyperparameter(s)]] with [[Validation set(s)]]
- So to choose a good value of depth ([[hyperparameter(s)]]), we coould
	1. Try a depth-1 decision tree, compute [[Validation Error]]
	2. Try a depth-2 decision tree, compute [[Validation Error]]
	3. ...
	4. Try a depth-20 decision tree, computer [[Validation Error]]
	5. Return the depth with the lowest [[Validation Error]]
- After you choose the [[hyperparameter(s)]], we usually re-train on the full training set with the chosen [[hyperparameter(s)]]