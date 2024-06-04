Given a set of linearly separable [[training data]] $S = \{(x_1, y_1), ..., (x_n, y_n)\}, y_i \in \{+1, -1\}$
We want to find a [[hyperplane]]
There is an infinite number of lines ([[hyperplane]](s)) separating the 2 classes
![[Pasted image 20240605104722.png]]
## Goal
The [[Hard-margin (SVMs)]] algorithms aims to find a linear [[classifier(s)]] that maximises ($\gamma$) the margin on $S$
- We want to find the one that is as far away as possible from the [[training data]] 
	- largest margin from the middle [[hyperplane]]
## Why?
Any linear [[classifier(s)]] that separates $S$ correctly will have margin $\gamma > 0$
We want to find the best one (the one that minimizes [[classification]] error on unseen data)
#### Assumption
- the [[hyperplane]] with the largest margin will generalise best on unseen data
[[Support Vector Machines (SVM)]] searches for [[hyperplane]] with largest margin
- [[Maximum Margin Hyperplane (MMH)]]
- [[Generalization Performance]]