In this context, [[Imbalanced Data]] refers to an imbalanced class distribution
- when you have skewed distribution$\rightarrow$ you must not [[overfit(ting)]]
	- because learning algorithms are more prone to predict the majority class

#compsci361example if there are far more 1s than 0s in the class
### Potential Problem
1. Problems with evaluation
	- Accuracy = $\frac {TP + TN}{P+N}$
		- because you may be wrong for the minority class
	- Alternative: [[Precision (Exactness)]]-[[Recall (Completeness)]], [[ROC Curves]]
2. [[classifier(s)]] try to reduce the overall error so they could over-predict the majority class
## Sampling the data
Under- & Over-sampling with replacement can significantly improve the prediction of the minority class
1. Randomly under-sampling the majority class
	- Randomly removes instances from the majority class
	- Balances the dataset
	- Discarded observations could have important information
	- Can introduce bias
1. Randomly over-sampling the minority class
	- Randomly add more instances from the minority class
	- No information loss
	- Risk of [[overfit(ting)]]