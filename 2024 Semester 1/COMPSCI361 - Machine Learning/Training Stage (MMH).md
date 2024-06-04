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
- Quadratic objective function with linear constrain