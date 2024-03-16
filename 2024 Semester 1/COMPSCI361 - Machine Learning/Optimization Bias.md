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
- Consider a multiple-choice (a, b, c, d) test with 10 questions:
	- If you choose answers randomly, expected grade is 25% (no bias)
	- If you fill out 2 tests randomly & pick the best, expected grade is 33%
		- [[Optimization Bias]] of ~8%
	- If you take the best among 10 random tests, expected grade is ~47%
	- If you take the best among 100 random tests, expected grade is ~62%
	- ...
- Model will overfit $\rightarrow$ You have more choices
- But on new questions the random choice accuracy is still 25%
- If we instead used a 100-question test then:
	- Expected grade from best over 1 randomly-filled test is 25%
	- Expected grade from best over 2 randomly-filled test is ~27%
	- Expected grade from best over 10 randomly-filled test is ~32%
	- Expected grade from best over 100 randomly-filled test is ~36%
	- ...
- The [[Optimization Bias]] grows with the number of things we try
	- Complexity of the set of models we search over
- But, [[Optimization Bias]] shrinks quickly with the number of examples
	- But it's still non-zero & growing if you over-use your [[Validation set(s)]]

## [[Validation Error]] & [[Optimization Bias]]
- [[Optimization Bias]] is small if you only compare a few models
	- Best [[Decision Tree(s)]] on the training set among depths: 1, 2, 3,..., 10
	- Risk of [[2024 Semester 1/COMPSCI361 - Machine Learning/Overfitting|Overfitting]] to [[Validation set(s)]] is low if we try 10 things
- [[Optimization Bias]] is large if you compare a lot of models
	- All possible [[Decision Tree(s)]] of depth 10 or less
	- Here we are using the [[Validation set(s)]] to pick between a billion+ models
		- Risk of [[2024 Semester 1/COMPSCI361 - Machine Learning/Overfitting|Overfitting]] to [[Validation set(s)]]: could have low [[Validation Error]] by chance
	- If you did this, you might want to have a second [[Validation set(s)]] to detect [[2024 Semester 1/COMPSCI361 - Machine Learning/Overfitting|Overfitting]]
- [[Optimization Bias]] shrinks as you grow size of [[Validation set(s)]]
	- More data = 'Better'

## [[Optimization Bias]] leads to Publication Bias
- Suppose that 20 researches perform the exact same experiment
- They each test whether if their effect is significant (p < 0.05)
	- $\frac{19}{20}$ find that it is not significant
	- But maybe that 1 group finding it significant publishes a paper about the effect
- This is again [[Optimization Bias]], contributing to publication bias
	- A contributing factor to many reported effects being wrong