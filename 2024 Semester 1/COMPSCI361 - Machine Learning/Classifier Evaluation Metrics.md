[[Confusion Matrix]]

1. Classifier accuracy or recognition rate
	- Percentage of test set tuples that are correctly classified
	- $Accuracy = \frac{(TP + TN)}{All}$
2. Precision (Exactness):
	- what % of tuples that the [[Classifier]] labelled as positive are actually positive? (Checking reliance)
	- $Precision = \frac{TP}{TP+FP}$
3. Recall (Completeness):
	- what % of positive tuples did the [[Classifier]] label as positive?
	- $Recall = \frac{TP}{TP+FN}$
- There is an inverse relationship between precision & recall