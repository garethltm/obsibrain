- We use [[Validation Error]] when:
	- How do we decide [[Decision Tree(s)]] depth?
	- We care about [[Test error]]
	- But we can't look at test data

1. Use part of training data to approximate [[Test error]]
2. Split training examples into training set & validation set:
	1. Train model based on training data
	2. Test model based on validation data

![[Pasted image 20240313170341.png]]
1. Train: 
	- model = train($X_{train}$, $Y_{train}$)
2. Predict: 
	- $\hat{y}$ = predict(model, $X_{validate}$)
3. Validate: 
	1