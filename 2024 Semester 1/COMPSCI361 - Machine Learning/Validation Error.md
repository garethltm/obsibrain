- We use [[Validation Error]] when:
	- How do we decide [[Decision Tree(s)]] depth?
	- We care about [[test error]]
	- But we can't look at test data

1. Use part of training data to approximate [[test error]]
2. Split training examples into training set & validation set:
	1. Train model based on training data
	2. Test model based on validation data

![[Pasted image 20240313170341.png]]
1. Train: 
	- model = train($X_{train}$, $Y_{train}$)
2. Predict: 
	- $\hat{y}$ = predict(model, $X_{validate}$)
3. Validate: 
	- error = $\sum (\hat{y} \not{=}\ y_{validate})$ 
- Note: if examples are ordered, split should be random

[[Independent & Identically Distributed (IID)]] data: [[Validation Error]] is unbiased approximation of [[test error]]
$\epsilon (E_{valid})$ = $\epsilon (E_{test})$

#compsci361example 
- Course analogy
	- You have 2 practice exams
	- You hide 1 exam, & spend a lot of time working through the other
	- You then do the other practice exam, to see how well you'll do the test
- We typically use [[Validation Error]] to choose "hyperparameters"