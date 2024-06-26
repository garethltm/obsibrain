- Optimization function: $f=x^2+y^2$

1. Subject to constraint: $g=2x+6y=c$ , with $c=5$
	![[Pasted image 20240605112500.png]]
	- At the minimum of $f$ such that constraint: $\nabla f = a\nabla g$
		- $gradient\ of\ f = a (gradient\ of\ g)$
	- Finding the minimum is then equivalent to solving: $\nabla f - a \nabla g = 0$
2. Subject to constraint: $g=2x +6y-5= 0$
	- Lagrange function (Lagrangian multiplier $\alpha$):
		- $L(x,y,\lambda) = f(x,y) - \alpha g(x,y)$ $= x^2 + y^2 - \alpha(2x + 6y - 5)$
		- Solution for the constrained problem is obtained by solving for points where the partial derivatives $L$ are zero:![[Pasted image 20240605113124.png]]