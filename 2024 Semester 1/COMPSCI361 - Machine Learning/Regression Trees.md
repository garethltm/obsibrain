[[Regression Trees]] used in [[eXtreme Gradient Boost (XGBoost)]]
- each split is based on 1 feature
- each leaf gives a real-valued prediction (a [[Regression]] value of a target)
- #compsci361example How many hours of video games per day?![[Pasted image 20240412165234.png]]

### How can we fit a [[Regression Trees]]?
###### Simple approach:
1. Predict: at each leaf, predict the mean of the training $\huge {y}\tiny {i}$ assigned to the leaf (the leaf (mode) is the prediction)
	- Weight $\huge {w}\tiny {L}$ at leaf L is set to mean($\huge {y}\tiny {i}$) among $\huge {y}\tiny {i}$ 