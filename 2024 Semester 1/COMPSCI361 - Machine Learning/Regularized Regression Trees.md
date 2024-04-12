Procedure monotonically decreases the [[Training error]]
- As long as not all $\huge w\tiny {L} \normalsize = 0$ (prediction = 0), each tree decreases [[Training error]] 
	- continues to improve as long as the predictions are not equal to 0

## Can it overfit?
1. It can overfit if trees are too deep - to restrict depth, add [[L0-regularization]] (stop splitting if $\huge w\tiny {L} \normalsize = 0$)
	$$f(\huge {w}\tiny{1}\normalsize ,\huge {w}\tiny{2}\normalsize ,...)=\displaystyle\sum_{i=1}^n (\huge {w}\tiny{Li}\normalsize - \huge{r}\tiny{i}\normalsize )^2 + \lambda \tiny{0}\normalsize ||w||\tiny {0}$$
	- $\lambda \tiny{0}\normalsize ||w||\tiny {0}$ = minimise number of leaves
		Only split if you decrease squared error by $\lambda \tiny{0}$
1. It can overfit if you have too many trees  (chain gets too long) - to further fight [[overfit(ting)]], [[eXtreme Gradient Boost (XGBoost)]] also adds L2-regularization of w- specialized stumps
	$$f(\huge {w}\tiny{1}\normalsize ,\huge {w}\tiny{2}\normalsize ,...)=\displaystyle\sum_{i=1}^n (\huge {w}\tiny{Li}\normalsize - \huge{r}\tiny{i}\normalsize )^2 + \lambda \tiny{0}\normalsize ||w||\tiny {0}\normalsize + \lambda \tiny{2}\normalsize ||w||^2$$
	- $\lambda \tiny{2}\normalsize ||w||^2$ = minimise number of trees