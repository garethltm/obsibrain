- Both decompositions serve the same purpose
	- Trying to evaluate how different factors affect [[test error]]
- They both lead to the same 3 conclusions
	1. Simple models can have high $E_{train}$ / bias, low $E_{approx}$ / variance
	2. Complex models can have low $E_{train}$ / bias, high $E_{approx}$ / variance
	3. As you increase n, $E_{approx}$ / variance goes down (for fixed complexity)![[Pasted image 20240312224429.png]]

#compsci361example 
A **decision tree** with a depth of 1 (also known as [[Decision Stumps]]) would typically have a **higher bias** than a tree with a depth of 5.

On the other hand, a decision tree with a depth of 5 is a more complex model. It can capture more details in the data and therefore typically has a **lower bias**. However, it’s important to note that while a more complex model like a depth-5 tree has a lower bias, it may have a higher variance, meaning it might overfit the training data and perform poorly on unseen data.

This is known as the **bias-variance tradeoff** in machine learning, and it’s a key concept when it comes to understanding model performance. The goal is to choose a model complexity that balances these two sources of error.

Related to: [[bias-variance decomposition]] & [[Fundamental Trade-Off]]