we need to choose just-right [[learning rate]]
## Motivation
[[Gradient descent]] is an optimization algorithm that finds the local minimum of a function by taking "steps" in the direction of the negative of the [[gradient]]

#compsci361questions 
## What will happen if we use a [[learning rate]] that is too small or too large?
- too small $\rightarrow$ longer time to find optimum
- Learning efficiency, optimization accuracy
- #compsci361example learning steps that were taken to find the local minimum of a function![[Pasted image 20240607011303.png]]
## [[learning rate]] decay schedule
- Common practice
	- decrease [[learning rate]] over time ([[learning rate]] decay)
		- gradually make the [[learning rate]] smaller to easily fine-tune the model
	- #compsci361example linear decay
- Linear decay for set number of iterations and then constant
## Adaptive learning rates strategies
- Monitors the model's performance & adapt the [[learning rate]] in response
- Reduces [[learning rate]] when performa
