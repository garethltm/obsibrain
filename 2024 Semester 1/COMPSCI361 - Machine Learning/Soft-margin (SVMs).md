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
	- ![[Pasted image 20240605233151.png]]
#### Definition
[[Soft-margin (SVMs)]] introduce a misclassification penalty ($C$) controls the trade-off between
1. Maximizing the margin (same as [[Hard-margin (SVMs)]])
2. Minimizing the loss
Primal formulation for the soft-margin
$$
\min_{w, b} \frac{\| \mathbf{w} \|^2}{2} + C \sum_{i=1}^{n} \xi_{i}
$$
y_i (\mathbf{w} \cdot \mathbf{x}_i + b) \geq 1 - \xi_i, \quad i = 1, 2, \ldots, n, \quad \xi_i \geq 0
$$\]$$
