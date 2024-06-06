![[Pasted image 20240606164308.png]]
- The inputs to the network correspond to the attributes measured for each training tuple
	- Inputs are then weighted and fed simultaneously to a ***Hidden Layer***
- The number of ***Hidden Layer*** is arbitrary
	- you can define the number of black neurons
- The network is [[feed-forward]]

Every node in a ***Hidden Layer*** operates on activations preceding layer & transmits activations forward to nodes of next layer
$$h=g(W^{(1)}x+b^{(1)})$$
- $h$ represents the activation value
- $g$ represents the [[Activation Function]]
- $(W^{(1)}x+b^{(1)})$ represents the Linear Predictor
Each neuron, we need to define the [[Activation Function]]
**NOTE**: Make sure [[Normalization]] ovvu

Networks perform non-[[Linear Regression]]:
- Given enough units & enough training samples, they can closely approximate any [[Continuous Space (Continuous Functions)]]
	- ([[Neural Network (NN)]] is an universal approximator)
## Architecture
- A two-layer [[Neural Network (NN)]]
## [[Activation Function]]
- $g$ represents the Nonlinear transformation
	- #compsci361example [[Sigmoid Function]] transformation
## *Hidden Layer*
We sum the inputs being fed into a single neuron
- $h=g(W^{(1)}x+b^{(1)})$
## Output layer
- $o=g(W^{(2)}h+b^{(2)})$
$W$ represents the Weight Matrix
$b$ represents the Bias Term
## Important
The more layers we have the more $W$ we have
- the more complex the [[Neural Network (NN)]]
**More neurons = more [[parameters]] $\rightarrow$ more approximation abilities on how to make a network more powerful**