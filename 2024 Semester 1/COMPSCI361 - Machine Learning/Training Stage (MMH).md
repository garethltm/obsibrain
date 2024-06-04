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
	$\min\limits_{w,b} \frac{||w||}{2} \quad s.t. \quad y_i(w \cdot x_i + b) \geq 1, \quad i=1,2,...,n$
We can convert it to the dual problem of [[Support Vector Machines (SVM)]] by introducing [[Lagrange Multipliers & Constrained Optimization]] ($\alpha _i$)
	$L(w,b,\alpha)=\frac{||w||}{2}-\sum\limits_{i=1}^n \alpha_i[y_i(\vec{w} \cdot \vec{x_i} + b) - 1], \quad \alpha_i > 0$
- Solving the primal problem is equivalent to solving the dual problem:
	$\min\limits_{w,b} \frac{||w||}{2} \equiv \max\limits_{\alpha} \min\limits_{w,b} L(w,b,\alpha)$
