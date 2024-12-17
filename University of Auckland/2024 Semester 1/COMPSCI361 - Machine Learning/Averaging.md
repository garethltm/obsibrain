- Improves approximation error of [[classifier(s)]] with high $E\tiny {approx}$ - models that overfit

Input: the prediction of a set of models
#compsci361example 
- [[Decision Tree(s)]] make 1 prediction
- [[Naïve Bayes classification]] makes another prediction
- [[k-nearest neighbor (kNN)]] makes another prediction

![[Simple model averaging]]

[[Averaging]] / [[Stacking]] often performs better than individual models

## Why does [[Averaging]] work?
1. #compsci361example Consider 3 binary [[classifier(s)]], each independently correct with probability 0.8 - with [[Simple model averaging]], the [[Ensemble(s)]] is correct if we have at least 2 right:![[Pasted image 20240411162311.png]]
- So the [[Ensemble(s)]] is right with a probability of 0.896 (0.512 + 0.384)
	NOTE:
	1. For [[Averaging]] to work, [[classifier(s)]] need to be at least somewhat independent (you gain nothing if its the same) - in relation to [[Independent & Identically Distributed (IID)]]
	2. You also want the probability of being right to be > 0.5, otherwise it will do much worse
	3. Probabilities also shouldn't be too different (otherwise, it might be better to take most accurate)
2. #compsci361example Consider a set of [[classifier(s)]] that makes these predictions ![[Pasted image 20240411162631.png]]
- If these independently get 80% [[Accuracy]], the mode would be close to 100%
	- In practice errors won't be completely independent due to [[Noise]] in the labels
3. #compsci361example Consider [[classifier(s)]] that [[overfit(ting)|overfit(ting)]] (like deep [[Decision Tree(s)]])
	- If they all [[overfit(ting)]] in exactly the same way, [[Averaging]] does nothing
	- But if they make independent errors
		1. Probability that average is wrong can be lower than for each [[classifier(s)]]
		2. Less attention to specific [[overfit(ting)]] of each [[classifier(s)]]
	- Combining them might still [[overfit(ting)]] but they [[overfit(ting)]] differently $\rightarrow$ somewhat [[overfit(ting)]] less because you are essentially combining them