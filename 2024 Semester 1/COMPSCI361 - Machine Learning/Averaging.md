- Improves approximation error of [[classifier(s)]] with high $E\tiny {approx}$ - models that overfit

Input: the prediction of a set of models
#compsci361example 
- [[Decision Tree(s)]] make 1 prediction
- [[Naïve Bayes classification]] makes another prediction
- [[k-nearest neighbour (KNN)]] makes another prediction

![[Simple model averaging]]

[[Averaging]] / [[Stacking]] often performs better than individual models

## Why does [[Averaging]] work?
1. #compsci361example Consider 3 binary [[classifier(s)]], each independently correct with probability 0.8 - with [[Simple model averaging]], the [[Ensembles]] is correct if we have at least 2 right:![[Pasted image 20240411162311.png]]
- So the [[Ensembles]] is right with a probability of 0.896 (0.512 + 0.384)
	NOTE:
	1. For [[Averaging]] to work, [[classifier(s)]] need to be at least somewhat independent
	2. You also want the probability of being right to be > 0.5, otherwise it will do much worse
	3. Probabilities also shouldn't be too different (otherwise, it might be better to take most accurate)
