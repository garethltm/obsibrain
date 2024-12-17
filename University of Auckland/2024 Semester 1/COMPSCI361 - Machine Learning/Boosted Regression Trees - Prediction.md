Consider an [[Ensemble(s)]] of [[Regression Trees]]
- For an example i, they each make a continuous prediction![[Pasted image 20240412171141.png]]

[[eXtreme Gradient Boost (XGBoost)]], final prediction is the sum of individual predictions![[Pasted image 20240412171212.png]]

We are not using the mean as we would with [[Random Forests]]
- In [[Boosting]], each tree is not individually trying to predict the true $\huge {y}\tiny {i}$ value (we assume they underfit)
- Instead, each new tree tries to fix the prediction make by the old trees, so that sum is $\huge {y}\tiny {i}$![[Pasted image 20240412171451.png]]


