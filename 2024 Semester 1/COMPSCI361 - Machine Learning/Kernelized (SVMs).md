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
- this will give you the [[support vectors]]1. $$ w = \sum_{i \in S} \alpha_i \phi(x_i) $$
2. $$ b = \frac{1}{|S|} \sum_{i \in S} y_i (w \cdot \phi(x_i)) $$

