- ROC (Receiver Operating Characteristics) curves
	- for visual comparisons of classification models

- Originated from signal detection theory
- Shows the trade-off between:
	- true positive rate TPR = $\frac{TP}{TP+FN}$
	- false positive rate FPR = $\frac{FP}{FP+TN}$
- how many negatives labelled as positives

The area under the [[ROC Curves]] (AUC: Area Under Curve, also AUROC) is a measure of the accuracy of the model

Rank the test tuples in decreasing order:
- the one that is most likely to belong to the positive class appears at the top of the list
The closer to the diagonal line (ie. the closer the area is to 0.5), the less accurate the model

![[Pasted image 20240322005120.png]]