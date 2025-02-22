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

##### **Training**
Solve the [[Kernelized Optimization Problem]] by [[Quadratic Programming (QP)]] 
- this will give you the [[support vectors (SV)]]
		$$ \vec {w} = \sum_{x_i \in S} \alpha_i y_i \phi(\vec {x_i}) $$$$\vec {b} = \frac{1}{|SV|} \sum_{x_i \in S} y_i - (\vec {w} \cdot \phi(\vec {x_i})) $$
##### Testing
Determine the class label for a test point $\vec {z}$ by using the learned [[Kernelized (SVMs)]] ($\vec {w}$ and $\vec {b}$) with [[support vectors (SV)]]
$$
f(\vec {z}) = \text{sign}(\vec{w} \cdot \phi(\vec {z}) + b)
$$

$$
= \text{sign}\left(\sum_{x_i \in SV} \alpha_i y_i (\Phi(\vec {x_i}) \cdot \Phi(\vec{z})) + b\right)
$$
## [[Kernelized (SVMs)]] with [[Soft-margin (SVMs)]]/[[Hard-margin (SVMs)]]
#compsci361questions 
Which decision boundaries refer to [[Kernelized (SVMs)]]? (note: [[support vectors (SV)]] are represented by solid square/triangle)
![[Pasted image 20240606134110.png]]
## Advantages
1. Prediction accuracy is generally high
2. As compared to [[Bayesian Learning]] methods generally
3. Robust when training examples contain errors
4. Fast evaluation of the learned target function
5. [[University of Auckland/2024 Semester 1/COMPSCI361 - Machine Learning/Bayesian Networks|Bayesian Networks]] are normally slow
## Disadvantages
1. Long training time
2. Difficult to understand the learned function (weights)
3. [[University of Auckland/2024 Semester 1/COMPSCI361 - Machine Learning/Bayesian Networks|Bayesian Networks]] can be used easily for pattern discovery
4. Not easy to incorporate domain knowledge
5. Easy in the form of priors on the data or distributions
## Why [[Kernelized (SVMs)]] work?
####  Main Reason:
- It uses nonlinear mapping to transform the original [[training data]] into a higher dimension
	1. With the new dimension, it searches for the [[decision boundary]]
	2. With an appropriate nonlinear mapping to a sufficiently high dimension, data from 2 classes can always be separated by a [[hyperplane]]
	3. The [[hyperplane]] discovered based on [[support vectors (SV)]] ("essential" training tuples) and margins (defined by the [[support vectors (SV)]])