## Illustration
![[Pasted image 20240606142249.png]]
## Architecture
It is possible to have multiple structures of neurons
![[Pasted image 20240606142350.png]]
- Network topology
- Number of units in the input layer
- Number of hidden layers (if > 1)
- Number of units in each hidden layer
- Number of connections between layers
- Number of units in the output layer
## Function
- maps input to output
- contains [[parameters]] to be learned
#### Output
$$\hat {y}=f(\sum_{j} w_{j}x_{j} + b)$$
### [[Activation Function]] $f(\cdot)$
- to control output of neurons to a certain range
- Applied to the weighted sum ($\sum_{j} w_{j}x_{j} + b$)
	#compsci361example ![[Pasted image 20240606143408.png]]
### [[Loss Function]]

## Optimisation
Given a set of [[training data]] $S = \{ (x^{(1)}, y^{(1)}), \ldots, (x^{(n)}, y^{(n)}) \}$
- $y^{(i)}$ is categorical: [[classification]] task ([[multi-class classification]] or [[binary classification]])
- $y^{(i)}$ is continuous: [[Regression]] task
## Goal
FInd $w$, such that [[empirical risk]] is minimized (smallest loss) on all [[training data]]
$$
L(w) = \frac{1}{n} \sum_{i} l(y^{(i)}, \hat{y}^{(i)})
$$
$$
\hat{y}^{(i)} = sign(x^{(i)},w) =\text{sign}(\sum_{j} w_j x_j^{(i)} + b)
$$
- this is used to make a prediction [-1, 1]
- $n$ represents [[Normalization]], this is used to organize for all $n$
	- so that $w$ can be used for all sizes of the dataset
## Solution
[[Stochastic Gradient Descent (SGD)]] + chain rule = [[Backpropagation]]
## Gradient Descent
1. Initialize the weights $w=(w_0,w_1,\dots,w_d)$
2. Repeat
	- For each training example ($x^{(i)},y^{(i)}$)
	- Compute $\hat {y}^{(i)}$
	- Compute the derivative of the [[Loss Function]]
	- Update the weights (only if $\hat {y}^{(i)} \ne y^{(i)}$)
		- $w\leftarrow w - \lambda (derivative\ of\ Hinge Loss)$ 
		- $w \leftarrow w - \lambda (- y^{(i)} x^{(i))$
		- 
		- [[Hinge Loss]]
		- $k$ represents the iteration number
		- $\lambda$ represents the learning rate (step size)
3. Until change of $w_j \le \ threshold$
4. 