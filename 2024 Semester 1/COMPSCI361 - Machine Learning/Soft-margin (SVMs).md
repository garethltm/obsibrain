![[Pasted image 20240605104139.png]]
![[Pasted image 20240605225310.png]]
[[Soft-margin (SVMs)]] selects the maximum margin linear [[classifier(s)]] with partial misclassifications allowed
## Soft-margin Maximization
Given a set of [[training data]] $S = ((x_1, y_1), \ldots, (x_n, y_n)), y_i \in \{+1, -1\}$
#### Goal
The [[Soft-margin (SVMs)]] algorithm aims to find a linear [[classifier(s)]] that
1. Maximises ($\gamma$) the margin on $S$ (on all [[training data]]) and
2. Minimise the misclassification error ($\left( C \sum_{i=1}^{n} \xi_{i} \right)$)
	- the new parameter $\xi$ denotes the degree of the errors of each [[training data]]
	- each [[training data]] has $\xi_i$ associated with it
		![[Pasted image 20240606121947.png]]
#### Definition
[[Soft-margin (SVMs)]] introduce a misclassification penalty ($C$) controls the trade-off between
1. Maximizing the margin (same as [[Hard-margin (SVMs)]])
2. Minimizing the loss
Primal formulation for the soft-margin
$$
\min_{w, b} \frac{\| \mathbf{\vec {w}} \|}{2} + C \sum_{i=1}^{n} \xi_{i}
$$
- representing the minimization of the loss 
$$y_i (\mathbf{\vec{w}} \cdot \vec {x_i} + b) \geq 1 - \xi_i, \quad i = 1, 2, \ldots, n, \quad \xi_i \geq 0
$$
1. If $(\mathbf{w} \cdot \mathbf{x}_i + b)y_i \geq 1$ then $\xi_i = 0$ (if correctly classified)
2. If $(\mathbf{w} \cdot \mathbf{x}_i + b)y_i < 1$ then $\xi_i = 1-(\mathbf{w} \cdot \mathbf{x}_i + b)y_i$ (if wrongly classified, we want to penalise)
##### [[Slack Variables]]
![[Pasted image 20240605234014.png]]

#compsci361example ![[Pasted image 20240605234454.png]]![[Pasted image 20240605234504.png]]
## Bias & Variance
![[Pasted image 20240605234846.png]]
1. A large value of C keeps the errors small at the cost of a reduced margin (can lead to [[overfit(ting)]], low bias, high variance)
2. A small value of C allows more misclassification while increasing the margin on the remaining examples (can lead to underfitting, large bias, low variance)

#compsci361questions 
1. How do we recover [[Hard-margin (SVMs)]] from [[Soft-margin (SVMs)]]?
	- Set misclassification penalty $C$ = $\infty$ (as long as large - using the [[Hard-margin (SVMs)]])
2. Given [[Linearly Separable Data]], we train a [[Hard-margin (SVMs)]] & find out that the margin is so small that the model becomes prone to [[overfit(ting)]]. How would you resolve the [[overfit(ting)]] issue?
	- We can opt for a larger margin by using [[Soft-margin (SVMs)]] in order to help the model generalize better