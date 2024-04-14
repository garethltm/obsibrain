In this context, [[Imbalanced Data]] refers to an imbalanced class distribution

#compsci361example if there are far more 1s than 0s in the class
### Potential Problem
1. Problems with evaluation
	- Accuracy = $\frac {TP + TN}{P+N}$
		- because you may be wrong for the minority class
	- Alternative: [[Precision (Exactness)]]-[[Recall (Completeness)]], [[ROC Curves]]
2. [[classifier(s)]] try to reduce the overall error so they could over-predict the majority class