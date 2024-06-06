penalises large weight values
- keeping weights close to zero for some neurons (simplify the structure of the [[Neural Network (NN)]])
![[Pasted image 20240607000005.png]]![[Pasted image 20240607000021.png]]
#### Purpose of [[Regularisation]]
- Large weights:
	- are characteristic of more complex models (higher learning time)
	- can be a sign of an over-specialized network ([[overfit(ting)]])
	- make the network unstable (sensitive to [[Noise]])
## Why use it?
- Penalises/constraints the weight values towards 0
	- a "weight shrinkage" or a "penalty against complexity"
	- Encourages
## How does it work?
### L1 and L2 norms
$$ \| \mathbf{w} \|_1 = |w_1| + |w_2| + \dots + |w_N| $$
$$| \mathbf{w} \|_2 = \left( |w_1|^2 + |w_2|^2 + \dots + |w_N|^2 \right)^{\frac{1}{2}}$$
1. Calculate the weights size
	- L1: Sum of the absolute values of the weights $\rightarrow$ $\displaystyle \sum_{i=1}^{N} |w_i|$
	- L2: Sum of the squared values of the weights $\rightarrow$ $\displaystyle \sum_{i=1}^{N} w_i^2$
2. Apply [[Regularisation]] to the weight update
	- L1 [[Regularisation]]:
		- $Loss ={Error(y, \hat{y})} + \lambda \displaystyle \sum_{i=1}^{N} |w_i|$
	- L2 [[Regularisation]]:
		- $Loss ={Error(y, \hat{y})} + \lambda \displaystyle \sum_{i=1}^{N} {w_i}^2$
	- $Error(y, \hat{y})$ represents the minimisation of the errors (summation of the [[Loss Function]]) - also known as [[empirical risk]]
	- We are trying to minimise $|w_i|$ and ${w_i}^2$ by adding penalties to the weight values which prevents [[overfit(ting)]]
	- This will result in a loss function that is minimised on all the training data using [[Stochastic Gradient Descent (SGD)]]
	- A large $\lambda$ value increases the penalty on the weights, encouraging smaller weight values and thus more [[Regularisation]]