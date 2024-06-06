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
1. Calculate the weights size
	- Sum of the absolute values of the weights $\rightarrow$ L1

