[[gradient]]s are calculated in the [[Backpropagation]] process to update the weights in the desired direction
## 1. Vanishing gradients (< 1)
caused by multiplying values ([[University of Auckland/2024 Semester 1/COMPSCI361 - Machine Learning/chain rule|chain rule]])
- where the values decreases through the multiplication of decimals
	- #compsci361example 0.1 $\rightarrow$ 0.001,...
**Gradients become smaller & smaller and can become close to 0**
- this can slow down or stop the learning process (very small weights' update)
- $$out_{zj} = g(Σ_iw_{i,j}x_i + b_j)$$$$out_{zj}' = g'(Σ_iw_{i,j}x_i + b_j)\cdot x_i$$
	([[University of Auckland/2024 Semester 1/COMPSCI361 - Machine Learning/chain rule|chain rule]])
	If $g'()$ is close to 0, then the value of the [[gradient]] comes smaller and smaller as [[Backpropagation]] processes back to the initial layers (significant for large [[Neural Network (NN)]])
## 2. Exploding gradients (>1)
can become exponentially large if term is larger than 1
**Gradients become larger and large as [[Backpropagation]] progresses**
- Learning can become unstable (large weights update) and diverge
## Solution
choosing the correct [[Activation Function]]
![[Pasted image 20240607012602.png]]
As the number of layers goes up, the [[gradient]] is more likely to vanish during [[Backpropagation]]
- Using ReLU [[Activation Function]] instead of $tanh$ or [[Sigmoid Function]] can reduce this problem since its [[gradient]] does not go to zero as the input goes to zero
- [[Sigmoid Function]] and $Tanh$ functions saturates at 0 or 1 when inputs become small or large