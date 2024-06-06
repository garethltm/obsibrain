![[Pasted image 20240606164308.png]]
## Architecture
- A two-layer network
## [[Activation Function]]
- $g$ represents the Nonlinear transformation
	- #compsci361example [[Sigmoid Function]] transformation
## Hidden Layer
We sum the inputs being fed into a single neuron
- $h=g(W^{(1)}x+b^{(1)})$
## Output layer
- $o=g(W^{(2)}h+b^{(2)})$
$W$ represents the Weight Matrix
$b$ represents the Bias Term

## Important
The more layers we have the more $W$ we have
- the more complex the [[Neural Network (NN)]]
More neurons = more [[parameters]] $\rightarrow$ 