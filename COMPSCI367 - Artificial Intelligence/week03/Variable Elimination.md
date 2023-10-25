If there is only 1 variable, return the intersection of its (unary [[constraint(s)]])

Otherwise:
- select a variable $X$
- join the [[constraint(s)]] in which $X$ appears, forming [[constraint(s)]] $R1$
- project $R1$ onto its variables other than $X$, forming $R2$
- replace all of the [[constraint(s)]] in which $X$ appears by $R2$
- recursively solve the simplified problem, forming $R3$
- return $R1$ joined with $R3$

> we want to construct a graph that represents the [[Constraint Satisfaction Problem (CSPs)]]; we want to eliminate the variables & introduce a new [[constraint(s)]] that doesn’t involve it


### Example
![[Pasted image 20231023171048.png]]Constraints: 
	$A ≠ B, E ≠ C, E ≠ D, A < D,B < E, D < C, E-A$ is odd
Variables: 
	$A, B, C, D, E$
Domains:
	$A = {1,2}$
	$B = {1,2,3}$
	$C = {3,4}$
	$D = {2,3}$
	$E = {2,3,4}$
![[Pasted image 20231023171158.png]]
they all show all possible combinations

![[Pasted image 20231023171227.png]]
- what it would look like without C

Related to: [[Variable Elimination Algorithm]]