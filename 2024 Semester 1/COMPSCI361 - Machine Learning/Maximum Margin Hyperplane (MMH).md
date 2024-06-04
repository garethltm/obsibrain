![[Pasted image 20240605105538.png]]

### For 1D
![[Pasted image 20240605110057.png]]
A separating hyperplane ($H$) can be formally defined as $\vec{w}\cdot \vec{x} +b=0$
- $\vec{w} = \{w_1, w_2, ..., w_n\}$ is a weight vector & $b$ is scalar (bias)
### For 2D
it can be written as: $w_1\cdot x_{i,1}+w_2\cdot x_{i,2}+b =0$,
- The [[hyperplanes]] defining the sides of the margin:
	- $H_1:w_1\cdot x_{i,1}+w_2\cdot x_{i,2}+b\ge 1$, for $y_i$ = +1, and
	- $H_2:w_1\cdot x_{i,1}+w_2\cdot x_{i,2}+b\le 1$, for $y_i$ = -1
Any training tuples (data) that fall on margins $H_1$ or $H_2$ 
-  are [[support vectors]]

## Linear model
$f(\vec{x}) = \begin{cases} +1, & \vec{w} \cdot \vec{x} + b \geq +1\\-1, & \vec{w} \cdot \vec{x} + b \leq -1\end{cases}$
$+1$ and $-1$ are class labels in this case

1. [[Training Stage (MMH)]]: Learning the model is equivalent to determining the values of $\vec{w}$ and $b$
	- How to find $\vec{w}$ and $b$ from [[training data]] $S$?
2. Testing Stage: Once $\vec{w}$ and b are found, given a [[test data]] ($\vec{x}$). use $f(\cdot)$ to determine the class label
Decision boundary depends only on [[support vectors]]
- If we have data set with same [[support vectors]], decision boundary will be the same