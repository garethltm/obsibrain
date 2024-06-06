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
