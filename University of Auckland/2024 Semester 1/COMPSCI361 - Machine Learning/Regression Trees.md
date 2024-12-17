[[Regression Trees]] used in [[eXtreme Gradient Boost (XGBoost)]]
- each split is based on 1 feature
- each leaf gives a real-valued prediction (a [[Regression]] value of a target)
- #compsci361example How many hours of video games per day?![[Pasted image 20240412165234.png]]

#compsci361questions 
### How can we fit a [[Regression Trees]]?
###### Simple approach:
1. [[Boosted Regression Trees - Prediction]]: at each leaf, predict the mean of the training $\huge {y}\tiny {i}$ assigned to the leaf (the leaf (mode) is the prediction)
	- Weight $\huge {w}\tiny {L}$ at leaf L is set to mean($\huge {y}\tiny {i}$) among $\huge {y}\tiny {i}$ at the lead node
2. [[Boosted Regression Trees - Training]]: set the $\huge {w}\tiny {L}$ values by minimizing the squared error ([[Linear Regression]])
$$f(\huge {w}\tiny{1}\normalsize ,\huge {w}\tiny{2}\normalsize ,...)=\displaystyle\sum_{i=1}^n (\huge {w}\tiny{Li}\normalsize - \huge{y}\tiny{i}\normalsize )^2$$
- Same speed as fitting [[Decision Tree(s)]] from earlier in the semester
	- Use mean instead of mode, & use squared error instead of accuracy/infogain (in relation to [[AdaBoost]] of the training of the tree)
- Use greedy strategy for growing tree