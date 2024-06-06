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
### Loss Functions
#### Definition
difference between the actual value and predicted value
$$l(y^{(i)},\hat{y}^{(i)} )$$
#compsci361example 
- $y^{(i)}$ = [1]
- $\hat{y}^{(i)}$ = [-1]
For every [[training data]] we has a Loss Function that we sum up to get an overall loss value
- For every $w$, we could have a loss value
This is used to quantify the difference between the output labels ($\hat{y}$) & true labels
#### Goal
Quantify the differences of outputs compared with labels (target)
![[empirical risk]]
#compsci361example ![[Pasted image 20240606144848.png]]
## Optimisation
Given a set of [[training data]] $S = \{ (x^{(1)}, y^{(1)}), \ldots, (x^{(n)}, y^{(n)}) \}$
- $y^{(i)}$ is categorical: [[classification]] task ([[multi-class classification]] or binary)
- 