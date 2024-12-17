updates values after looking at each item in the training set to make steps right away
## Definition
Optimisation of the [[parameters]] (weights $w$ and biases $b$) to minimise a cost/[[Loss Function]]/error function
- #compsci361example the difference between actual value and predicted value

#compsci361example ![[Pasted image 20240606150700.png]]
## Steps
1. Perform update in downhill direction for each coordinate
	- The steeper the slope (the higher the derivative) the bigger the step for that coordinate
- #compsci361example ![[Pasted image 20240606150822.png]]
	##### **Idea**
	1. Start somewhere
	2. Repeat: Take a step in the [[steepest direction]] (descent)![[Pasted image 20240606151114.png]]
		![[Pasted image 20240606151447.png]]
	- $\lambda$: [[Learning rate]]
		- [[hyperparameter(s)]] that needs to be chosen carefully
	1. If too high $\rightarrow$ chance to miss the optimum
	2. If too low $\rightarrow$ very long time
