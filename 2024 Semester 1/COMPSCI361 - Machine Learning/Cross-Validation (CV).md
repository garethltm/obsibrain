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
		- t