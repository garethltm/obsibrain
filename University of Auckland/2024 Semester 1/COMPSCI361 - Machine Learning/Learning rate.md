we need to choose just-right [[Learning rate]]
## Motivation
[[Gradient descent]] is an optimization algorithm that finds the local minimum of a function by taking "steps" in the direction of the negative of the [[gradient]]

#compsci361questions 
## What will happen if we use a [[Learning rate]] that is too small or too large?
- too small $\rightarrow$ longer time to find optimum
- Learning efficiency, optimization accuracy
- #compsci361example learning steps that were taken to find the local minimum of a function![[Pasted image 20240607011303.png]]
## [[Learning rate]] decay schedule
- Common practice
	- decrease [[Learning rate]] over time ([[Learning rate]] decay)
		- gradually make the [[Learning rate]] smaller to easily fine-tune the model
	- #compsci361example linear decay
- Linear decay for set number of iterations and then constant
## Adaptive [[Learning rate]] strategies
Monitors the model's performance & adapt the [[Learning rate]] in response
1. Reduces [[Learning rate]] when performance plateaus
2. Increases [[Learning rate]] when performance does not improve for a number of iterations
