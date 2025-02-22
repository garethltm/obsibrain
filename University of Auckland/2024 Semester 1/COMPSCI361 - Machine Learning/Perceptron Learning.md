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
[[Stochastic Gradient Descent (SGD)]] + [[University of Auckland/2024 Semester 1/COMPSCI361 - Machine Learning/chain rule|chain rule]] = [[Backpropagation]]
- [[University of Auckland/2024 Semester 1/COMPSCI361 - Machine Learning/chain rule|chain rule]]: to calculate the gradient with respect to weight
- [[Gradient descent]]: Update the [[parameters]] in the direction of "maximum descent" in the [[Loss Function]] across all points
- [[Stochastic Gradient Descent (SGD)]]: update the weight for every instance
- Mini-batch [[Stochastic Gradient Descent (SGD)]]: update over min-batches of instances
## Gradient Descent
1. Initialize the weights $w=(w_0,w_1,\dots,w_d)$
2. Repeat
	- For each training example ($x^{(i)},y^{(i)}$)
	- Compute $\hat {y}^{(i)}$
	- Compute the derivative of the [[Loss Function]]
	- Update the weights (only if $\hat {y}^{(i)} \ne y^{(i)}$) using [[Weight Update Formula]]
		![[Pasted image 20240606155445.png]]
		- $w\leftarrow w - \lambda (derivative\ of\ Hinge Loss)$ 
		- $w\leftarrow w - \lambda (- y^{(i)} x^{(i)} )$
		- $w\leftarrow w + \lambda ( y^{(i)} x^{(i)})$
			- [[Hinge Loss]]
		- $k$ represents the iteration number
		- $\lambda$ represents the [[Learning rate]] (step size)
3. Until change of $w_j \le \ threshold$

#compsci361example ![[Pasted image 20240606155701.png]]
## Types of [[Gradient descent]]
![[Pasted image 20240606160203.png]]![[Pasted image 20240606160226.png]]
1. [[Batch Gradient Descent (BGD)]]
	- computes the [[Loss Function]] with respect to all [[parameters]] on all [[training data]]
2. [[Stochastic Gradient Descent (SGD)]]
	- small batches of [[training data]] being picked
	- [[Stochastic Gradient Descent (SGD)]] direction is very jagged compared to [[Batch Gradient Descent (BGD)]] or mini-batch
## Summary

|                                          | [[Batch Gradient Descent (BGD)]]                                                                                                         | [[Stochastic Gradient Descent (SGD)]]                                                                                                                 |
| ---------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Algorithm**                            | Computes the gradient of the cost function with respect to the model [[parameters]] using the entire [[training data]] in each iteration | Computes the gradient using a small subset of examples in each iteration                                                                              |
| **Convergence Speed**                    | Takes longer to converge since it computes the gradient using the entire [[training data]] in each iteration                             | Can converge faster since it updates the model [[parameters]] after processing each example                                                           |
| **Convergence Accuracy**                 | More accurate since it computes the gradient using the entire [[training data]]                                                          | Less accurate since it computes the gradient using a subset of examples, which can introduce more [[Noise]] and [[variance]] in the gradient estimate |
| **Computation & Memory Requirements**    | More Computation and Memory since it needs to process the entire [[training data]] in each iteration                                     | Less Computation and Memory since it only needs to process a single example or a small subset of examples in each iteration                           |
| **Optimization of Non-Convex Functions** | Can get stuck in local minima                                                                                                            | More suitable for optimizing non-convex functions since it can escape local minima and find the global minimum                                        |
- [[Batch Gradient Descent (BGD)]] is not as practical in the real world