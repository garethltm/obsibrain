$$
k(\vec x,\vec z) = \exp\left(-\frac{\|\vec x-\vec z\|}{2\sigma^2}\right), \quad k(\cdot) \in [0,1]
$$
- $\sigma$ is tunable
- sigma ($\sigma$) defines the [[kernel width]] (radius) of a single [[training data]]
	1. high $\sigma$ values mean 'wider kernel' $\rightarrow$ smoother decision boundary
	2. small $\sigma$ values mean 'narrow kernel' $\rightarrow$ like the [[nearest neighbor(s)]]
![[Pasted image 20240606133626.png]]
#compsci361example 
![[Pasted image 20240606133135.png]]
## Bias and Variance
- a [[Non-Linearly Separable Data]] that trades off between the bias and variance
	![[Pasted image 20240606133907.png]]
	- based on [[validation dat]]
