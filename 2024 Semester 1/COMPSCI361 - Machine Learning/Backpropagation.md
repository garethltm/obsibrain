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
### 2. Forward propagation
	![[Pasted image 20240606232924.png]]![[Pasted image 20240606232933.png]]
### 3. Calculating total error (Calculating the [[Loss Function]])
	![[Pasted image 20240606233038.png]]- Square [[Loss Function]]$$E({y}, \hat{{y}}) = \frac{1}{2} \| {y} - \hat{{y}} \|^2$$
	![[Pasted image 20240606233338.png]]
### 4. [[Backpropagation]] (output layout)
	![[Pasted image 20240606233459.png]]![[Pasted image 20240606233511.png]]
		- [[2024 Semester 1/COMPSCI361 - Machine Learning/chain rule|chain rule]]
		Checking how each weight influences the error $\rightarrow$ inclusive offset values
	1. [[Backpropagation]]![[Pasted image 20240606233647.png]]![[Pasted image 20240606233708.png]]![[Pasted image 20240606233718.png]]
	2. [[Backpropagation]]![[Pasted image 20240606233757.png]]![[Pasted image 20240606233810.png]]
		[[Activation Function]] - [[Sigmoid Function]]
	3. [[Backpropagation]]![[Pasted image 20240606233846.png]]![[Pasted image 20240606233900.png]]
	4. [[Backpropagation]]![[Pasted image 20240606233917.png]]![[Pasted image 20240606233932.png]]![[Pasted image 20240606234130.png]]
	5. [[Backpropagation]]![[Pasted image 20240606234223.png]]