- Another name for [[2024 Semester 1/COMPSCI361 - Machine Learning/Overfitting|Overfitting]]
	- How biased is an error that we optimized over many possibilities?
- [[Optimization Bias]] of [[parameters]] learning
	- During learning, we could search over tons of different [[Decision Tree(s)]]
	- So we can get lucky & find 1 with low [[training error]] by chance
		- [[2024 Semester 1/COMPSCI361 - Machine Learning/Overfitting|Overfitting]] of the [[training error]]
- [[Optimization Bias]] of [[hyperparameter(s)]] tuning
	- Here, we might optimize the [[Validation Error]] over 20 values of depth
	- 1 of the 20 trees might have low [[Validation Error]] by chance
		- [[2024 Semester 1/COMPSCI361 - Machine Learning/Overfitting|Overfitting]] of the [[Validation Error]]

#compsci361example 
- Consider a multiple-choice (a)