Procedure monotonically decreases the [[Training error]]
- As long as not all $\huge w\tiny {L} = 0$ (prediction = 0), each tree decreases [[Training error]] 
	- continues to improve as long as the predictions are not equal to 0

## Can it overfit?
1. It can overfit if trees are too deep or you have too many trees
2. To further fight [[overfit(ting)]], [[eXtreme Gradient Boost (XGBoost)]] also adds L2-regularization of w