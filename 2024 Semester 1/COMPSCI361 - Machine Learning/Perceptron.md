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
For every [[training data]] we have, a
#### Goal
Quantify the differences of outputs compared with labels (target)