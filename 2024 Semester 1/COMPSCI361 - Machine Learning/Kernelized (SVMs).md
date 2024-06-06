Given a set of [[training data]] $S = \{(x_1, y_1), ..., (x_n, y_n)\}, y_i \in \{+1, -1\}$
## Goal
The [[Kernelized (SVMs)]] algorithm aims to find a non-linear [[classifier(s)]], which is a separating [[hyperplane]]/[[hyperplanes]] in a higher dimensional space
## Approach
1. Transform the original input data into a higher dimensional space
2. Search for a [[Linearly Separable Data]] [[hyperplane]] in the new space
## Steps
#### Step 1: Space Transformation
$\Phi(\cdot)$: Transform the original input data into a higher dimensional space
![[Pasted image 20240606123251.png]]
- We can use a [[Hard-margin (SVMs)]] to derive a [[hyperplane]]
#### Step 2: Search for a Linearly Separating [[hyperplane]]
1. [[Dual Optimization Problem]]
2. [[Kernelized Optimization Problem]]
Solve the [[Kernelized Optimization Problem]] by [[Quadratic Programming (QP)]] 
- this will give you the [[support vectors]]$$
	\max_{\alpha} \sum_{i=1}^n \alpha_i - \frac{1}{2} \sum_{i=1}^n \sum_{j=1}^n \alpha_i \alpha_j y_i y_j \Phi(\vec{x}_i) \cdot \Phi(\vec{x}_j)$$

	subject to$$
	\alpha_i \geq 0 \quad \text{and} \quad \sum_{i=1}^n \alpha_i y_i = 0, \quad i = 1, 2, \ldots, n$$
