## Objective 
is to maximise:
$$\gamma = \frac{2}{||\vec{w}||}$$
- where $||\vec{w}||$ is the Euclidean norm of $w$
	Equivalently, the objective is to maximise:
	$\min_{w,b} \frac{||\vec{w}||}{2}$
#### Subject to following constraints
$y_i = \begin{cases} +1, & \vec{w} \cdot \vec{x_i} + b \geq +1\\ -1, & \vec{w} \cdot \vec{x_i} + b \leq -1 \end{cases}$
or
$y_i(\vec{w}\cdot \vec{x_i} +b) \ge 1$ , $i=1,2,\dots ,n$ (Uniform form)
- $n$ inequality constraints
This becomes a constrained (convex) quadratic optimization problem:
- Quadratic objective function with linear constraints $\rightarrow$ [[Quadratic Programming (QP)]]
## Duality
[[Support Vector Machines (SVM)]] primal problem form:
	$\min\limits_{w,b} \frac{||\vec {w}||}{2} \quad s.t. \quad y_i(\vec {w} \cdot \vec {x_i} + b) \geq 1, \quad i=1,2,...,n$
1. We can convert it to the dual problem of [[Support Vector Machines (SVM)]] by introducing [[Lagrange Multipliers & Constrained Optimization]] ($\alpha _i$)
	$L(\vec {w},b,\alpha)=\frac{||\vec {w}||}{2}-\sum\limits_{i=1}^n \alpha_i[y_i(\vec{w} \cdot \vec{x_i} + b) - 1], \quad \alpha_i > 0$
2. Solving the primal problem is equivalent to solving the dual problem:
	$\min\limits_{w,b} \frac{||\vec {w}||}{2} \equiv \max\limits_{\alpha} \min\limits_{w,b} L(\vec {w},b,\alpha)$
3. Set the derivatives to [[Support Vector Machines (SVM)]] Lagrangian function with respect to $\vec {w}$ and b to be zero:
	$L(\vec {w},b,\alpha)=\frac{||\vec {w}||}{2}-\sum\limits_{i=1}^n \alpha_i[y_i(\vec{w} \cdot \vec{x_i} + b) - 1], \quad \alpha_i > 0$
	- $\frac{dL}{d\vec {w}} = 0 \Rightarrow \vec{w} = \sum_{i=1}^{n} \alpha_i y_i \vec{x_i}$
	- $\frac{dL}{db} = 0 \Rightarrow \sum_{i=1}^{n} \alpha_i y_i = 0$
4. Substituting them in the Lagrangian function $L$, we obtain the final dual optimization function:
	$$\max_{{\alpha}} \sum_{i=1}^{n} \alpha_i - \frac{1}{2} \sum_{i=1}^{n} \sum_{j=1}^{n} \alpha_i \cdot \alpha_j \cdot y_i \cdot y_j \cdot \vec{x_i} \cdot \vec{x_j}$$
#### Solving the Dual Problem
- **Dual Problem Optimization**
	$$\max_{{\alpha}} \sum_{i=1}^{n} \alpha_i - \frac{1}{2} \sum_{i=1}^{n} \sum_{j=1}^{n} \alpha_i \cdot \alpha_j \cdot y_i \cdot y_j \cdot \vec{x_i} \cdot \vec{x_j}$$
	such that $\alpha _i \ge 0$ and $\sum_{i=1}^{n} \alpha_i y_i = 0$,  $i=1,2,...,n$
	This can be solved efficiently using numerical optimization
	- $a_i > 0$ for [[support vectors]] $\vec {x_i}$ that lie on the margin $H_1$ and $H_2$
	- $a_i = 0$ for other training points
Thus, the solution of $\vec {w}$ corresponding to the maximal margin classifier can be written as a linear combination of just the [[support vectors]]:
$$\vec{w} = \sum_{x_i \in SV} \alpha_i y_i \vec{x_i}$$