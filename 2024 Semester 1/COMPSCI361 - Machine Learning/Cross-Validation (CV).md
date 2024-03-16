- 5-fold [[Cross-Validation (CV)]]
	- Train on 80% of the data, validate on the other 20%
	- Repeat this 5 more times with different splits & average the score![[Pasted image 20240316194613.png]]
	1. Train on folds 1, 2, 3, 4 compute error on fold 5
	2. Train on folds 1, 2, 3, 5 compute error on fold 4
	3. Train on folds 1, 2, 4, 5 compute error on fold 3
	4. ...
	6. Take the average of the 5 errors as approximation of [[test error]]![[Pasted image 20240316194759.png]]
	- [[Cross-Validation (CV)]] error estimate for this [[hyperparameter(s)]] mean(errors) = 0.16
		- Using every part of the dataset

- k-fold [[Cross-Validation (CV)]]
	- 10-fold [[Cross-Validation (CV)]]
		- Train on 90% of data & validate on 10%
			- Repeat 10 times & average (test on fold 1, then fold 2,... then fold 10)
	- Leave-one-out [[Cross-Validation (CV)]]
		- Train on all but 1 training example
			- Repeat n times & average
- Gets more accurate but more expensive with more folds
		- To choose depth we compute the [[Cross-Validation (CV)]] score for each depth
	- As before, if data is ordered then folds should be random splits
		- Randomize first, then split into fixed folds
	- Usually used in [[classification]]: stratified [[Cross-Validation (CV)]]
		- This enforces that class distribution in all folds is approximately the same as in the full data set