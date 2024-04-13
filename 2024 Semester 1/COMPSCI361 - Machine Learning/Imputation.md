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
### Imputation as matrix completion problem