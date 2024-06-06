[[gradient]]s are calculated in the [[Backpropagation]] process to update the weights in the desired direction
## Vanishing gradients:
caused by multiplying values ([[2024 Semester 1/COMPSCI361 - Machine Learning/chain rule|chain rule]])
- where the values decreases through the multiplication of decimals
	- #compsci361example 0.1 $\rightarrow$ 0.001,...
[[gradient]]s become smaller & smaller and can become close to 0
- this can slow down or stop the learning process (very small weights' update)
- 