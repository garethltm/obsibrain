[[gradient]]s are calculated in the [[Backpropagation]] process to update the weights in the desired direction
## 1. Vanishing gradients (< 1)
caused by multiplying values ([[2024 Semester 1/COMPSCI361 - Machine Learning/chain rule|chain rule]])
- where the values decreases through the multiplication of decimals
	- #compsci361example 0.1 $\rightarrow$ 0.001,...
**Gradients become smaller & smaller and can become close to 0**
- this can slow down or stop the learning process (very small weights' update)
- $$out_{zj} = g(Σ_iw_{i,j}x_i + b_j)$$$$out_{zj}' = g'(Σ_iw_{i,j}x_i + b_j)\cdot x_i$$
	([[2024 Semester 1/COMPSCI361 - Machine Learning/chain rule|chain rule]])
	If $g'()$ is close to 0, then the value of the [[gradient]] comes smaller and smaller as [[Backpropagation]] processes back to the initial layers (significant for large [[Neural Network (NN)]])
## 2. Exploding gradients (>1)
Gra