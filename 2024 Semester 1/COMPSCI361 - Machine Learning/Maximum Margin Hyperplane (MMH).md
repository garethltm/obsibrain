![[Pasted image 20240605105538.png]]

### For 1D
![[Pasted image 20240605110057.png]]
A separating hyperplane ($H$) can be formally defined as $\vec{w}\cdot \vec{x} +b=0$
- $\vec{w} = \{w_1, w_2, ..., w_n\}$ is a weight vector & $b$ is scalar (bias)
### For 2D
it can be written as: $w_1\cdot x_{i,1}+w_2\cdot x_{i,2}+b =0$,
- The [[hyperplane]]s defining the sides of the margin:
	- $H_1:w_1\cdot x_{i,1}+w_2\cdot x_{i,2}+b\ge 1$, for $y_i$ = +1, and
	- $H_2:w_1\cdot x_{i,1}+w_2\cdot x_{i,2}+b\le 1$, for $y_i$ = -1
Any training tuples (data) that fall on margins $H_1$ or $H_2$ 
- #compsci361example the [[hyperplane]]s defining the margin