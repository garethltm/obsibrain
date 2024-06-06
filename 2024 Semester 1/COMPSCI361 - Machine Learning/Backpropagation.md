Going backwards to get gradient
## Definition
Modifications are made in the "backwards" direction
- From the output layer, through each hidden layer down to the 1st hidden layer
## Training
Iteratively process a set of training tuples & compare the network's prediction with the actual known target value
#### [[Loss Function]]
For each training tuple, the weights are modified to minimize the loss between the network's prediction & actual target value, say mean squared error
- we compare the differences of the output of the [[Neural Network (NN)]] with the target labels
- adjust weight to minimize [[Loss Function]]
- [[empirical risk]] for all [[training data]]
## Steps
**Random initialization of weights**
- For each training instance:
	1. Make a prediction (forward pass/propagation) 
	2. Measure the error/loss (to calculate the [[Loss Function]])
	3. Go through each layer in reverse to measure the [[error contribution]] from each connection (backward pass/propagation)
	4. Slightly tweak the connection weights to reduce the error ([[Stochastic Gradient Descent (SGD)]] step)
Until stopping criterion is reached

#compsci361example 
![[Pasted image 20240606175452.png]]![[Pasted image 20240606175511.png]]
### 1. Initialization of weights (random weight initialization)
	![[Pasted image 20240606175603.png]]
### 2. Forw