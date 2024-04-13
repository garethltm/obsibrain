### Problem![[Pasted image 20240413213542.png]]

### Solution
1. Fill in the missing data manually![[Pasted image 20240413213624.png]]
2. Fill in automatically (this is more feasible rather than the manual entry for large datasets) 
	1. a global constant (since they are all of the same type) ![[Pasted image 20240413213930.png]]
		- However, it might still work for [[Classification]] problem & it affects the class variable
	2. the attribute mean (more general case, where there are mixed values & continuous variable) ![[Pasted image 20240413214300.png]]
		- Done automatically by many implementations $\rightarrow$ Default assumption
		- Changes relationship with other variables $\implies$ bias in data (because you are calculating the mean based on a variable that may be dependent)
		- The mean is calculated based on observed values in that variable (you calculate the mean based on the available values at the end)
	3. the attribute mean of the samples belonging to the same class (replacing the value that has a similar target variable) - a **BETTER** way to do it![[Pasted image 20240413214545.png]]
		- Might change relationship with other variables other than class $\implies$ bias in data (we need to explore the whole data in such a way where we keep those underlying relations)
		- There might be relationship between X' & other features in combination (you are only looking at a single pairwise relationship)
	4. the most probable value (dividing the complete dataset into 2 parts) - **NOT TESTED** ![[Pasted image 20240413214838.png]]
		- Inference-based such as Bayesian formula, [[Decision Tree(s)]], [[k-nearest neighbour (KNN)]],...
	- IDEA: Any model that can be used for [[Supervised Learning]] can be used here
## Imputation as matrix completion problem
- useful for high-dimensional, sparsely populated datasets
#### Matrix factorization approaches
- you assume there is some kind of **hidden space** in which you can project your original dataset - some hidden variables that influence your dataset
		![[Pasted image 20240413220237.png]]
	 - Decompose the data matrix $X$ such that $X\tiny {n\times d}\normalsize = (U\tiny {n\times k}\normalsize )(V\tiny {k\times d})$ such that the product $U\times V = X'$ recovers the original matrix
		 - n = number of instances
		 - d = number of dimensionality/features
		 - we want to find the k
	- [[Low-rank matrix]] approximation $X'$, with $k\leq min(n,d)$ factors
		- #compsci361example movie genres in per-use movie-preference data
		- we want the lowest possible (k), we want to further reduce the amount of dimensions
		- Well suited for larger datasets with high levels of sparsity (as in recommender systems)
	![[Pasted image 20240413221011.png]]
	- Minimise the sum of squared errors (over the observed elements of X), as evaluated on a hold-out dataset
	- Finding that 1 or 2 features that drive the relationship in the dataset (you don't need all the features)
	- Max number of factors is the dimensionality of your input space
## Multiple Iterations of [[Imputation]]
1. [[Expectation Maximization (EM) Imputation]]
2. [[Multiple imputation by chain equations (MICE)]]
- There is no best approach (No Free Lunch Theorem) - use an approach that could work in the most restrictive way not