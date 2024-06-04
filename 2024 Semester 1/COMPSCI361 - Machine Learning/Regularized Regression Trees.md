Procedure monotonically decreases the [[Training error]]
- As long as not all $\huge w\tiny {L} \normalsize = 0$ (prediction = 0), each tree decreases [[Training error]] 
	- continues to improve as long as the predictions are not equal to 0

#compsci361questions 
## Can it overfit?
1. It can overfit if trees are too deep - to restrict depth, add [[L0-regularization]] (stop splitting if $\huge w\tiny {L} \normalsize = 0$)
2. It can overfit if you have too many trees (chain gets too long - specialized stumps) - to further fight [[overfit(ting)]], [[eXtreme Gradient Boost (XGBoost)]] also adds [[L2-regularization]] of w 
